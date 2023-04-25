## Init Linux Config

    sudo apt-get update && sudo apt-get upgrade
    
##### Init config

    nano /etc/sudoers
    # nax ALL=(ALL) NOPASSWD:ALL

##### brave
    
https://brave.com/linux

##### sublime text

https://www.sublimetext.com/docs/linux_repositories.html

##### git

https://git-scm.com/download/linux

    apt-get install git && git --version

##### ssh keys

	$ ssh-keygen -t rsa -b 2048 -C "notebook linux"
	Enter file in which to save the key (/home/naxo/.ssh/id_rsa): /home/naxo/.ssh/id_ssh, , 

	# Copiar salida en [https://github.com/settings/keys] (https://github.com/settings/keys)
	cat /home/naxo/.ssh/id_ssh.pub

	# Agrega la llave ssh a tu pc 
	ssh-add /home/naxo/.ssh/id_ssh

##### nvm 
    curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.38.0/install.sh | bash
    source ~/.bashrc
    
##### pnpm
https://pnpm.io/installation#on-alpine-linux

### Atajos terminal
    # alt + 
    q subl
    w python3 /home/nax/.miConfig/launch-or-focus-brave.py
    m io.elementary.files
    e io.elementary.terminal
    x brave-browser https://github.com/naxo25/
    n brave-browser https://github.com/mediatique-press
    g python3 /home/nax/Documentos/configs/launch-or-focus-browser2.py
    a codium
    
##### Install jump para launch-or-focus
    alt + r -> io.elementary.terminal
    git clone https://github.com/mkropat/jumpapp.git
    cd jumpapp
    sudo apt install make
    sudo apt install wmctrl
    make && sudo make install

##### Code launch-or-focus

    # importing webbrowser python module
    import webbrowser
    import subprocess

    #Assigning URL to be opened
    url = "https://nacholabraweb.000webhostapp.com/"
    link = subprocess.run(["/home/nax/Documentos/configs/jumpapp/jumpapp", atajo])

    # Detectar si navegador esta abierto
    if (link.returncode == 0):
        print (link.returncode);
    else:
        #Open url in default browser
        webbrowser.open(url);

Atajos, "brave" "google-chrome" "smerge" "subl"

Esté codigo es para saltar entre aplicaciones usando atajos del teclado.
Made in naxo25


	
##### Config sublime text

    Console wrap
    Matherial Theme
    StandardFormat
    tailwind CSS Autocomplete
    Vue syntax highlight
    
##### Snippets for sublime

https://github.com/naxo25/Snippets-Copilot
