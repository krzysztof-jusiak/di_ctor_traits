**Dependency Injection Constructor Traits** python script based on lib clang generating constructor traits. Useful for third party libraries, which can't be changed.

[![Code Health](https://landscape.io/github/krzysztof-jusiak/di_ctor_traits/master/landscape.png)](https://landscape.io/github/krzysztof-jusiak/di_ctor_traits/master)

### Requirements
 + [python](http://www.python.org) (tested with 2.7 and 3.3)
 + [libclang](http://clang.llvm.org) (tested with 3.2 and 3.3)

### Download
```
git clone --recursive git@github.com:krzysztof-jusiak/di_ctor_traits.git
```

### Usage
```
Usage: di_ctor_traits.py [options] files...

Options:
  -h, --help                    show this help message and exit
  -o OUTPUT, --output=OUTPUT    output file (default='di_ctor_traits.hpp')
  -l LIMIT, --limit=LIMIT       limit to constructors within declaration (default='')

```

### Example
```sh
./di_ctor_traits.py -o di_ctor_traits.hpp -l "namespace::class" files...
```

