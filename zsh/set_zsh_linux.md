#!/bin/bash
#clear environment
rm -rf ~/.oh-my-zsh

# install zsh
apt install zsh
# install oh my zsh
#sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"
curl -L http://install.ohmyz.sh | sh

# install auto suggestions
git clone https://github.com/zsh-users/zsh-autosuggestions ~/.zsh/zsh-autosuggestions
echo "source ~/.zsh/zsh-autosuggestions/zsh-autosuggestions.zsh" >> ~/.zshrc

# install completion
git clone https://github.com/zsh-users/zsh-completions ~/.oh-my-zsh/custom/plugins/zsh-completions
#echo 'plugins=(zsh-completions)' >> ~/.zshrc
echo 'autoload -U compinit && compinit' >> ~/.zshrc

#install powerlevel9k
git clone https://github.com/bhilburn/powerlevel9k.git ~/.oh-my-zsh/custom/themes/powerlevel9k
echo 'ZSH_THEME="powerlevel9k/powerlevel9k"' >> ~/.zshrc

#source ~/.zshrc
