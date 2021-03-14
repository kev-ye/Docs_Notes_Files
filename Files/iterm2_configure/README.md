# My iterm2 configuration

## Configuration

### Step 1 : Installation of fonts
    
I use homebrew for almost installations

`Install nerd-fonts` 

    - brew tap homebrew/cask-fonts  
    - brew cask install font-hack-nerd-font

`Add fonts`  

    - iTerm2 -> Preferences -> Profiles -> Text -> Font  
    - Use a different font for non-ASCII text  
    - Non-ASCII Font  
    - Hack Nerd Font

### Step 2 : Installation of oh_my_zsh

`Install Oh_My_Zsh`  

    sh -c "$(curl -fsSL https://raw.github.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"

### Step 3 : Add powerlevel10k themes

`Install Powerlevel10k Themes`  

    git clone --depth=1 https://github.com/romkatv/powerlevel10k.git ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/themes/powerlevel10k

`Change themes basics configures`  
    
    - vim ~/.zshrc
    - ZSH_THEME="powerlevel10k/powerlevel10k"
    - source ~/.zshrc

`Auto configure`  

    p10k configure

## Utils_plugins

`autojump : j somedir`  

    brew install autojump

`zsh-syntax-highlighting`  

    - git clone https://github.com/zsh-users/zsh-syntax-highlighting.git ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-syntax-highlighting

    - vim ~/.zshrc : plugins=(zsh-syntax-highlighting)

`zsh-autosuggestions`

    - git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions

    - vim ~/.zshrc : plugins=(zsh-autosuggestions)
