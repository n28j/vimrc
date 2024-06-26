# Clone the vundle repo
git clone git@github.com:VundleVim/Vundle.vim.git ~/.vim/bundle/Vundle.vim

# Move/Copy vimrc to ~/.vimrc
cp vimrc ~/.vimrc

# Clone YouCompleteMe
git clone git@github.com:ycm-core/YouCompleteMe ~/.vim/bundle/youcompleteme

# Install build tools
sudo dnf install make gcc-c++ cmake python3-devel -y

# Congifure ycm
cd ~/.vim/bundle/youcompletem
python3 install.py --clangd-completer

# Open vim and run the following command:
# :PluginInstall
