# File `test.js`

**Modules**
* [Global](#module-Global)
* [foo](#module-foo)

**Overview:** What's up?



**Copyright** *(c) 2012 Blah Blah Blah***Author** Joe Schmo

**License:** MIT 

**Version:** 1.0.1

# Module Global

**[Functions](#functions)**
* [bar](#bar-x21e8-Boolean ❘ null-)
* [testNamed](#testNamed-file-optional-x21e8-undefined-)


## Functions
### bar()  &#x21e8; `Boolean ❘ null`
I so cool


**Deprecated:** Not a good function







---
### testNamed(file, optional)  &#x21e8; `undefined`
This is a test function   with a description on multiple lines



**Parameters**

| name | type | description |
|------|------|-------------|
| **file** | `String ❘ null` | filename to parse                        this parsing thing is funny business |
| ***optional*** | `Boolean ❘ null` | Changes behavior |



**Fires**: [`foo#one_thing`](module:foo#event:one_thing) [`foo#another`](module:foo#event:another) [`foo#booyah`](module:foo#event:booyah) 

---


# Module foo
Can I get some description please   on more than one line, if possible.

**[Functions](#functions)**
* [testAnonynous](#testAnonynous-x21e8-String-)
* [testAnon2](#testAnon2-x21e8-String-)
* [func1](#func1-a-b-x21e8-)
* [func2](#func2-c-d-x21e8-)
* [testDeprecated](#testDeprecated-x21e8-undefined-)

**[Classes](#classes)**
* [Ketch](#class-Ketch)
* [SampleClass](#class-SampleClass)


## Functions
### testAnonynous()  &#x21e8; `String`
function without name



**Returns:** the result.






---
### testAnon2()  &#x21e8; `String`
second function without name



**Returns:** the result.






---
### func1(a, b)  &#x21e8; 



**Returns:** the result.

**Parameters**

| name | type | description |
|------|------|-------------|
| **a** |  | the first param |
| **b** |  | the second param |




---
### func2(c, d)  &#x21e8; 



**Returns:** the other result.

**Parameters**

| name | type | description |
|------|------|-------------|
| **c** |  | the first param |
| **d** |  | the second param |




---
### testDeprecated()  &#x21e8; `undefined`
This is a deprecated function.


**Deprecated:** Because I said so






---


## Classes
* [Ketch](#class-Ketch)
* [SampleClass](#class-SampleClass)

## Class: Ketch
Provides chainable functions to easily build and execute a command.
***
### Members

| name | type | description |
|------|------|-------------|
| **last_err** | `String` | Last error, if present |
| **cmd** | `Array` | Internal array representation of this command. |
***

## Class: SampleClass
This is a class
***

### Methods
* [func1](#func1-a-b-x21e8-)
* [testAnonynous](#testAnonynous-x21e8-String-)
* [testNamed](#testNamed-file-optional-x21e8-undefined-)
***
### func1(a, b)  &#x21e8; 
A method in the class

**Example**:
```
func1(1, 2)
```


**Returns:** the result.

**Parameters**

| name | type | description |
|------|------|-------------|
| **a** |  | the first param |
| **b** |  | the second param |




---
### testAnonynous()  &#x21e8; `String`
function without name



**Returns:** the result.






---
### testNamed(file, optional)  &#x21e8; `undefined`
This is a test method     with a description on multiple lines



**Parameters**

| name | type | description |
|------|------|-------------|
| **file** | `String ❘ null` | filename to parse                          this parsing thing is funny business |
| ***optional*** | `Boolean ❘ null` | Changes behavior |



**Fires**: [`foo#one_thing`](module:foo#event:one_thing) [`foo#another`](module:foo#event:another) [`foo#booyah`](module:foo#event:booyah) 

---
