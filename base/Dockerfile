FROM ubuntu:22.04
RUN set -e \
    && set -x \
    && apt update -y \
    && apt install git -y \
    && apt install curl wget -y \
    && apt install default-jdk openjdk-8-jdk openjdk-17-jdk -y \
    && apt install maven -y \
    && apt install zsh -y \
    && chsh -s /usr/bin/zsh \
    && sh -c "$(curl -fsSL https://raw.github.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"

RUN set -e \
    && set -x \
    && git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions \
    && git clone https://github.com/zsh-users/zsh-syntax-highlighting.git ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-syntax-highlighting
    