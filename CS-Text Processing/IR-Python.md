# IR - Python

```python
def count_words(filename, stops):
    wordRE = re.compile(r'[A-Za-z]+')   # list words
    counts = {}		# word:count
    with open(filename, 'r') as infile:
        for line in infile:
            for word in wordRE.findall(line.lower()): 	# lowercase
                if word not in stops: 
                    if word not in counts:
                        counts[word] = 0
                    counts[word] += 1
    return counts
```

## Dictionary

`get(key, 0)` -  if key not in dictionary, return 0.

## File

`open(filename, mode)` 

​	There are four different methods (modes) for opening a file:

​	`	"r"` - Read - Default value. Opens a file for reading, error if the file does not exist

​	`	"a"` - Append - Opens a file for appending, creates the file if it does not exist

​	`"w"` - Write - Opens a file for writing, creates the file if it does not exist

​	`"x"` - Create - Creates the specified file, returns an error if the file exists

​	In addition you can specify if the file should be handled as binary or text mode

​	`"t"` - Text - Default value. Text mode

​	`"b"` - Binary - Binary mode (e.g. images)

