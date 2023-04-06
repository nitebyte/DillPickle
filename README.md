# DillPickle

DillPickle is a Python program that generates a company diligence report for a list of companies located in towns.csv. The program uses OpenAI's GPT-3 language model to generate text for each section of the report. The generated text is then saved to a text file and converted to a Microsoft Word document using the python-docx library.

## Installation
1. Clone this repository
```
git clone https://github.com/nitebyte/DillPickle.git
```
2. Install the required modules:

   - `openai`
   - `ebooklib`
   - `docx`
   - `requests`
   - `json`
   
3. Get an OpenAI API key [here](https://beta.openai.com/signup/).
4. Replace the `api_key` in the `PR` function and the `headers` dictionary with your OpenAI API key.
5. Run the program with the command:
```
python TripTeller.py
```
6. Your completed reports(s) will be saved as a `.docx` file in the same directory.

## Usage

1. Add the names of the towns and states you want to generate reports for to towns.csv.
2. Run DillPickle.py: `python DillPickle.py`
3. The program will generate a text file for each town in the format "Town Name State.txt".
4. The text files will be converted to Microsoft Word documents in the format "Town Name State.docx".

## Example

Suppose towns.csv contains the following entries:

```
Boeing Co, Null
Weyland-Yutani, Null
```

Running DillPickle.py will generate the following files:

```
Boeing Co, Null.txt
Boeing Co, Null.docx
Weyland-Yutani, Null.txt
Weyland-Yutani, Null.docx
```

The text files will contain the generated text for each section of the company diligence report for the respective town. The Microsoft Word documents will contain the same text formatted as a book with a title page, copyright page, dedication page, and table of contents.

## Credits
- OpenAI
- ebooklib
- csv
- requests
- json
- io
- python-docx

## License
DillPickle is licensed under the MIT License. See LICENSE for more information.
