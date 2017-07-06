### 生成ssh-keygen

#### 首先查看本地是否有ssh秘钥

```
	cat ~/.ssh/id_rsa.pub
```

#### 如果没有可通过以下命令生成ssh

```
	ssh-keygen -t rsa -C "your email"
```

#### 一路回车...

#### 成功后进入.ssh目录查看且复制公钥

```
	cat ~/.ssh/id_rsa.pub
```

复制命令

#### Windows:

```
	clip < ~/.ssh/id_rsa.pub
```


#### Mac:

```
	pbcopy < ~/.ssh/id_rsa.pub
```

#### GNU/Linux (requires xclip):

```
	xclip -sel clip < ~/.ssh/id_rsa.pub
```


#### 把复制的内容粘贴到远程仓库添加设置ssh对应的位置。


