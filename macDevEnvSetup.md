# 开发环境搭建

## 一键安装

   打开并保存[mac](https://github.com/letotecn/meta/blob/master/mac)到本地，然后在你的终端里面运行
``` bash
 sh mac
```


## 详细步骤

### 安装 [homebrew](https://brew.sh/)

当你拿到你的Mac以后，Homebrew是必不可少的需要安装的软件之一，作为一款自由及开放源代码的软件包管理系统，使用 homebrew 可以大大简化 Mac OS X 系统上的软件安装过程哦。

复制以下代码到你的终端中运行

```bash
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
```

### 安装 git

当你安装好 homebrew 之后，接下来的一切就变得很简单了。首先使用 homebrew 安装git

在终端中运行
  ``` bash 
  brew install git 
  ``` 
即可，在完成git安装以后，你可以通过 
  ``` bash 
  git --version
  ``` 
命令来验证是否安装成功

### 安装 erlang

运行下面的脚本安装 erlang

``` bash 
brew install erlang
```

### 安装 [asdf](https://github.com/asdf-vm/asdf/blob/master/README.md)

  考虑到我们的项目可能依赖的elixir版本不同，我们可能需要安装 asdf, asdf是一个可扩展的版本管理器，支持Ruby，Node.js，Elixir，Erlang等 

- 首先克隆该仓库

  ```bash
  git clone https://github.com/asdf-vm/asdf.git ~/.asdf --branch v0.5.1
  ```

- 然后运行以下命令
  ```bash
  echo -e '\n. $HOME/.asdf/asdf.sh' >> ~/.bash_profile
  echo -e '\n. $HOME/.asdf/completions/asdf.bash' >> ~/.bash_profile
  ```

- 安装 elixir
  ``` bash
  asdf plugin-add elixir
  
  ```
  你可以使用一下命令查看你已经安装的 plugin
  ```bash
  asdf plugin-list
  ```
- 安装 nodejs
  ``` bash
  asdf plugin-add nodejs
  ```

### 安装Database MySQL & PostgreSQL

- 安装 mysql

  ``` bash
  brew install mysql
  ```

- 安装PostgreSQL

  ```postgresql
  brew install postgresql
  ```
  考虑到要跑我们的项目，最好在安装好PostgreSQL的时候创建角色,首先启动PostgreSQL
  ```bash
  brew services start postgresql
  ```
  然后运行
  ```bash
  createuser -sP postgres
  ```


