## 1.Velvet

#### 1.1下载并安装

Velvet 是一个老牌的基因组测序数据拼接软件。Velvet最新版本是1.2.10，可以访问 [官方网站](https://www.ebi.ac.uk/~zerbino/velvet/) 下载源代码包，也可以通过克隆 [软件仓库](https://github.com/dzerbino/velvet.git) 的方式获得最新的源代码。

**下载源代码**

普通用户可以下载源代码包自行编译获得软件。

```
$ cd /tmp
$ wget https://www.ebi.ac.uk/~zerbino/velvet/velvet_1.2.10.tgz
$ tar xvf -C velvet velvet_1.2.10.tgz
```

**克隆代码仓库**

如果在软件运行中遇到问题，想试用最新版代码，或是有能力提交issues，或者想改进软件参与开源代码编写的可以选择克隆代码库的方式。

```
$ cd ~/tmp
~/tmp$ git clone https://github.com/dzerbino/velvet.git
```

**编译安装**

make可以进行编译，有几个编译参数可以选择，分别是MAXKMERLENGTH, DIRECTORY

```
$ cd velvet
$ make MAXKMERLENGTH=127
$ sudo cp velveth velvetg /usr/local/sbin
```

#### 1.2 拼接基因组

首先来了解一下velvet的组成。

```
$ velvet
```