1.cp -a vimconfig ~/.vim
2.ln -s .vim/vimrc .vimrc
3.sudo apt install exuberant-ctags


zshell
1.sudo apt-get install zsh git wget
2.wget --no-check-certificate https://github.com/robbyrussell/oh-my-zsh/raw/master/tools/install.sh -O - | sh
3.chsh -s /bin/zsh
4.sudo reboot


oh-my-zsh有大量精美主题托管在项目中，
可以在此预览 https://github.com/robbyrussell/oh-my-zsh/wiki/themes，其中最拉风的一款agnoster。
配置过程记录如下。
为了能够显示诸如分支（branch）、闪电（这个符号应该指拿到root权限）、
错误(红色叉叉)、后台（一个齿轮）的各种符号，必须使用一个patch过的字体，
在ubuntu下默认是Ubuntu Mono，OS X下坐着配的是Menlo，
很多常见的等宽字体都打好了patch，当然也可以自己手动打patch。?
cd~/.fonts/ && git clone https://github.com/scotu/ubuntu-mono-powerline.git && cd~
在 ~/.zshrc 把主题设置为 agnoster
在 ~/.zshrc 设定 DEFAULT_USER 变量可以使得即使登陆在本机
(即非SSH到远程)时也能显示“user@hostname”

powerline front https://github.com/powerline/fonts


BundleInstall

DrawIt install
1,$vim DrawIt.vba.gz
2,:so %
3,:q

\di：开启DrawIt
\ds：关闭DrawIt
\b    矩形框
\e    椭圆
r <space>  删除
