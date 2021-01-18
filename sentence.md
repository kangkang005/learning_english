# File
+ This file is loaded by Spacemacs at startup. It must be stored in your home directory.

# Function
    (setq-default)
+ This function is called immediately after `dotspacemacs/init', before layer configuration.
    (defun dotspacemacs/user-env)
+ "Environment variables setup. This function defines the environment variables for your Emacs session. By default it calls `spacemacs/load-spacemacs-env' which loads the environment variables declared in `~/.spacemacs.env' or `~/.spacemacs.d/.spacemacs.env'. See the header of this file for more information."
    (defun dotspacemacs/user-init ())
+ "Initialization for user code: This function is called immediately after `dotspacemacs/init', before layer configuration. It is mostly for variables that should be set before packages are loaded. If you are unsure, try setting them in `dotspacemacs/user-config' first."
    (defun dotspacemacs/user-load ())
+ "Library to load while dumping. This function is called only while dumping Spacemacs configuration. You can `require' or `load' the libraries of your choice that will be included in the dump."
    (defun dotspacemacs/user-config ())
+ "Configuration for user code: This function is called at the very end of Spacemacs startup, after layer configuration. Put your configuration code here, except for variables that should be set before packages are loaded."
    (defun dotspacemacs/emacs-custom-settings ())
+ "Emacs custom settings. This is an auto-generated function, do not modify its content directly, use Emacs customize menu instead. This function is called at the very end of Spacemacs initialization."
    (custom-set-faces)
+ custom-set-faces was added by Custom. If you edit it by hand, you could mess it up, so be careful. Your init file should contain only one such instance. If there is more than one, they won't work right.


# Variable
    dotspacemacs-ask-for-lazy-installation t
+ If non-nil then Spacemacs will ask for confirmation before installing a layer lazily. (default t)
    dotspacemacs-configuration-layers '(markdown ivy)
+ List of configuration layers to load.
    dotspacemacs-configuration-layer-path '()
+ List of additional paths where to look for configuration layers. Paths must have a trailing slash (i.e. `~/.mycontribs/')
    dotspacemacs-emacs-dumper-dump-file (format "spacemacs-%s.pdmp" emacs-version)
+ Name of the Spacemacs dump file. This is the file will be created by the portable dumper in the cache directory under dumps sub-directory. To load it when starting Emacs add the parameter `--dump-file' when invoking Emacs 27.1 executable on the command line, for instance: ./emacs --dump-file=$HOME/.emacs.d/.cache/dumps/spacemacs-27.1.pdmp (default (format "spacemacs-%s.pdmp" emacs-version))
    dotspacemacs-elpa-timeout 5
+ Maximum allowed time in seconds to contact an ELPA repository. (default 5)
    dotspacemacs-verify-spacelpa-archives t
+ If non-nil then spacemacs will check for updates at startup
    dotspacemacs-editing-style 'vim
+ One of `vim', `emacs' or `hybrid'. `hybrid' is like `vim' except that `insert state' is replaced by the `hybrid state' with `emacs' key bindings. The value can also be a list with `:variables' keyword (similar to layers). Check the editing styles section of the documentation for details on available variables. (default 'vim)
    dotspacemacs-startup-buffer-show-version t
+ If non-nil show the version string in the Spacemacs buffer. 
    dotspacemacs-frozen-packages '()
+ A list of packages that cannot be updated.
    dotspacemacs-startup-buffer-responsive t
+ True if the home buffer should respond to resize events. (default t)
    dotspacemacs-scratch-buffer-persistent nil
+ If non-nil, *scratch* buffer will be persistent. Things you write down in *scratch* buffer will be saved and restored automatically.
    dotspacemacs-initial-scratch-message nil
+ Initial message in the scratch buffer, such as "Welcome to Spacemacs!" (default nil)
    dotspacemacs-themes '(spacemacs-dark spacemacs-light)
+ List of themes, the first of the list is loaded when spacemacs starts.
    dotspacemacs-mode-line-theme '(spacemacs :separator wave :separator-scale 1.5)
+ Set the theme for the Spaceline. Supported themes are `spacemacs', `all-the-icons', `custom', `doom', `vim-powerline' and `vanilla'. 
    dotspacemacs-colorize-cursor-according-to-state t
+ If non-nil the cursor color matches the state color in GUI Emacs.
    dotspacemacs-default-font '("Source Code Pro" :size 10.0 :weight normal :width normal)
+ Default font or prioritized list of fonts. The `:size' can be specified as a non-negative integer (pixel size), or a floating-point (point size). Point size is recommended, because it's device independent. (default 10.0)
    dotspacemacs-emacs-command-key "SPC"
+ The key used for Emacs commands `M-x' (after pressing on the leader key). (default "SPC")
    dotspacemacs-major-mode-leader-key ","
+ Major mode leader key is a shortcut key which is the equivalent of pressing `<leader> m`. Set it to `nil` to disable it. (default ",")
    dotspacemacs-major-mode-emacs-leader-key (if window-system "<M-return>" "C-M-m")
+ Major mode leader key accessible in `emacs state' and `insert state'. (default "C-M-m" for terminal mode, "<M-return>" for GUI mode). Thus M-RET should work as leader key in both GUI and terminal modes. C-M-m also should work in terminal mode, but not in GUI mode.
    dotspacemacs-distinguish-gui-tab nil
+ These variables control whether separate commands are bound in the GUI to the key pairs `C-i', `TAB' and `C-m', `RET'. Setting it to a non-nil value, allows for separate commands under `C-i' and TAB or `C-m' and `RET'.
    dotspacemacs-display-default-layout nil
+ If non-nil the default layout name is displayed in the mode-line.
    dotspacemacs-auto-save-file-location 'cache
+ Location where to auto-save files. Possible values are `original' to auto-save the file in-place, `cache' to auto-save the file to another file stored in the cache directory and `nil' to disable auto-saving. (default 'cache).
    dotspacemacs-enable-paste-transient-state nil
+ If non-nil, the paste transient-state is enabled. While enabled, after you paste something, pressing `C-j' and `C-k' several times cycles through the elements in the `kill-ring'. (default nil)
    dotspacemacs-switch-to-buffer-prefers-purpose nil
+ Control where `switch-to-buffer' displays the buffer. If nil, `switch-to-buffer' displays the buffer in the current window even if another same-purpose window is available. If non-nil, `switch-to-buffer' displays the buffer in a same-purpose window even if the buffer can be displayed in the current window. (default nil)
    dotspacemacs-fullscreen-at-startup nil
+ If non-nil the frame is fullscreen when Emacs starts up. (default nil)
    dotspacemacs-maximized-at-startup t
+ If non-nil the frame is maximized when Emacs starts up. Takes effect only if `dotspacemacs-fullscreen-at-startup' is nil.
    dotspacemacs-active-transparency 90
+ A value from the range (0..100), in increasing opacity, which describes the transparency level of a frame when it's active or selected. Transparency can be toggled through `toggle-transparency'. (default 90)
    dotspacemacs-smooth-scrolling t
+ If non-nil smooth scrolling (native-scrolling) is enabled. Smooth scrolling overrides the default behavior of Emacs which recenters point when it reaches the top or bottom of the screen. (default t)
    dotspacemacs-line-numbers t
+ Control line numbers activation. If set to `t', `relative' or `visual' then line numbers are enabled in all `prog-mode' and `text-mode' derivatives. If set to `relative', line numbers are relative. If set to `visual', line numbers are also relative, but lines are only visual lines are counted. 
    dotspacemacs-folding-method 'evil
+ Code folding method. Possible values are `evil', `origami' and `vimish'. (default 'evil)
    dotspacemacs-smart-closing-parenthesis nil
+ If non-nil pressing the closing parenthesis `)' key in insert mode passes over any automatically added closing parenthesis, bracket, quote, etc... This can be temporary disabled by pressing `C-q' before `)'. (default nil)
    dotspacemacs-enable-server nil
+ If non-nil, start an Emacs server if one is not already running.
    dotspacemacs-search-tools '("rg" "ag" "pt" "ack" "grep")
+ List of search tool executable names. Spacemacs uses the first installed tool of the list. Supported tools are `rg', `ag', `pt', `ack' and `grep'. (default '("rg" "ag" "pt" "ack" "grep"))
    dotspacemacs-zone-out-when-idle nil
+ Either nil or a number of seconds. If non-nil zone out after the specified number of seconds. (default nil)
    dotspacemacs-home-shorten-agenda-source nil
+ If nil the home buffer shows the full path of agenda items and todos. If non nil only the file name is shown.
