Linux服务器配置
====
----------------------
[TOC]

----------------------


##2. Python
###2.1 Build SQLite
Django needs SQLite, so the python must be built with SQLite. 
Download the SQLite from the website: [www.sqlite.org](www.sqlite.org).
configure --> make --> make install

### 2.2 Build Python with SQLite
```
cd /usr/local/src
wget https://www.python.org/ftp/python/2.7.8/Python-2.7.8.tgz
tar xvf Python-2.7.8.tgz
```
Build the python with SQLite.
```
cd Python-2.7.8
./configure LDFLAGS='-L<path/to/sqlite-autoconf-3080403/.lib>' CPPFLAGS='-I<path/to/sqlite-autoconf-3080403>'
```
### 2.3 Copy the SQLite dynamic libraries to python lib-dynload
```
cp ./build/lib.linux-i686-2.7/_sqlite3.so  <path/to/python home>/lib/python2.7/lib-dynload/
```

##3. pip

##4. virtualenv

```
virtualenv <env name>
source <path/to/env>/bin/activate
```
## 4.1 virtualenvwrapper
This is a wrapper of virtualenv which can help manage multiple virtualenv. 
source /usr/local/bin/virtualenvwrapper.sh
mkvirtualenv
workon

## 5. Django
```
pip install Django==1.7.1
//Also you can:
//Store the dependence in the requirement.txt file and 
pip install -r requirement.txt
```