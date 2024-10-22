Enron was an infamous large company that had fraudulent activities in accounting practices. There are 500,000 emails generated by the employees of Enron Corp. These emails were obtained by the Federal Energy Regulatory Commission during it's investigation of Enron Corps collapse.
You are assigned as an employee of the Federal Energy Regulatory Commission is to index all emails containing a particular word. Unfortunately, your employer is cheap and didn't give you a proper computer. You have a device with limited RAM and CPU, but unlimited disk space.

### Task
Given a word, we want to return a list of numbers indicating in which email it was contained. We consider words a sequence of lower case (a-z) and upper case A Z letters. Every other character can be considered as a delimiter.
The program has to run in a very constrained computation budget, therefore a linear search, as done by grep , would take too long. You need to provide a faster solution. You can also not load the entire dataset into memory.
You have access to a computer with higher resources which can be used for preprocessing the dataset if necessary.

## Example 1:
```
> grep -R "Tesla" .
None
$ your_query_program [datastructure_path] Tesla
```
### Example 2:
```
> grep -R "OceanConnect" .
  ./21891.txt:* Chemoil takes stake in OceanConnect
./21891.txt:Thomas Reilly, OceanConnect's president, announced
./21891.txt:and is using OceanConnect as its exclusive
$ your_query_program [datastructure_path] OceanConnect
21891
```

### Example 3:
```
 grep -R "feedwater" .
./1732.txt:the other for unplanned maintenance on boiler feedwater pumps, which could
./2665.txt:the other for unplanned maintenance on boiler feedwater pumps, which could
./1021.txt:the other for unplanned maintenance on boiler feedwater pumps, which could
./509.txt:the other for unplanned maintenance on boiler feedwater pumps, which could
$ your_query_program [datastructure_path] OceanConnect
1732
2665
1021
509
```

### Download dataset
https://drive.google.com/file/d/1XFk1wpS2JEj4TcgHVtQdjAVPVnzJuXAC Dataset contains 30503 emails.

### Constraints
- A word is defined as \s[a-zA-Z]\s .
- Lower or upper case character surrounded by spacing or any other
character (e.g. , . !

### Submission details
You may use any programming language. Using standard libraries is allowed, but you should not use high level libraries.
The code should have no external dependencies (except the basic environment, e.g. c++ compiler, python environment), and needs to have a description of how to setup the environment/compile the code.
  SW Task 2

Your programs (feel free to change their name) should receive the following arguments:

### Preprocessing program:
`your_preprocessing_program [dataset_path] [datastructure_path]`

### Query program:
`your_query_program [datastructure_path] [query_word]`
Please send your code back as an archived single file (e.g. zip, tar) per email. We wish you good work!
