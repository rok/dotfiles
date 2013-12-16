Dotfiles
========

1. Set up:

   ```
   curl -L 'https://github.com/rok/dotfiles/raw/master/vimrc' > ~/.vimrc
   git clone https://github.com/gmarik/vundle.git ~/.vim/bundle/vundle
   ```

2. Install configured bundles:

   Launch `vim`, run `:BundleInstall`

3. Compile YouCompleteMe
   ```
   cd ~/.vim/bundle/YouCompleteMe
   sudo apt-get install CMake (if necessary)
   ./install.sh --clang-completer
   ```

4. Compile Command-T
   ```
   sudo apt-get install ruby-dev
   cd ~/.vim/bundle/Command-T/ruby/command-t/
   ruby extconf.rb
   make
   ```

5. Install Latex-suite, laguage support and eps2pdf
   ```
   sudo apt-get install vim-latexsuite texlive-lang-european texlive-font-utils
   sudo vim-addons -w install latex-suite
   ```
