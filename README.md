# My Terminal Config
<p align="center">
	<img src="https://s3.amazonaws.com/ohmyzsh/oh-my-zsh-logo.png" alt="Oh My Zsh" width="337" height="208">
	<img src="https://raw.githubusercontent.com/jandedobbeleer/oh-my-posh/main/website/static/img/logo.png" alt="Oh My Posh" width="337" height="208">
</p>
## Install zsh

```
sudo yum install zsh-autosuggestions zsh-syntax-highlighting zsh lsd
```

## Install Oh my ZSH

```
sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```

## Install Oh my Posh

```
curl -s https://ohmyposh.dev/install.sh | bash -s
```

## Install font

Oh My Posh has a CLI to help you select and install a [Nerd Font](https://www.nerdfonts.com/):
```
oh-my-posh font install adwaitamono
```

## Install plugins.
 - autosuggesions plugin
 
```
git clone https://github.com/zsh-users/zsh-autosuggestions.git $ZSH_CUSTOM/plugins/zsh-autosuggestions
```
	
 - zsh-syntax-highlighting plugin
 
```
git clone https://github.com/zsh-users/zsh-syntax-highlighting.git $ZSH_CUSTOM/plugins/zsh-syntax-highlighting
```
	
 - zsh-fast-syntax-highlighting plugin
 
```
git clone https://github.com/zdharma-continuum/fast-syntax-highlighting.git ${ZSH_CUSTOM:-$HOME/.oh-my-zsh/custom}/plugins/fast-syntax-highlighting
```
	
 - zsh-autocomplete plugin
	
```
git clone --depth 1 -- https://github.com/marlonrichert/zsh-autocomplete.git $ZSH_CUSTOM/plugins/zsh-autocomplete
```

- autoenv

```
curl -#fLo- 'https://raw.githubusercontent.com/hyperupcall/autoenv/main/scripts/install.sh' | sh
```

## Download and replace .zshrc

```
curl --output ~/.zshrc "https://raw.githubusercontent.com/JelonGames/My-Terminal-Config/refs/heads/main/.zshrc"
```

If you are using a system other than the REHL distribution, remove the yum plugin and change aliases.
 - open file ./~zshrc
 - Find the line which says 
	 `plugins=(git zsh-autosuggestions zsh-syntax-highlighting fast-syntax-highlighting zsh-autocomplete autoenv yum)`.
 - Delete yum
 - At the very bottom of the file, you will find all aliases to be changed.

## Refrences

 - [Oh my ZSH](https://github.com/ohmyzsh/ohmyzsh)
 - [zsh-autosuggestions](https://github.com/zsh-users/zsh-autosuggestions)
 - [zsh-syntax-highlighting](https://github.com/zsh-users/zsh-syntax-highlighting)
 - [zsh-fast-syntax-highlighting](https://github.com/zdharma/fast-syntax-highlighting)
 - [zsh-autocomplete](https://github.com/marlonrichert/zsh-autocomplete)
 - [autoenv](https://github.com/hyperupcall/autoenv)
 - [Oh my Posh](https://ohmyposh.dev/)
 - [Nerd Font](https://www.nerdfonts.com/)
 - [LSD](https://github.com/lsd-rs/lsd)