# 使用该配置
## 1、安装zsh
```bash
sudo apt install zsh
```

## 2、oh my zsh
安装：
```bash
sh -c "$(wget https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh -O -)"
```

## 3、将我的配置覆盖你的默认配置

```bash
git clone https://github.com/xjintong/zshconfig.git

cd zshconfig

cp .zshrc ~/

```

## 4、安装Plugins
- powerlevel10k主题

```bash
git clone --depth=1 https://github.com/romkatv/powerlevel10k.git ${ZSH_CUSTOM:-$HOME/.oh-my-zsh/custom}/themes/powerlevel10k
```

- 代码高亮，终端输入正确命令时候是绿色的，不正确的是红色的。 
安装：
```bash
git clone https://github.com/zsh-users/zsh-syntax-highlighting.git ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-syntax-highlighting
```

[https://github.com/zsh-users/zsh-syntax-highlighting](https://github.com/zsh-users/zsh-syntax-highlighting)

- 代码提示，终端输入命令的部分字母时候，会提示后面的字母。
安装：
```bash
git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions
````

[https://github.com/zsh-users/zsh-autosuggestions](https://github.com/zsh-users/zsh-autosuggestions)

- autojump
```
sudo apt install autojump
```

## 5、重新加载zsh配置

```bash
exec zsh
```
