# Run a script from a zip file

Nice little trick to package a python program or slip something past a malware scanner

You could stick it inside anything that's based on zip like a jar, apk, docx, etc. You can even [make it executable](https://docs.python.org/3/library/zipapp.html#specifying-the-interpreter).

```
$ mkdir test
$ echo "print('hello world')" > test/__main__.py
$ zip -j test.zip test/*
$ python3 test.zip
hello world
$
```


### references

[@indiecom](https://twitter.com/indiecom/status/1255555099088338946)
[(backup)](https://archive.is/1pAex)