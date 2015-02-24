# jsTextManager
jsTextManager is a simple tool to manipulate string in Javascript.

Essentially all you have to do is download TexManager.html and open it in a browser.

The code is written in pure Js, without using any external object so it could be used also offline.

__BE CAREFUL:__ jsTextManager is tested on Chrome 40.0.2214.115 (64-bit) for OsX.


![image](https://github.com/gianx/jsTextManager/blob/master/Screenshot/TextManager_1.png)

From this screen you can do some operations with the text:

#### General functions 
_ALL UPPER_: Converts all the text uppercase;

_ALL LOWER_: Converts all the text lowercase;

_REMOVE EMPTY LINES_: Removes all empty lines (both Unix and Windows formats);

### Extract
_URLS_: Extracts all the URLs embedded in the text;

_EMAIL_: Extracts all the Emails embedded in the text;

### Encode

_URI ENCODE_: Performs an encoding off each line of the text;

_URI DECODE_: Performs a decoding off each line of the text;

_XML ENCODE_: Replaces all XML need-to-be-escaped chars;

_XML DECODE_: Replaces all XML escape sequences with correspondents chars;

### ROWS

_ENUMERATE_: Enumerates all rows;

_LTRIM_: Removes spaces from the beginning of all rows;

_RTRIM_: Removes spaces from the ending of all rows;

### SINGLE PARAMETER

_AFTER ALL_: Inserts the parameter at the end of the text;

_AFTER EACH_: Inserts the parameter after each row;

_BEFORE ALL_: Inserts the parameter at the beginning of the text;

_BEFORE EACH_: Inserts the parameter before each line;

_COUNT_: Counts the occurrences of parameter;

_DELETE FROM CHAR_: Deletes each row from the string specified by the parameter;

_DELETE TO CHAR_: Deletes each row from the beginning to the firs occurrence of the string specified by the parameter;

_ENCAPSULATE_: Encapsulates each row with the parameter (it's inserted at the beginning and at the end of each lines);

_JOIN_: Merges rows in one using parameter as a separator

_REMOVE_: Removes every occurence of the parameter from the text;

_SPLIT_: Splits text into lines using parameter as delimiter;

### DELETE

_FIRST_: Deletes first X chars of each row;

_LAST_: Deletes last X chars of each row;

### REPLACE

_REPLACE_: Replaces all the occurences of a string with another;

### PAD

_ON LEFT_: Adds a number of a specified char on the left of each row to reach the specified length;

_ON RIGHT_: Adds a number of a specified char on the right of each row to reach the specified length;

### SPECIAL

_ORACLE IN_: Transform the text in a text suitable for using with PL-SQL insert putting all lines between "'", adding "," at the end of the line and putting all the text between "()".

For example:

	A
	B
	C
	D
	E
	
Becomes:

	('A',
	'B',
	'C',
	'D',
	'E')