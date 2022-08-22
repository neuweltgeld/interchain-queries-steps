# ICQ

## If you get "icq not found" error try this
### These commands permanently delete all files of existing icq installation

```
cd $HOME
rm -rf interchain-queries
rm -rf /usr/local/bin/icq
rm -rf .icq
rm -rf /etc/systemd/system/icqd.service
```

## Install go

```
wget -c https://go.dev/dl/go1.18.3.linux-amd64.tar.gz && rm -rf /usr/local/go && tar -C /usr/local -xzf go1.18.3.linux-amd64.tar.gz && rm -rf go1.18.3.linux-amd64.tar.gz
```
```
echo 'export GOROOT=/usr/local/go' >> $HOME/.bash_profile
echo 'export GOPATH=$HOME/go' >> $HOME/.bash_profile
echo 'export GO111MODULE=on' >> $HOME/.bash_profile
echo 'export PATH=$PATH:/usr/local/go/bin:$HOME/go/bin' >> $HOME/.bash_profile && . $HOME/.bash_profile
```

## Install icq again



***************************

## Error parsing chain config: default chain (stride-testnet) configuration not found error

Make sure your .icq/config.yaml file is valid.
The spaces at the beginning of the lines are important. Set it like this.

![image](https://user-images.githubusercontent.com/101174090/185809736-b8b88ea0-7347-457e-96dd-59358da687d1.png)
