# guia-de-instalacion-bettercap
esta es una guia de installacion de bettercap en linux en mi caso es linux mint y en este perfil de github dejare mas guias de instalacion ya que estoy creando mi version de linux mint para pentesting


🛠️ Bettercap Installation Guide (Linux)

Primero, actualiza tu sistema e instala las dependencias requeridas:

sudo apt update
sudo apt install golang-go git build-essential libpcap-dev libusb-1.0-0-dev libnetfilter-queue-dev
🔧 Go Environment Configuration

Configura tu entorno Go agregando las siguientes líneas a tu archivo ~/.bashrc:

export GOPATH=$HOME/go
export PATH=$PATH:$GOPATH/bin:/usr/local/go/bin

Aplica los cambios ejecutando:

source ~/.bashrc
🏗️ Build & Install

Clona el repositorio oficial, compila el binario e instálalo a nivel sistema:

git clone https://github.com/bettercap/bettercap.git
cd bettercap
sudo make build
sudo make install
🚀 Usage

Una vez instalado, puedes ejecutar Bettercap con:

sudo bettercap
🛠️ Troubleshooting

Verifica que Go esté correctamente instalado:

go version
Asegúrate de que $GOPATH/bin esté incluido en tu variable PATH
Si hay errores en la compilación, revisa que todas las dependencias estén instaladas correctamente
Ejecuta los comandos con permisos adecuados (sudo)
📄 License

Para más información sobre la licencia, consulta el repositorio oficial de Bettercap:
https://github.com/bettercap/bettercap
