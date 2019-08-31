---
redirect_from:
  - "/features/dictionaries"
interact_link: content/C:\Users\Pete_local\OneDrive\UoM\2019\Jupyter_book\reg_test\content\features/Dictionaries.ipynb
kernel_name: python3
has_widgets: false
title: 'Dictionaries'
prev_page:
  url: /features/notebooks
  title: 'Jupyter notebooks'
next_page:
  url: 
  title: ''
comment: "***PROGRAMMATICALLY GENERATED, DO NOT EDIT. SEE ORIGINAL FILES IN /content***"
---


# The Python Dictionary data structure

In Python a dictionary object maps keys to values. A dictionary can hold any number of keys and an associated value, but a key cannot be duplicated, it must be unique.

The following code sections show examples of creating a dictionary object and manipulating the keys and values.





<div markdown="1" class="cell code_cell">
<div class="input_area" markdown="1">
```python
# create an empty dictionary
myDict = {}
print(myDict)


```
</div>

</div>



#### A dictionary with a single Key-value pair



<div markdown="1" class="cell code_cell">
<div class="input_area" markdown="1">
```python
personDict = {'Name' : 'Peter'}
print(personDict)

```
</div>

</div>



#### I can add more about 'Peter' to the dictionary

Once a dictionary has been created you can addd more keys, but remember that the key name must be unique.



<div markdown="1" class="cell code_cell">
<div class="input_area" markdown="1">
```python
personDict['Location'] = 'Manchester'
personDict['Age'] = '61'

```
</div>

</div>



#### I can print all of the keys and values from the dictionary as a list of tuples



<div markdown="1" class="cell code_cell">
<div class="input_area" markdown="1">
```python
print(personDict.items())

```
</div>

<div class="output_wrapper" markdown="1">
<div class="output_subarea" markdown="1">
{:.output_stream}
```
dict_items([('Name', 'Peter'), ('Location', 'Manchester')])
```
</div>
</div>
</div>



#### or all of the keys



<div markdown="1" class="cell code_cell">
<div class="input_area" markdown="1">
```python
print(personDict.keys())

```
</div>

<div class="output_wrapper" markdown="1">
<div class="output_subarea" markdown="1">
{:.output_stream}
```
dict_keys(['Name', 'Location'])
```
</div>
</div>
</div>



#### or all of the values



<div markdown="1" class="cell code_cell">
<div class="input_area" markdown="1">
```python
print(personDict.values())

```
</div>

<div class="output_wrapper" markdown="1">
<div class="output_subarea" markdown="1">
{:.output_stream}
```
dict_values(['Peter', 'Manchester'])
```
</div>
</div>
</div>



#### I can print all of the keys and values from the dictionary - and make it look a bit nicer



<div markdown="1" class="cell code_cell">
<div class="input_area" markdown="1">
```python
# 'item' is simple a made up variable name. The for loop iterates over the keys in the dictionary
for item in personDict:
    print(item, "=", personDict[item])

```
</div>

<div class="output_wrapper" markdown="1">
<div class="output_subarea" markdown="1">
{:.output_stream}
```
Name = Peter
Location = Manchester
```
</div>
</div>
</div>




#### I can access the value for a given key





<div markdown="1" class="cell code_cell">
<div class="input_area" markdown="1">
```python
x = personDict['Name']
print(x)

```
</div>

<div class="output_wrapper" markdown="1">
<div class="output_subarea" markdown="1">
{:.output_stream}
```
Peter
```
</div>
</div>
</div>



#### I can change value for a given key






<div markdown="1" class="cell code_cell">
<div class="input_area" markdown="1">
```python
personDict['Name'] = "Fred"
print(personDict['Name'])

```
</div>

<div class="output_wrapper" markdown="1">
<div class="output_subarea" markdown="1">
{:.output_stream}
```
Fred
```
</div>
</div>
</div>



#### I can check if a key exists




<div markdown="1" class="cell code_cell">
<div class="input_area" markdown="1">
```python
key = 'Name'

if key in personDict :
    print("already exists")
else :
    personDict[key] = "New value"

```
</div>

<div class="output_wrapper" markdown="1">
<div class="output_subarea" markdown="1">
{:.output_stream}
```
already exists
```
</div>
</div>
</div>



#### Checking whether a key exists or not is a very common action.

When we were adding keys, we did so by simply referencing the (new) Key name and assigning a value to it.

If the key already existed, then we would have simply overwritten the its previous value. This would be valid code and would not produce an error.



## More complex Dictionaries

The value assigned to a dictionary key can be of any data type. So far we have used simple strings and integers.



<div markdown="1" class="cell code_cell">
<div class="input_area hidecode" markdown="1">
```python
# This is a hidden code cell
print("Hello World")

```
</div>

<div class="output_wrapper" markdown="1">
<div class="output_subarea" markdown="1">
{:.output_stream}
```
Hello World
```
</div>
</div>
</div>



### This is a markup cell after the hidden cell

