# linux
Comandos e procedimentos adotados no dia-a-dia do uso de linux.

# ativar wifi após a instalação
1) conectar cabo de rede ao computador
2) ir em Configurações do sistema > Programas e atualizações > Drivers adicionais (instalar drivers)

# instalação do antivírus eset nod32
1) download via site para 64-bit
2) abrir terminal
3) sudo dpkg --add-architecture i386
4) sudo apt update
5) sudo apt install libc6:i386
6) chmod +x <nome-do-arquivo-baixado>.linux
7) ./<nome-do-arquivo-baixado>.linux (necessário ir até diretório de download)

# formas de instalar programas (pacotes)
1) via repositórios oficiais usando apt-get
2) via download do pacote usando dpkg

# comandos para instalação de pacotes
1) se o pacote já estiver nos repositórios oficiais:
  1.1) sudo apt-get install <pacote>
2) se for necessário adicionar um novo repositório:
  2.1) sudo add-apt-repository <repositório>
  2.2) sudo apt-get update
  2.3) sudo apt-get install <pacote>
3) pacote .deb
  3.1) sudo dpkg -i <pacote>.deb
  3.2) sudo apt-get -f install (corrige problemas ocorridos durante a instalação)
  
# instalação de temas

tema:
1) download do tema
2) conceder permissão de escrita: sudo chmod +x theme-xxx.deb 
3) instalar o tema: sudo dpkg -i theme-xxx.deb 
4) instalar dependências: sudo apt-get -f install 

ou 

1) sudo add-apt-repository ppa:noobslab/themes
2) sudo apt-get update
3) sudo apt-get install arc-theme

ícones:
1) sudo add-apt-repository ppa:moka/daily
2) sudo apt-get update
3) sudo apt-get install moka-icon-theme faba-icon-theme faba-mono-icons

ou 

1) sudo add-apt-repository ppa:noobslab/icons
2) sudo apt-get update
3) sudo apt-get install arc-icons

ferramenta de configuração:   
1) sudo apt install unity-tweak-tool

# instalação do Git
1) sudo apt-get update
2) sudo apt-get install git
3) git config --global user.name "Felipe Thomas"
4) git config --global user.email "felipecejug@gmail.com"
