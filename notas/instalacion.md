# Instalación de AWX

# Paso 1... SOLO EN NUESTRO CASO:
Limpiar las imagenes de contenedor que nos da Amazon de clavo

>>> docker rmi $(docker images -q)

# Paso 2 es clonar el repo de AWX en la maquina
git clone -b 17.1.0 https://github.com/ansible/awx.git

# Paso 3. Instalar ansible
sudo apt-add-repository --yes --update ppa:ansible/ansible
sudo apt install ansible -y
ansible-playbook --version

# Paso 4. En el fichero de inventario hay que cambiar varias cosas...
Tenemos que poner un secret-key
sudo apt install pwgen -y
pwgen -N 1 -s 30

# Dependencias
sudo apt install docker-compose -y
sudo apt install software-properties-common

sudo -H pip3 install --upgrade setuptools
python3 -m pip install -U pip
sudo -H pip3 install docker
sudo pip3 install docker-compose
sudo -H pip install docker
sudo pip install docker-compose

# Instalacion awx
cd awx/installer
ansible-playbook -i inventory install.yml