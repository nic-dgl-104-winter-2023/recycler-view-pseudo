# Model (data)
The model is where constructs that can be used to access app data are stored. Typically, this means an abstraction layer that is used to represent data in code, paired with functionality that permits the retrieval of data from storage.

*Where* the data itself is stored (e.g. locally in file storage or database, remotely in either) isn't our main concern here. We can mock whatever data we'd like to represent as a form of list.

## Pseudocode
```
LIST all data points

MODEL an abstraction that permits access to data points
```