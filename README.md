# ULID

>__Note:__ Forked from [mdipierro/ulid](https://github.com/mdipierro/ulid) by Massimo Di Pierro

## Universally Unique Lexicographically Sortable Identifier ([Spec](https://github.com/ulid/spec))

A ULID is built with two constituent parts; a Timestamp and 80 bits of Randomness. As an alternative to a the UUID variations. ULIDs offer the following features:
*  128-bit compatibility with UUID
* 1.21e+24 unique ULIDs per millisecond
* Lexicographically sortable!
* Canonically encoded as a 26 character string, as opposed to the 36 character UUID
* Uses Crockford's base32 for better efficiency and readability (5 bits per character)
* Case insensitive
* No special characters (URL safe)

### Design

**Timestamp**
- 48 bit integer
- UNIX-time in milliseconds
- Won't run out of space 'til the year 10889 AD.

**Randomness**
- 80 bits
- Cryptographically secure source of randomness, if possible

### Design - String Representation

```
ttttttttttrrrrrrrrrrrrrrrr

where
t is Timestamp
r is Randomness
```

## Changes:
* Modified/Simplified README.md
* Convered ULID Python Code into Class
* Simplified Project Structure for Class / Git Submodule Use
* Removed Setup.py / PIP Code

## Licence
MIT Licence (as per original 2016 project by Massimo Di Pierro)

## Thanks
* [Massimo Di Pierro](https://github.com/mdipierro) for the Python Source
* [ULID Spec Contributors](https://github.com/ulid/spec) for the design and specification work