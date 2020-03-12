# ConfigFiles
My Configuration Files

# iTerm2 Customization

## Install Homebrew
Paste url in terminal if you don't have Homebrew already installed 

    /usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"


## Install iterm2

    brew cask install iterm2
 
# Oh My Zsh 

## Install with curl
    
    sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"
    
    
## Powerlevel9k / Powerlevel10k

    git clone https://github.com/romkatv/powerlevel10k.git $ZSH_CUSTOM/themes/powerlevel10k

Then edit your `~/.zshrc` and set `ZSH_THEME="powerlevel10k/powerlevel10k"`.

## Install a patched font
First Install Source Code Pro 
- [Source Code Pro + Font Awesome](https://github.com/Falkor/dotfiles/blob/master/fonts/SourceCodePro%2BPowerline%2BAwesome%2BRegular.ttf), this one is needed if you want the icons from Font Awesome as shown in the screenshot for Powerlevel10k.
Open the downloaded font and press "Install Font".

After go to:
- [Others @ powerline fonts](https://github.com/powerline/fonts)
    
Copy and paste these commands to your terminal. Comments are fine too.

    # clone
    git clone https://github.com/powerline/fonts.git --depth=1
    # install
    cd fonts
    ./install.sh
    # clean-up a bit
    cd ..
    rm -rf fonts

Set Source Code Pro for Powerline in iTerm2 (iTerm → Preferences → Profiles → Text → Change Font)
Set in Solarized Dark  (iTerm → Preferences → Profiles → Text → Change Color Presets)


Restart iTerm2 for all changes to take effect.

After completing the wizard and choosing the style you wantm your iTerm2 should look similar to this:

![Screenshot 2019-12-06 at 12 21 52 PM](https://user-images.githubusercontent.com/49213748/70317438-6d4fed80-1826-11ea-8c98-3c652cdcb2c4.png)

To enable shortcuts for navigation in iTerm2 go to:

Go to iTerm Preferences → Profiles, select your profile, then the Keys tab. Find ⌥← and ⌥→ and set them to send escape sequence b and send escape sequence f respectively.

Go to iTerm Preferences → Keys Find ←⌘ and ⌘→ set them to send hex code 0x01 and send hex code 0x05 respectively.Also add if it doesn't exist ⌘ + backspace to send hex code 0x15.

