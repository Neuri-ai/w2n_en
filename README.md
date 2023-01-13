# Word to Number (Spanish) ![GitHub issues](https://img.shields.io/github/issues/Neuri-ai/w2n_en) ![GitHub forks](https://img.shields.io/github/forks/Neuri-ai/w2n_en) ![GitHub stars](https://img.shields.io/github/stars/Neuri-ai/w2n_en) ![GitHub licence](https://img.shields.io/github/license/Neuri-ai/w2n_en)

This is a Python module to convert number words (eg. veintiuno) to numeric digits (21).
It works for positive numbers upto the range of 999,999,999,999 (i.e. billions)
Below is the installation, usage and other details of this module.

## Installation

Please ensure that you have **updated pip** to the latest version before installing word2number_en.

You can install the module using Python Package Index using the below command.

    pip install word2number_en

Make sure you install all requirements given in requirements.txt
```
pip install -r requirements.txt
```
## Usage

First you have to import the module using the below code.

    from word2number_en import w2n

Then you can use the **word_to_num** method to convert a number-word to numeric digits, as shown below.
```
print(w2n.word_to_num("two million two hundred and ninety two thousand and zero"))
2292000
```
```
print(w2n.word_to_num('two poin three')) 
2.3
```
```
print(w2n.word_to_num('112')) 
112
```
```
print(w2n.word_to_num('point five')) 
0.5
```
```
print(w2n.word_to_num('two thousand and twenty three')) 
2023
```
```
print(w2n.word_to_num('million million'))
Error: Redundant number! Please enter a valid number word (eg. two million twenty three thousand and forty nine)
None
```
```
print(w2n.word_to_num('blah'))
Error: No valid number words found! Please enter a valid number word (eg. two million twenty three thousand and forty nine)
None
```

You can also use the **numwords_in_sentence** to convert all number words in a sentence to numeric digits, as shown below.
```
print(w2n.numwords_in_sentence("set a timer for five minutes"))
set a timer for 5 minutes
```



## Contributors
- Ben Batorsky [bpben](https://github.com/bpben)
- Alex [ledovsky](https://github.com/ledovsky)
- Tal Yarkoni [tyarkoni](https://github.com/tyarkoni)
- ButteredGroove [ButteredGroove](https://github.com/ButteredGroove)
- TurqW [TurqW](https://github.com/TurqW)