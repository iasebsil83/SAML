# ***SAML : Simply A Markup Language***

**The simplest syntax to describe a data structure.**

&nbsp;

&nbsp;


# Content

This project is divided in different branches :
- [master](https://github.com/iasebsil83/SAML), General information about the SAML.
- [python](https://github.com/iasebsil83/SAML/tree/python), library for reading/writting SAML in Python.
- [C     ](https://github.com/iasebsil83/SAML/tree/c), library for reading/writting SAML in C.
- [JS    ](https://github.com/iasebsil83/SAML/tree/javascript), library for reading/writing SAML in JavaScript.
- [Kotlin](https://github.com/iasebsil83/SAML/tree/kotlin), library for reading/writting SAML in Kotlin.
- [Go    ](https://github.com/iasebsil83/SAML/tree/go), library for reading/writting SAML in Go.
- [Lua   ](https://github.com/iasebsil83/SAML/tree/lua), library for reading/writting SAML in Lua.

We are currently on branch **master**.

&nbsp;

&nbsp;


# Objective

This language is inspired on the basics of the [YAML](https://yaml.org).

SAML is a serializable data syntax including the minimum rules in order to be interpreted the fastest and the easiest way.

It has been made as **simple** as possible to be read and written by any kind of program.

The objective behind SAML is to get/set information from a data file as quickly as possible.

That means that the syntax must be the lightest possible and restrictive.

***NOTE:*** The default SAML syntax is **included** into the YAML syntax.

That means that a YAML reader can understand a SAML text but the opposite is not totally true.

&nbsp;

&nbsp;


# Rules

Here are all the rules of the SAML syntax :

```
- No empty line is allowed.
- Comments are allowed and concerns every line starting with a COMMENT CHARACTER.
- Every non-commented line must be composed by :
  - A serie of consecutive TABULATION CHARACTERS (describing the depth degree of the data)
  - The key name of the current piece of data
  - A SEPARATION CHARACTER
  - The corresponding data
  - An END CHARACTER
- Key names must contain only alphanumerical characters and underscores [a-z] + [A-Z] + [0-9] + '_'.
- Key names must not start with a digital character [0-9].
- Data can be either boolean, character, integer, float or string :
  - Booleans must be either true or false.
  - Characters must be delimited between simple quotes '\''.
    They can contain any special character.
  - Integers must be only composed of numerical characters except the first one that can be a negative sign '-'.
  - Floats must respect the same rules as integers with the exception that a dot '.' is allowed as coma and numbers allowed as well after this.
  - Strings must be delimited by double quotes '\"'.
    They can contain any special caracter too.
- There is no maximum number of character for key names/data fields but the minimum number is 1.
- Every key-value pair must have a data field except if it has children pairs.
- Every line indented one more time from the previous one is a child of this one.
- Every line indented the same as the previous one is a brother of this one.
```

As you might have seen, there is a set of **special characters** that must be defined.

By default, these characters are :
```
COMMENT    CHARACTER : '#'
END        CHARACTER : '\n' (line feed)
SEPARATION CHARACTER : ':'
TABULATION CHARACTER : '\t' (tabulation)
```
They are customizable at the beginning of all SAML programs/libraries.

***WARNING:*** Do not use alphanumerical characters as special (including underscores) or you may have surprises !

Also pay attention to the character used, especially because of its encoding.

&nbsp;

&nbsp;


*Contact     : i.a.sebsil83@gmail.com*<br>
*Youtube     : https://www.youtube.com/user/IAsebsil83*<br>
*GitHub repo : https://github.com/iasebsil83*<br>

Let's Code ! &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;By I.A.
