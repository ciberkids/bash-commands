# bash-commands
Self made bash commands

### Install

```
dir=${HOME}/usr/local/bin/
mkdir -p ${dir}
cd ${dir}
pushd .
git clone git@github.com:ciberkids/bash-commands.git
popd
```


### remember to add this to your bashrc




```
while IFS= read -r dir
do
    PATH="$dir:$PATH"
done < <(find $HOME/usr/local/bin -type d  -not -name '.git' -not -path '*/.git/*')

```

or use :

[https://github.com/ciberkids/bash-home]
