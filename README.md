# Documentation how to setup Windows Prework
## Command for updating and upgrading apt-get. Actualiza para instalar comandos
sudo apt-get update -y && sudo apt-get upgrade -y
### Para instalar nodejs.
sudo apt install nodejs -y
### Para obtener la version de nodejs que tengo instalada.
node -v
### Para instalar manejador de paqueteria de nodejs (instalacion que permite utilizar javascripto en mi PC)
sudo apt install npm -y
### Para ejecutar un comando una sola vez sin tener que instalar desde internet un paquete de npm
npx package-example
### Example. Creates a react project named test in current directory
npx create-react-app test
### Para instalar Git
sudo apt install git
### Para verificat version de git
git --version

# Para crear llave ssh y configurarla
## Para create llave ssh mediante keygenerator
ssh-keygen -t -rsa -b 4096 -C "yourgithubpassword"
## Para evaluar ssh agent
eval "$(ssh-agent -s)"
## Para copiar id de llave public (NO NECESARIAMENTE HACERLO) PRIMERO LEER https://www.ssh.com/ssh/copy-id
ssh-copy-id armystrategie@gmail.com
## go to directory where you have ssh key
cd ~/.ssh

# Para inicializar proyecto en git (github)
## Inicializa git en proyecto actual
git init
## Agrega archivos a update de version
git add -A
git add .
## Haces commit de cambio de version con nombre de commit
git commit -m "First commit name"
## Creas rama principal
git branch -M main
## Agregas repositorio remoto en github (URL)
git remote add origin git@github.com:Armychess/proyectoDemoCursoPrework.git.
## Haces push y envias cambios de commit a github
git push -u origin main

## Si te equivocaste agregando https como repo remoto, arreglalo con
git remote set-url origin git@github.com:Armychess/proyectoDemoCursoPrework.git