# unique-dictionaries

## The Problem:

Given N lists of dictionaries, create a single list of dictionaries with one "unique" version of each dictionary
A dictionary is considered unique if it has the same "name" and "version" field
e.g.

```json
input1 = [
    {
        "name": "foo",
        "version": "1.0",
        "comment": "foo v1"
    },
    {
        "name": "bar",
        "version": "1.0",
        "comment": "bar v1"
    },
]

input2 = [
    {
        "name": "foo",
        "version": "1.0",
        "comment": "foo version 1"
    },
    {
        "name": "bar",
        "version": "2.0",
        "comment": "bar v2"
    },
]

input3 = [
    {
        "name": "foo",
        "version": "3.0",
        "comment": "foo v3"
    }
]

output = [
    {
        "name": "foo",
        "version": "1.0",
        "comment": "foo v1"
    },
    {
        "name": "bar",
        "version": "1.0",
        "comment": "bar v1"
    },
    {
        "name": "bar",
        "version": "2.0",
        "comment": "bar v2"
    },
    {
        "name": "foo",
        "version": "3.0",
        "comment": "foo v3"
    }
]
```
