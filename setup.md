---
layout: page
title: Setup
permalink: /setup/
---

## CURL

The code is based on cURL. cURL is an open source command line tool and library for transferring data with URL syntax. cURL is used in command lines or scripts to transfer data.

 * Please check the dependencies before you start.
 * You will also need test credentials for the epic server.


#### Install cURL dependencies

CURL: is an open source command line tool and library for transferring data with URL syntax.
On the training machines

```py
apt-get install curl
apt-get install uuid-runtime
```

#### Own laptop

In case you are working on your own laptop with your own python, please install:

```py
easy_install curl
easy_install uuid-runtime
```

Final check

```py
curl --help
```

If you write the code described below in a file, don't forget to change the permissions.
You should make each file executable.

Suppose you have a file `filename.sh`

you can make it by doing as:
`chmod +x filename.sh`

so it will execute when you type
`./filename.sh`

## EpicClient

The code is based on the [epicclient.py](https://github.com/EUDAT-B2SAFE/B2SAFE-core/blob/master/cmd/epicclient.py).
Please check the dependencies before you start.
You will also need test credentials for the epic server. On the user interface, credentials are located in *credentials/cred_epic*

Please download the epicclient.py.
```sh
wget https://raw.githubusercontent.com/EUDAT-Training/B2SAFE-B2STAGE-Training/develop/code/epicclient.py
```

#### Install python dependencies

On the user interface machine you will find python compiler preinstalled with all neceassary dependencies, we also offer ipython for convenient testing:
```sh
python
```
or
```
ipython
```

#### Own laptop
In case you are working on your own laptop with your own python, please install:

```sh
easy_install httplib2
easy_install simplejson
easy_install lxml
easy_install defusedxml
```

Final check

```sh
python epicclient.py --help
```

## b2handle

## Prerequisites
If you are not working on one of our test machines you need to install the B2HANDLE library and apply for a prefix. For instructions please follow the documentation:

https://github.com/EUDAT-B2SAFE/B2HANDLE/blob/master/README.md

http://eudat-b2safe.github.io/B2HANDLE/handleclient.html#authentication
