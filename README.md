[gae link pip helper · kaichu.io](http://kaichu.io/2016/03/gae-link-pip-helper/)

## Quick tutorial

```bash
# git clone repo
$ git clone git@github.com:cage1016/link-pip-helper.git
Cloning into 'link-pip-helper'...
remote: Counting objects: 7, done.
remote: Compressing objects: 100% (5/5), done.
remote: Total 7 (delta 0), reused 7 (delta 0), pack-reused 0
Receiving objects: 100% (7/7), done.
Checking connectivity... done.

# switch to link-pip-helper
$ cd link-pip-helper/

# 利用 virtualenvwrapper 建立 virtualenv
$ mkvirtualenv link-pip-helper-tutorial
New python executable in /Users/{HOME}/.virtualenvs/link-pip-helper-tutorial/bin/python2.7
Also creating executable in /Users/{HOME}/.virtualenvs/link-pip-helper-tutorial/bin/python
Please make sure you remove any previous custom paths from your /Users/{HOME}/.pydistutils.cfg file.
Installing setuptools, pip, wheel...done.
virtualenvwrapper.user_scripts creating /Users/{HOME}/.virtualenvs/link-pip-helper-tutorial/bin/predeactivate
virtualenvwrapper.user_scripts creating /Users/{HOME}/.virtualenvs/link-pip-helper-tutorial/bin/postdeactivate
virtualenvwrapper.user_scripts creating /Users/{HOME}/.virtualenvs/link-pip-helper-tutorial/bin/preactivate
virtualenvwrapper.user_scripts creating /Users/{HOME}/.virtualenvs/link-pip-helper-tutorial/bin/postactivate
virtualenvwrapper.user_scripts creating /Users/{HOME}/.virtualenvs/link-pip-helper-tutorial/bin/get_env_details

# pip 安裝相依套件
$ pip install -r requirements.txt
Collecting google-api-python-client==1.4.0 (from -r requirements.txt (line 1))
....

# 執行 shell (你可以將 link pip.sh 內容 export 成任何 function 名)
$ link_pip lib

# 本地執行 Google App Engine
$ dev_appserver.py .
```