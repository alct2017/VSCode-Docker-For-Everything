FROM ubuntu

# 更换Ubuntu清华源，更新和升级
RUN sed -i 's/archive.ubuntu.com/mirrors.tuna.tsinghua.edu.cn/g' /etc/apt/sources.list; \ 
    sed -i 's/security.ubuntu.com/mirrors.tuna.tsinghua.edu.cn/g' /etc/apt/sources.list; \
    apt-get update; \
    apt-get upgrade -y
    
# 设置安装过程无交互
ENV DEBIAN_FRONTEND=noninteractive

# 安装所需texlive、tex中文包、xelatex、latexmk
RUN apt-get install -y texlive-full texlive-lang-chinese texlive-xetex latexmk