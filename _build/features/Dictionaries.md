---
redirect_from:
  - "/features/dictionaries"
interact_link: content/C:\Users\pfsmy\OneDrive\UoM\2019\Jupyter_book\reg_test\content\features/Dictionaries.ipynb
kernel_name: python3
has_widgets: false
title: 'Copy of Jupyter notebooks'
prev_page:
  url: /features/notebooks
  title: 'Jupyter notebooks'
next_page:
  url: 
  title: ''
comment: "***PROGRAMMATICALLY GENERATED, DO NOT EDIT. SEE ORIGINAL FILES IN /content***"
---


# The Python dictionary structure

In Python a dictionary object maps keys to values. A dictionary can hold any number of keys and values but a key cannot be duplicated.

The following code sections show examples of creating a dictionary object and manipulating the keys and values.





<div markdown="1" class="cell code_cell">
<div class="input_area" markdown="1">
```python
# create an empty dictionary
myDict = {}


```
</div>

</div>



#### A dictionary with a single Key-value pair



<div markdown="1" class="cell code_cell">
<div class="input_area" markdown="1">
```python
personDict = {'Name' : 'Peter'}

```
</div>

</div>



#### I can add more about 'Peter' to the dictionary




<div markdown="1" class="cell code_cell">
<div class="input_area" markdown="1">
```python
personDict['Location'] = 'Manchester'

```
</div>

</div>



#### I can print all of the keys and values from the dictionary



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



#### I can print all of the keys and values from the dictionary - and make it look a bit nicer



<div markdown="1" class="cell code_cell">
<div class="input_area" markdown="1">
```python
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



## More on Dictionaries

