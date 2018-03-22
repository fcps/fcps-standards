## <a name="metadata"></a> 3. Metadata requirements/Practices
Explains what [codebooks](#codebook), [data dictionaries](#dataDictionary), [value labels](#valueLabels), and [variable labels](#variableLabels) are, when they are used, what they should contain, and why they are important.  Binding metadata to the data source helps ensure that there is always sufficient documentation built into the data to allow any end user to more quickly/easily get up and running with a data set.  These sections should also explain when these elements are required as part of data deliverables.

[Back to the Top](#top)  [Back to Table of Contents](#dataStandardsTOC)

### <a name="codebook"></a> Codebooks
This section would explain what a codebook is.  Codebooks have two primary functions:

  1. Explain numeric mappings to semantic meanings 
  2. Show basic distribution properties of a variable

For example, if we code student sex with a [bit](#dataTypes) type with values of 0 and 1 how would an end user know which numeric value represents female?  The codebook would provide this explanation as well as show the distribution of some/all of the values for basic validation/verification:

Value | Label  | Freq. | Pct.
----- | ------ | ----- | -----
0     | Male   | 4,900 | 49%
1     | Female | 5,100 | 51%

[Back to the Top](#top) [Back to Top of Section](#metadata) [Back to Table of Contents](#dataStandardsTOC)

### <a name="dataDictionary"></a> Data Dictionary
Any time a file is delivered to an end-user there must be sufficient metadata embedded in the file to allow the user to 
easily and unambiguously derive meaning from the values contained in each column of the data.  When the file being provided 
is not a plain text file, these metadata shall be permanently bound to the data itself.  

In SQL we can accomplish this goal through the use of column comments, or extended properties in SQL Server.  There is
extensive documentation and some examples of how to accomplish this in [MS SQL Server](https://technet.microsoft.com/en-us/library/ms190243(v=sql.105).aspx)
and an example is provided below for convenience:

__Example.__ _Attaching metadata to table and column in SQL Server._
```SQL
CREATE TABLE [dbo].example (
    id INT PRIMARY KEY,
    female BIT NOT NULL
);

-- Adds a comment to a table
EXEC sys.sp_addextendedproperty 
    @name = 'MS_Description',
    @value = 'Table contains an identifier and indicator of whether the individual is a female',
    @level0type = 'SCHEMA', @level0name = dbo,
    @level1type = 'TABLE', @level1name = example;

-- Adds a comment to an individual column of a table
EXEC sys.sp_addextendedproperty 
    @name = 'MS_Description',
    @value = '0 = Male / 1 = Female - Indicates the biophysiological sex of the student',
    @level0type = 'SCHEMA', @level0name = dbo,
    @level1type = 'TABLE', @level1name = example,
    @level2type = 'COLUMN', @level2name = female;

```

In statistical software packages like [Stata](https://www.stata.com) this can be accomplished through the use of variable labels:

__Example.__ _Attaching metadata to dataset and variables in [Stata](https://www.stata.com)._
```Stata
// Clear memory
clear

// Create a data set with some data
input byte id byte female
1 0
2 0
3 1
4 0 
5 1
6 1
7 1
end

// Now attach metadata to the female variable
la var female "Indicates the biophysiological sex of the student"

// This could also be written without abbreviations as:
label variable female "Indicates the biophysiological sex of the student"

// We can add meta data to the dataset as a whole in a couple different ways:

// This will attach the metadata to a characteristic
char _dta[comment] "Dataset contains an identifier and indicator of whether the individual is a female"

// You can also add the data as a note
note: Dataset contains an identifier and indicator of whether the individual is a female
```


[Back to the Top](#top) [Back to Top of Section](#metadata) [Back to Table of Contents](#dataStandardsTOC)

### <a name="valueLabels"></a> Labeling Numerically Encoded Data

[Back to the Top](#top) [Back to Top of Section](#metadata) [Back to Table of Contents](#dataStandardsTOC)

### <a name="variableLabels"></a> Labeling Variables/Columns

[Back to the Top](#top) [Back to Top of Section](#metadata) [Back to Table of Contents](#dataStandardsTOC)



