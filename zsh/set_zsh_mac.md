brew install zsh zsh-completions

# install oh-my-zsh

sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"

#install powerlevel9k
git clone https://github.com/bhilburn/powerlevel9k.git
echo 'source ~/powerlevel9k/powerlevel9k.zsh-theme' >> ~/.zshrc

#install auto-suggestions
brew install zsh-autosuggestions
echo 'source /usr/local/share/zsh-autosuggestions/zsh-autosuggestions.zsh' >> ~/.zshrc


#install syntax-highlighting
brew install zsh-syntax-highlighting
echo 'source /usr/local/share/zsh-syntax-highlighting/zsh-syntax-highlighting.zsh' >> ~/.zshrc

# install Nerd font and configure it in iTerm2
cd ~/Library/Fonts && curl -fLo "Droid Sans Mono for Powerline Nerd Font Complete.otf" https://github.com/ryanoasis/nerd-fonts/raw/master/patched-fonts/DroidSansMono/complete/Droid%20Sans%20Mono%20Nerd%20Font%20Complete.otf

# iTerm -> Preferences -> Profiles -> Text -> Font -> Change Font -------> Change font to Droid Sans Mono Nerd Font

