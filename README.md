Bash Testing Script
===================

Script to test bash projects

When the test.sh script is run, it will check all files in the src/ directory. It will exit 1 on error, and 0 on success.

An example usage in a `.travis.yml` file for [travis-ci](http://travis-ci.org).

```
language: sh
install:
- wget https://raw.github.com/daboross/bash-test-script/master/test.sh -O test.sh
- chmod 775 test.sh
script: ./test.sh
```
