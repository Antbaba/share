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

```
	1. enter
	2. enter
	3. enter

```

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


#### 把复制的内容粘贴到远程仓库添加设置ssh对应的位置


#### git本地仓库生成

比如说在demo文件夹下生成本地仓库 => 在demo目录下生成.git隐藏文件夹目录 

```
	cd demo
	git init

```

#### 配置当前项目git用户名和邮箱

```
	git config user.name 'your name'
	git config user.email 'your email'
```

#### 可通过命令查看当前项目git config配置项

```
	git config --list
```

### 本地仓库项目推送到远程仓库

#### 添加远程仓库


```
	git remote add demo git@github.com:/**.git
```

#### 可通过命令查看添加的远程仓库

```
	git remote -v
```

#### 可通过命令推送到远程仓库

```
	git push demo master
```


```
	未完待续...
```