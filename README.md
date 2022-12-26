# Documentation how to setup Windows Prework
## Command for updating and upgrading apt-get. Actualiza para instalar comandos
sudo apt-get update -y && sudo apt-get upgrade -y
# Para instalar nodejs.
sudo apt install nodejs -y
# Para obtener la version de nodejs que tengo instalada.
node -v
# Para instalar manejador de paqueteria de nodejs (instalacion que permite utilizar javascripto en mi PC)
sudo apt install npm -y
# Para ejecutar un comando una sola vez sin tener que instalar desde internet un paquete de npm
npx package-example
# Example
npx create-react-app test