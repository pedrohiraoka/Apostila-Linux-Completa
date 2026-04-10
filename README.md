# Apostila-Linux-Completa

Apostila Completa de Linux: Do Iniciante ao Profissional Certificado

Baseado em "Linux - A Bíblia", 8ª Edição, de Christopher Negus
Sumário

Parte I: Começando com o Linux

    Capítulo 1: O que é Linux e Por que Usá-lo?

    Capítulo 2: Escolhendo e Usando um Ambiente de Desktop (GNOME)

Parte II: Tornando-se um Usuário Avançado do Linux (Power User)

    Capítulo 3: Dominando o Shell de Linha de Comando (Bash)

    Capítulo 4: Navegando e Gerenciando o Sistema de Arquivos

    Capítulo 5: Trabalhando com Arquivos de Texto e Editores (Vim)

    Capítulo 6: Gerenciando Processos em Execução

    Capítulo 7: Automatizando Tarefas com Scripts de Shell

Parte III: Tornando-se um Administrador de Sistema Linux

    Capítulo 8: Fundamentos da Administração de Sistemas e o Usuário root

    Capítulo 9: Instalando o Linux (Fedora/RHEL)

    Capítulo 10: Gerenciando Softwares e Pacotes (RPM/YUM)

    Capítulo 11: Gerenciando Usuários e Grupos

    Capítulo 12: Gerenciando Discos, Partições e LVM

Parte IV: Tornando-se um Administrador de Servidores Linux

    Capítulo 13: Conceitos de Administração de Servidores e Acesso Remoto (SSH)

    Capítulo 14: Configuração e Administração de Redes

    Capítulo 15: Controlando Serviços (systemd e SysVinit)

    Capítulo 16: Servidor de Impressão (CUPS)

    Capítulo 17: Servidor Web (Apache HTTPD)

    Capítulo 18: Servidor FTP (vsftpd)

    Capítulo 19: Servidor de Arquivos Windows (Samba)

    Capítulo 20: Servidor de Arquivos de Rede (NFS)

    Capítulo 21: Solução de Problemas no Linux

Parte V: Segurança no Linux

    Capítulo 22: Fundamentos de Segurança (Contas, Senhas, Permissões)

    Capítulo 23: Segurança Avançada (Criptografia e PAM)

    Capítulo 24: SELinux (Security-Enhanced Linux)

    Capítulo 25: Segurança de Rede (Firewall iptables)

Parte I: Começando com o Linux
Capítulo 1: O que é Linux e Por que Usá-lo?

1.1. O que é Linux?
Linux é o kernel (núcleo) de um sistema operacional. Um sistema operacional completo, muitas vezes chamado de "distribuição Linux", é composto pelo kernel Linux mais uma vasta coleção de ferramentas e aplicativos (principalmente do projeto GNU), razão pela qual alguns o chamam de GNU/Linux.

Funções Principais do Kernel Linux:

    Gerenciar Processos: Controla quais programas são executados, por quanto tempo e com qual prioridade.

    Gerenciar Memória: Aloca RAM e gerencia o espaço de troca (swap).

    Gerenciar Hardware: Carrega drivers (módulos) para se comunicar com discos, placas de rede, etc.

    Sistemas de Arquivos: Organiza e controla o acesso a arquivos e diretórios.

    Segurança: Gerencia usuários, permissões e autenticação.

1.2. Por que o Linux é Especial? (Código Aberto)
Linux é distribuído sob a licença GPL (GNU General Public License), que garante as "quatro liberdades":

    Executar o programa para qualquer propósito.

    Estudar como o programa funciona e adaptá-lo às suas necessidades (acesso ao código-fonte).

    Redistribuir cópias.

    Aperfeiçoar o programa e liberar os seus aperfeiçoamentos (modificar o código-fonte).

1.3. Distribuições Linux Populares
Uma distribuição é o kernel Linux + utilitários + gerenciador de pacotes + filosofia da comunidade.
Família	Distribuições Principais	Foco Principal
Red Hat	Red Hat Enterprise Linux (RHEL)	Corporativo: Estabilidade, suporte pago e certificações (RHCSA/RHCE).
	Fedora	Inovação: Tecnologias de ponta, "laboratório" da Red Hat.
	CentOS / Rocky Linux	Servidores: Versão gratuita e compatível com o RHEL.
Debian	Debian GNU/Linux	Estabilidade e Software Livre: Base sólida e princípios rígidos.
	Ubuntu	Desktop e Facilidade: Interface amigável, ótima para iniciantes.
Capítulo 2: Escolhendo e Usando um Ambiente de Desktop (GNOME)

2.1. Conceitos Básicos do Desktop Linux
O ambiente gráfico do Linux é construído sobre o X Window System (X11), que atua como uma base de rede, permitindo que aplicativos rodem em uma máquina e sejam exibidos em outra. Sobre o X11, são construídos os Gerenciadores de Janelas e os Ambientes de Desktop completos.

2.2. GNOME (Padrão do Fedora/RHEL)
O GNOME é o ambiente de desktop mais popular no mundo corporativo Linux.

    GNOME 3 (Fedora): Interface moderna, focada em atividades (Activities), uso de espaços de trabalho dinâmicos e uma barra superior (Dash). Navegação fluida com a tecla Windows (Super).

    GNOME 2 (RHEL 6 e anteriores): Layout tradicional com dois painéis (superior e inferior), menus Applications, Places e System.

2.3. Ferramentas e Aplicativos Essenciais do GNOME

    Nautilus (Arquivos): Gerenciador de arquivos para navegar, copiar, mover e deletar arquivos.

    Configurações do Sistema: Painel central para configurar rede, impressão, usuários, aparência e mídia removível.

    Software (PackageKit): Loja de aplicativos gráfica para instalar e remover programas.

Parte II: Tornando-se um Usuário Avançado do Linux (Power User)
Capítulo 3: Dominando o Shell de Linha de Comando (Bash)

O shell é o interpretador de comandos. É a ferramenta mais poderosa para interagir com o Linux. O shell padrão é o Bash (Bourne Again Shell).

3.1. Comandos Básicos
Comando	Função	Exemplo
pwd	Mostra o diretório atual ("Print Working Directory")	$ pwd
ls	Lista arquivos e diretórios	$ ls -l
cd	Muda de diretório ("Change Directory")	$ cd /etc
cat	Exibe o conteúdo de um arquivo	$ cat /etc/passwd
echo	Exibe uma mensagem na tela	$ echo "Olá"
man	Exibe o manual de um comando	$ man ls

3.2. Atalhos e Recursos do Bash

    Histórico: Use as setas ↑ e ↓ para navegar pelos comandos anteriores. Ctrl+R para busca reversa.

    Autocompletar: Pressione Tab para completar comandos, nomes de arquivos ou diretórios automaticamente.

    Aliases: Crie apelidos para comandos longos. Ex: alias ll='ls -l'

    Redirecionamento (>, >>, <): Envia a saída de um comando para um arquivo ou recebe a entrada de um arquivo.

        ls > lista.txt (Cria/sobrescreve um arquivo)

        ls >> lista.txt (Adiciona ao final do arquivo)

    Pipes (|): Conecta a saída de um comando diretamente na entrada de outro.

        ls -l | grep "txt" (Lista arquivos e filtra apenas os que contêm "txt")

    Variáveis de Ambiente: Armazenam informações do sistema. Ex: $HOME, $PATH, $USER.

Capítulo 4: Navegando e Gerenciando o Sistema de Arquivos

4.1. A Hierarquia do Sistema de Arquivos (FHS)
Tudo no Linux é um arquivo, organizado a partir da raiz (/).
Diretório	Conteúdo Principal
/bin	Comandos essenciais para todos os usuários (ex: ls, cp, cat).
/boot	Arquivos necessários para iniciar o sistema (kernel, GRUB).
/dev	Arquivos que representam dispositivos de hardware (ex: /dev/sda para o disco rígido).
/etc	Arquivos de configuração do sistema. O local mais importante para um administrador.
/home	Diretórios pessoais dos usuários.
/root	Diretório pessoal do superusuário (root).
/tmp	Arquivos temporários (apagados na reinicialização).
/usr	Aplicativos, bibliotecas e documentação para usuários.
/var	Dados variáveis, como logs do sistema (/var/log), filas de e-mail e bancos de dados.

4.2. Permissões de Arquivos
Cada arquivo tem três conjuntos de permissões: para o Usuário (u), para o Grupo (g) e para Outros (o).

    r (Read - Leitura) = 4

    w (Write - Escrita) = 2

    x (eXecute - Execução) = 1

Exemplo: -rwxr-xr--

    -: Arquivo comum (d para diretório, l para link).

    rwx: Dono pode Ler, Escrever e Executar (4+2+1 = 7).

    r-x: Grupo pode Ler e Executar (4+0+1 = 5).

    r--: Outros podem apenas Ler (4+0+0 = 4).
    Permissão final: 754

Comandos-chave:

    chmod: Altera permissões (ex: chmod 755 arquivo ou chmod u+x arquivo).

    chown: Altera o dono e o grupo (ex: chown joe:devs arquivo).

Capítulo 5: Trabalhando com Arquivos de Texto e Editores (Vim)

Arquivos de configuração no Linux são, em sua maioria, texto puro. Saber editá-los é uma habilidade fundamental.

5.1. O Editor Vim
O Vim (Vi Improved) é poderoso, mas tem uma curva de aprendizado íngreme. Ele opera em dois modos principais:

    Modo de Comando: Padrão ao abrir. As teclas executam ações (navegar, deletar, copiar).

    Modo de Inserção: Para digitar texto. Pressione i, a, o para entrar.

Comandos Essenciais do Vim (no Modo de Comando):

    i: Entra no modo de inserção.

    ESC: Sai do modo de inserção e volta ao modo de comando.

    :w: Salva o arquivo.

    :q: Sai do Vim.

    :wq ou ZZ: Salva e sai.

    :q!: Sai sem salvar.

    dd: Deleta uma linha inteira.

    yy: Copia (yank) uma linha.

    p: Cola o texto copiado.

    /palavra: Procura por "palavra".

5.2. Buscando Arquivos e Conteúdo

    find: Pesquisa arquivos no sistema de arquivos em tempo real. Muito flexível.

        find /home -name "*.txt" (Procura por arquivos .txt em /home)

        find / -size +100M (Procura arquivos maiores que 100MB)

    grep: Pesquisa por texto dentro de arquivos.

        grep "erro" /var/log/messages (Procura a palavra "erro" no arquivo de log).

        ps aux | grep firefox (Filtra a saída do comando ps para mostrar apenas processos do Firefox).

Capítulo 6: Gerenciando Processos em Execução

Um processo é um programa em execução. O Linux é multitarefa, gerenciando centenas de processos ao mesmo tempo.

    ps: Exibe uma lista estática dos processos.

        ps aux: Mostra todos os processos do sistema, com detalhes.

    top: Exibe uma lista dinâmica e em tempo real dos processos, ordenados por uso de CPU.

        Pressione M para ordenar por uso de memória.

        Pressione q para sair.

    Primeiro e Segundo Plano:

        comando &: Executa um comando diretamente em segundo plano.

        Ctrl+Z: Pausa um processo em primeiro plano.

        bg: Envia o processo pausado para o segundo plano.

        fg: Traz um processo de volta para o primeiro plano.

    kill: Envia um sinal para um processo (geralmente para encerrá-lo).

        kill PID: Envia o sinal SIGTERM (15) para encerrar de forma segura.

        kill -9 PID: Envia o sinal SIGKILL (9) para forçar o encerramento imediato.

        killall nome_do_processo: Encerra todos os processos com aquele nome.

Capítulo 7: Automatizando Tarefas com Scripts de Shell

Scripts são arquivos de texto contendo uma sequência de comandos que podem ser executados como um único programa.

Estrutura Básica de um Script (meu_script.sh):
bash

#!/bin/bash
# Este é um comentário. Define que o interpretador é o bash.

echo "Olá, mundo!"
echo "A data de hoje é $(date)"

Para executar: chmod +x meu_script.sh (torna executável) e depois ./meu_script.sh.

Elementos de Programação:

    Variáveis: NOME="João" (uso: echo $NOME).

    Condicionais (if):
    bash

    if [ $1 == "sim" ]; then
        echo "Você disse sim!"
    else
        echo "Você não disse sim."
    fi

    Loops (for):
    bash

    for ARQUIVO in *.txt; do
        echo "Processando $ARQUIVO"
    done

Parte III: Tornando-se um Administrador de Sistema Linux
Capítulo 8: Fundamentos da Administração de Sistemas e o Usuário root

O usuário root (UID 0) é o superusuário, com poderes totais sobre o sistema. Nunca use o sistema logado como root para tarefas cotidianas.

8.1. Obtendo Privilégios Administrativos

    su -: Abre um shell como root. Requer a senha do root.

    sudo: Permite que um usuário comum execute comandos específicos com privilégios de root. Mais seguro e auditável. Requer configuração no arquivo /etc/sudoers.

8.2. Principais Responsabilidades do Administrador

    Gerenciar Usuários e Grupos: (useradd, usermod, userdel, groupadd).

    Gerenciar Software: Instalar, atualizar e remover pacotes (YUM/DNF).

    Gerenciar Serviços: Iniciar, parar e habilitar serviços (systemctl).

    Monitorar o Sistema: Verificar logs (/var/log), uso de disco (df), memória (free).

    Configurar Redes e Firewall: Definir endereços IP, rotas e regras de segurança.

    Realizar Backups: Proteger os dados do sistema.

Capítulo 9: Instalando o Linux (Fedora/RHEL)

O instalador do Fedora/RHEL chama-se Anaconda. Ele oferece modos gráfico e texto.

    Particionamento: É a etapa mais crítica. Pode ser automático ou manual. Esquemas comuns incluem partições separadas para /, /boot, /home e swap. O LVM (Logical Volume Manager) é altamente recomendado por sua flexibilidade.

    Gerenciador de Boot (GRUB2): Software que permite escolher qual sistema operacional ou kernel iniciar. É instalado no Master Boot Record (MBR) ou em uma partição EFI.

    Instalação Automatizada (Kickstart): Para ambientes corporativos, arquivos Kickstart automatizam totalmente o processo de instalação, respondendo a todas as perguntas.

Capítulo 10: Gerenciando Softwares e Pacotes (RPM/YUM)

10.1. RPM (Red Hat Package Manager)
É o formato de pacote padrão para Fedora/RHEL. Um arquivo .rpm contém os binários, arquivos de configuração, documentação e metadados do software.

10.2. YUM/DNF (Gerenciador de Pacotes)
O YUM (Yellowdog Updater, Modified) (substituído pelo DNF no Fedora) resolve o "inferno das dependências". Ele busca pacotes em repositórios e instala tudo o que é necessário automaticamente.

    yum install nome_do_pacote: Instala um pacote.

    yum update: Atualiza todos os pacotes do sistema.

    yum remove nome_do_pacote: Remove um pacote.

    yum search palavra_chave: Procura por um pacote.

    yum provides */nome_do_arquivo: Descobre qual pacote fornece um arquivo específico.

10.3. Repositórios
São servidores que armazenam coleções de pacotes RPM. A configuração fica em /etc/yum.repos.d/. Repositórios de terceiros como EPEL e RPM Fusion fornecem softwares adicionais não incluídos na distribuição oficial.
Capítulo 11: Gerenciando Usuários e Grupos

    useradd: Cria uma nova conta de usuário.

        useradd -c "Nome Completo" -m -s /bin/bash usuario

    usermod: Modifica uma conta existente.

        usermod -aG wheel usuario (Adiciona o usuário ao grupo wheel para poder usar sudo).

    userdel: Remove um usuário.

        userdel -r usuario (Remove também o diretório /home do usuário).

    passwd: Define ou altera a senha de um usuário.

    groupadd: Cria um novo grupo.

Arquivos Importantes:

    /etc/passwd: Informações da conta do usuário (nome, UID, GID, shell). Legível por todos.

    /etc/shadow: Senhas criptografadas e informações de envelhecimento. Legível apenas pelo root.

    /etc/group: Informações sobre os grupos do sistema.

Permissões Especiais:

    Sticky Bit (o+t): Em diretórios como /tmp, impede que um usuário delete arquivos de outros usuários.

    Set GID (g+s): Em diretórios, faz com que novos arquivos criados herdem o grupo do diretório. Útil para pastas de colaboração.

Capítulo 12: Gerenciando Discos, Partições e LVM

12.1. Ferramentas de Particionamento

    fdisk: Ferramenta clássica para criar e modificar partições MBR.

    parted / gdisk: Ferramentas modernas para discos GPT (necessário para discos > 2TB).

12.2. LVM (Logical Volume Manager)
O LVM cria uma camada de abstração entre os discos físicos e os sistemas de arquivos, oferecendo uma flexibilidade incrível.

    Conceitos:

        PV (Physical Volume): Partições de disco ou discos inteiros formatados para LVM.

        VG (Volume Group): Um "pool" de armazenamento composto por um ou mais PVs.

        LV (Logical Volume): "Partições virtuais" criadas dentro de um VG. É onde os sistemas de arquivos são criados.

    Principais Comandos LVM:

        pvcreate /dev/sdb1: Cria um PV.

        vgcreate meu_vg /dev/sdb1: Cria um VG.

        lvcreate -n meu_lv -L 10G meu_vg: Cria um LV de 10GB.

        lvextend -L +5G /dev/meu_vg/meu_lv: Aumenta o tamanho de um LV.

12.3. Montagem de Sistemas de Arquivos

    mount: Conecta um sistema de arquivos a um diretório (ponto de montagem).

        mount /dev/sdb1 /mnt/meu_disco

    /etc/fstab: Arquivo que define quais sistemas de arquivos são montados automaticamente na inicialização.

Parte IV: Tornando-se um Administrador de Servidores Linux
Capítulo 13: Conceitos de Administração de Servidores e Acesso Remoto (SSH)

13.1. O Ciclo de Vida de um Serviço

    Instalar: yum install <pacote>.

    Configurar: Editar arquivos em /etc/.

    Iniciar: systemctl start <serviço>.

    Habilitar (persistente): systemctl enable <serviço> (inicia no boot).

    Proteger: Configurar firewall, SELinux e permissões.

    Monitorar: Verificar logs, uso de recursos.

13.2. Acesso Remoto Seguro (SSH)
O SSH substitui ferramentas inseguras como telnet.

    ssh usuário@servidor: Conecta-se a um servidor remoto de forma criptografada.

    scp arquivo.txt usuário@servidor:/tmp/: Copia um arquivo de forma segura.

    rsync: Ferramenta de sincronização que usa SSH, ideal para backups por ser incremental (copia apenas as diferenças).

    Chaves SSH: Permitem autenticação sem senha. Você gera um par de chaves (pública e privada) e copia a chave pública para o servidor (ssh-copy-id).

13.3. Logs do Sistema

    rsyslog: O principal serviço de logging. Configurado em /etc/rsyslog.conf. Os logs são armazenados em /var/log/.

    logwatch: Ferramenta que analisa os logs diariamente e envia um resumo por e-mail para o administrador.

Capítulo 14: Configuração e Administração de Redes

    ip addr show: Exibe as interfaces de rede e seus endereços IP.

    ping google.com: Testa a conectividade com um host remoto.

    Arquivos de Configuração (RHEL/Fedora):

        /etc/sysconfig/network-scripts/ifcfg-<interface>: Configurações de cada placa de rede (DHCP ou IP estático).

        /etc/resolv.conf: Define os servidores DNS.

    NetworkManager: Serviço que simplifica a configuração de rede em desktops, lidando com Wi-Fi, VPNs, etc.

Capítulo 15: Controlando Serviços (systemd e SysVinit)

systemd é o sistema de inicialização moderno (usado no Fedora, RHEL 7+ e Ubuntu recente), substituindo o antigo SysVinit.
Ação	Comando systemd (systemctl)
Iniciar um serviço	systemctl start nome.service
Parar um serviço	systemctl stop nome.service
Reiniciar um serviço	systemctl restart nome.service
Recarregar configurações	systemctl reload nome.service
Habilitar no boot	systemctl enable nome.service
Desabilitar no boot	systemctl disable nome.service
Verificar status	systemctl status nome.service
Listar serviços com falha	systemctl --failed
Mudar runlevel padrão	systemctl set-default multi-user.target (modo texto)
Capítulo 16 a 20: Configurando Servidores Específicos

    Impressão (CUPS): Serviço de impressão padrão. Configurado via interface web (http://localhost:631).

    Web (Apache): Servidor web mais popular. Pacote httpd. Conteúdo padrão em /var/www/html.

    FTP (vsftpd): "Very Secure FTP Daemon". Permite transferência de arquivos (não criptografada).

    Windows/Samba: Permite que um servidor Linux compartilhe arquivos e impressoras com clientes Windows usando o protocolo SMB/CIFS.

    NFS (Network File System): Protocolo padrão para compartilhar arquivos entre sistemas Linux/Unix.

Capítulo 21: Solução de Problemas no Linux

    Inicialização:

        Problemas com a BIOS/ordem de boot.

        Problemas com o GRUB: Pode ser necessário entrar no modo de recuperação (Rescue Mode) a partir da mídia de instalação.

        Problemas com o Kernel: Inicializar com um kernel mais antigo listado no menu do GRUB.

    Memória:

        Uso excessivo de RAM leva à troca (swap), causando lentidão.

        Comandos: free -h, top (coluna %MEM).

        OOM Killer (Out-Of-Memory) encerra processos quando a memória acaba.

    Rede:

        Verificar se o cabo está conectado ou Wi-Fi ligado.

        Usar ping para testar conectividade.

        Usar traceroute para ver a rota dos pacotes.

        Verificar firewall local (iptables -L).

    Sistema de Arquivos:

        df -h para verificar espaço em disco.

        du -sh /diretorio para encontrar o que está ocupando espaço.

    Modo de Recuperação (Rescue Mode): Inicializar a partir de um CD/DVD/USB para acessar e reparar o sistema instalado no disco rígido.

Parte V: Segurança no Linux
Capítulo 22: Fundamentos de Segurança

    Ciclo de Vida da Segurança: Planejar, Implementar, Monitorar, Auditar.

    Segurança Física: Restringir o acesso à sala do servidor.

    Contas e Senhas:

        Uma conta por usuário (não compartilhe).

        Não logar diretamente como root.

        Impor políticas de senha forte e envelhecimento com o comando chage e o arquivo /etc/login.defs.

    Sistema de Arquivos:

        Cuidado com permissões "perigosas" (777).

        Localizar arquivos sem dono (find / -nouser).

    Detecção de Intrusão:

        rpm -Va: Verifica a integridade de todos os pacotes instalados.

        AIDE / Tripwire: Sistemas de Detecção de Intrusão (IDS) baseados em host que verificam alterações em arquivos críticos.

Capítulo 23: Segurança Avançada (Criptografia e PAM)

    Criptografia:

        Simétrica: Usa uma única chave para cifrar e decifrar. Rápida. Ex: AES, Blowfish.

        Assimétrica: Usa um par de chaves (pública e privada). Lenta, mas resolve o problema de troca de chaves. Ex: RSA. Ferramenta: GnuPG (gpg).

        Hashing: Gera uma "impressão digital" única e irreversível de um arquivo. Usado para verificar integridade. Ex: md5sum, sha256sum.

    PAM (Pluggable Authentication Modules): Estrutura que centraliza a autenticação de usuários para todos os serviços (login, SSH, su). Configurável através de arquivos em /etc/pam.d/. Permite impor restrições complexas, como limites de recursos, horários de login e uso de autenticação de dois fatores.

Capítulo 24: SELinux (Security-Enhanced Linux)

O SELinux implementa o Controle de Acesso Mandatório (MAC). Ele adiciona uma camada de segurança sobre as permissões tradicionais do Linux (DAC - Controle de Acesso Discricionário).

Conceitos-chave do SELinux:

    Modos:

        Enforcing: Políticas do SELinux são impostas. Acesso negado é bloqueado e logado.

        Permissive: Políticas não são impostas, mas violações são logadas. Útil para testes e depuração.

        Disabled: Desativado.

    Contexto de Segurança: Todo processo, arquivo e usuário tem um rótulo (contexto) SELinux. Ex: system_u:object_r:httpd_sys_content_t:s0. As políticas definem quais contextos podem interagir.

    Booleanos: "Chaves" que ligam/desligam partes específicas da política do SELinux sem a necessidade de criar novas regras complexas.

        Exemplo: setsebool -P httpd_enable_homedirs on (permite ao Apache acessar diretórios /home).

    Comando Útil: restorecon -R /var/www/html (restaura o contexto de segurança padrão dos arquivos).

Capítulo 25: Segurança de Rede (Firewall iptables)

O firewall padrão do Linux é o Netfilter, gerenciado pelo comando iptables. Ele opera com tabelas, cadeias e regras.

Estrutura Básica do iptables:

    Tabelas: filter (padrão), nat, mangle.

    Cadeias (chains): INPUT (tráfego de entrada), OUTPUT (saída), FORWARD (roteamento).

    Política Padrão (policy): O que fazer se nenhuma regra corresponder (ex: DROP tudo).

    Regras (rules): Exceções à política padrão (ex: ACCEPT porta 22).

Exemplo de Configuração Simples:
bash

# Definir política padrão como DROP (bloquear tudo)
iptables -P INPUT DROP
iptables -P FORWARD DROP
iptables -P OUTPUT ACCEPT

# Permitir tráfego na interface de loopback (localhost)
iptables -A INPUT -i lo -j ACCEPT

# Permitir conexões já estabelecidas e relacionadas
iptables -A INPUT -m state --state ESTABLISHED,RELATED -j ACCEPT

# Permitir acesso SSH (porta 22)
iptables -A INPUT -p tcp --dport 22 -j ACCEPT

# Permitir acesso Web (porta 80)
iptables -A INPUT -p tcp --dport 80 -j ACCEPT

    Salvar Regras: service iptables save (RHEL/CentOS 6) ou iptables-save > /etc/iptables/rules.v4 (sistemas modernos).

    TCP Wrappers: Outra camada de controle de acesso baseada nos arquivos /etc/hosts.allow e /etc/hosts.deny.
