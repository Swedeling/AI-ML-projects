# Speaker Recognition

This project is part of my engineering thesis "Automatic Identity Recognition Using Speech Biometric". The main assumptions of the project include creating the most effective solution that will enable the identification of 34 speakers based on 14 recordings of individual words from each of them.


## [Data Selection](https://github.com/Swedeling/Portfolio/blob/main/SpeakerRecognition/data_selection.ipynb)

The data used during the project implementation comes from the free [Common Voice](https://commonvoice.mozilla.org) database. It is an open source collection of recordings of the human voice in various languages. A database of single-word recordings in English was selected for this project. The words spoken are "zero", "one", "two", "three", "four", "five", "six", "seven", "eight", "nine", "yes", "no", "Hey", "Firefox". Such a selection of words is due to the fact that they are universal and most often used for user verification (for example with a PIN code), which is one of the applications of speaker recognition systems.
The entire collection contained 16,285 short recordings of words spoken by various users. Therefore, I decided to standardize and limit them. In this [section](https://github.com/Swedeling/Portfolio/blob/main/SpeakerRecognition/data_selection.ipynb) you can find my data selection process. 

## [Silence Removing](https://github.com/Swedeling/Portfolio/blob/main/SpeakerRecognition/silence_removing.ipynb)
Voice data can be divided into three segments: speech segment, silence segment, and background noise. Depending on the recording conditions, their ratio may be different. If you want to obtain high classification results, you should take care of the "purity" of the signal. In order to extract the voice parts, I decided to use an endpoint detection algorithm and unnecessary parts removing. For the purposes of this project, the algorithm described in "A New Silence Removal and Endpoint Detection Algorithm for Speech and Speaker Recognition Applications" was used. [1]. 

Its operation is presented in the diagram below.
![tekst alternatywny](../docks/schemat1.png)

In this [section](https://github.com/Swedeling/Portfolio/blob/main/SpeakerRecognition/silence_removing.ipynb) you can find my implementaion of it. 

A sample result of the operation:

!["one" - raw signal ](../docks/silence1.png)

!["one" - after silence removing](../docks/silence2.png)

```python
import numpy as np
```

## Logistic Regression
asdaksd





## Bibliography

[1] Saha, Goutam & Chakroborty, S.S. & Senapati, Suman. (2005). A New Silence Removal and Endpoint Detection Algorithm for Speech and Speaker Recognition Applications.