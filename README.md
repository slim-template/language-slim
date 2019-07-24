# Slim Atom language package

## Description

This is the [Atom](http://atom.io/) language package, converted from the [Slim TextMate/Sublime bundle](https://github.com/slim-template/ruby-slim.tmbundle).

## Contributing

Grammar is pulled as YAML from [slim-template/ruby-slim.tmbundle](https://github.com/slim-template/ruby-slim.tmbundle) and converted to CSON, additional changes might be done to the resulting _grammars/ruby slim.cson_ file.

```sh
npm install
wget https://raw.githubusercontent.com/slim-template/ruby-slim.tmbundle/master/Syntaxes/Ruby%20Slim.YAML-tmLanguage
node_modules/.bin/yaml2json "Ruby Slim.YAML-tmLanguage" -p | node_modules/.bin/json2cson --2spaces > "grammars/ruby slim.cson"
```

Optionally, make changes to _grammars/ruby slim.cson_. Preview the results by rebuilding/linking the package and previewing _demo.slim_.

```sh
apm rebuild && apm link && atom .
```

## Author

[Fred Wu](http://fredwu.me/)
