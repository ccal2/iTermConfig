# My iTerm2 configuration

I follwed [this](https://gist.github.com/kevin-smets/8568070) and ended up with this:

![Screenshot](/Screenshot.png)

I also installed the `colorls` plugin to have icons at file listings:

![colorls](/colorls.png)


## Installation

- [iTerm2](https://www.iterm2.com)

        brew install --cask iterm2

- [Oh My Zsh](https://ohmyz.sh)

        sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"

- [Powerlevel10k](https://github.com/romkatv/powerlevel10k)

        git clone https://github.com/romkatv/powerlevel10k.git $ZSH_CUSTOM/themes/powerlevel10k

    - My style configuration:
      - (3)  Rainbow.
      - (1)  Unicode.
      - (1)  No.
      - (1)  Angled.
      - (1)  Sharp.
      - (3)  Sharp.
      - (2)  Two lines.
      - (2)  Dotted.
      - (1)  No frame.
      - (3)  Dark.
      - (2)  Sparse.
      - (2)  Many icons.
      - (1)  Concise.
      - (n)  No.
      - (2)  Quiet.

- [Auto suggestions](https://github.com/zsh-users/zsh-autosuggestions)

        git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions

- [Syntax highlighting](https://github.com/zsh-users/zsh-syntax-highlighting)

        brew install zsh-syntax-highlighting

- [Colorls](https://github.com/athityakumar/colorls)

        gem install colorls


## Files placement

- `.zprofile`, `.zshrc` and the `.config` folder go in the home diretory.

  - on `.zshrc`, update line 12 with your information
  
        export ZSH="/Users/{username}/.oh-my-zsh"

  - The file `dark_colors.yaml` at `.config/colorls` is used to override the default colors for `colorls` on dark mode, as explained [here](https://github.com/athityakumar/colorls) on the topic `Custom configurations`

- `Default.json` is the iTerm2 Profile. To import it, go to iTerm2 > Preferences.

    ![iTerm2 Preferences](/iTerm2_Preferences.png)
