# tutorial
tutorial for dumemo

1.  installer Ubuntu

    først installer raspberrypi imager


    først søk up raspbarrypi imager så klikk den første linken eller klikk denne [raspbarry pi imager](https://www.raspberrypi.com/software/)

    laungh raspbarrypi imager and then but the SD-card into ur laptop

      on "choose device" choose raspbarrypi 4

      on "choose os" choose other general-purpoes OS then Ubuntu then the first one on the top

      on "choose storage" choose the only one that you can

    after its done installing place the SD-card back into the raspbarrypi

    do all the nesessary ubuntu installations


2.  update everything in your commandprompt (ctrl + alt + T)

    ```
    sudo apt update

    sudo apt upgrade
    ```
x


3.  installer firewall

    skriv in disse commandene in i commandprompt
    ```
    sudo apt install ufw

    sudo ufw enable

    sudo ufw allow ssh
    ```

4.  installer ssh server

    skriv in disse commandene in i commandprompt

    ```
    sudo apt install openssh-server

    sudo systemctl enable ssh
    
    sudo systemctl start ssh
    ```


5.  installer python, git and mariadb

    skriv in disse commandene in i commandprompt

    ```
    sudo apt install python3-pip
    
    sudo apt install git
    
    sudo apt install mariadb-server
    
    sudo mysql_secure_installation
    ```

6.  lage en ny bruker i mariadb

    logg in to mariadb using root
    ```
    sudo mariadb -u root
    ```

    make a new user
    ```
    CREATE USER 'username'@'localhost' IDENTIFIED BY 'password';
    ```

    give the user privileges
    ```
    GRANT ALL PRIVILEGES ON *.* TO 'username'@’localhost’
    ```

    update the privileges
    ```
    FLUSH PRIVILEGES;
    ```

7. 
