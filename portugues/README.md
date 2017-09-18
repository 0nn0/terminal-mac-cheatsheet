# Terminal Cheatsheet para Mac (básico)
Original translation by [zeluizr](https://github.com/zeluizr)

------------

## ATALHOS

| Atalho | Descrição |
| ------ | ----------|
| Ctrl + A | Ir para o início da linha em que você está digitando |
| Ctrl + E | Vá para o final da linha em que você está digitando |
| Ctrl + L | Limpa a tela |
| Command + K | Limpa a tela |
| Ctrl + U | Limpa a linha antes da posição do cursor. Se estiver no fim da linha, apaga toda a linha. |
| Ctrl + H | O mesmo que backspace |
| Ctrl + R | Permite pesquisar através de comandos usados ​​anteriormente |
| Ctrl + C | Para o que você está executando |
| Ctrl + D | Sair do shell atual |
| Ctrl + Z | Coloca o que está sendo executado em um processo de segundo plano. O comando "fg" para restaura-lo. |
| Ctrl + W | Para excluir a palavra antes do cursor |
| Ctrl + K | Apague a linha após o cursor |
| Ctrl + T | Troque os dois últimos caracteres antes do cursor |
| Esc + T | Troque as duas últimas palavras antes do cursor |
| Option + → | Mover o cursor uma palavra para frente na linha atual |
| Option + ← | Move cursor backward one word on the current line |
| Tab | Auto-Completar de comandos e nomes de arquivos. |


## COMANDOS PRINCIPAIS

| Atalho | Descrição |
| ------ | ----------|
| cd | Diretório Home |
| cd [pasta] | Muda o diretório |
| cd ~ | Diretório Home, ex.: 'cd ~/pasta/' |
| cd / | Diretório raiz (root) |
| ls | Lista os arquivos na pasta |
| ls -l | Lista os arquivos de uma pasta no formato lista |
| ls -a | Lista os arquivos de uma pasta contantendo os arquivos escondidos |
| ls -lh | Lista os arquivos de uma pasta com todos os detalhes |
| ls -R | Lista os arquivos de uma pasta recursivamente |
| sudo [comando] | Executar comando com os privilégios de super-usuário |
| open [arquivo] | Abre um arquivo (como se você clica-se duas vezes nele) |
| top | Mostra processos ativos. Precione "q" para sair |
| nano [arquivo] | Abre o editor do Terminal |
| pico	[arquivo] | Abre o editor do Terminal |
| exit | Sair do Terminal |
| clear | Limpa a tela |


## COMANDOS DE HISTÓTICO

| Atalho | Descrição |
| ------ | ----------|
| history n | Mostra os comandos digitados - Quantos históricos serão exibidos a partir do último comando |
| ctrl-r | Permite pesquisar através de comandos usados ​​anteriormente |
| ![valor] | Execute o último comando digitado que começa com 'valor' |
| !! | Execute o último comando digitado |


## MANIPULANDO ARQUIVOS

| Atalho | Descrição |
| ------ | ----------|
| touch [arquivo] | Cria um novo arquivo |
| pwd | Caminho completo para o diretório de trabalho |
| ls -l | Lista completa do diretório pai |
| cd ../../ | Move dois niveis acima |
| cd . | Pasta atual |
| cd .. | Voltar uma pasta |
| cat | Concatenar as telas |
| rm [arquivos] | Apaga arquivos, ex.: rm [arquivo] [arquivo] |
| rm -i [arquivo] | Deletar com comfirmação |
| rm -r [diretorio] | Apaga um diretório e seu conteúdo |
| rm -f [arquivo] | Força o apagar sem confirmação |
| cp [arquivo] [novo arquivo copiado] | Copiar arquivo |
| cp [arquivo] [diretorio] | Copiar um arquivo para outro diretorio |
| mv [arquivo] [novo nome] | Move/Renomeia, ex.: mv -v [arquivo] [diretorio] |


## MANIPULANDO DIRETÓRIOS

| Atalho | Descrição |
| ------ | ----------|
| mkdir [diretorio] | Cria uma nova pasta |
| mkdir -p [diretorio]/[diretorio] | Cria uma pasta com uma sub-pasta |
| rmdir [diretorio] | Remove pasta ( esse comando só funciona se a pasta estiver vazia ) |
| rm -R [diretorio] | Remove a pasta com todos os arquivos dentro |
 


## PIPES - permite combinar vários comandos que geram saída

| Atalho | Descrição |
| ------ | ----------|
| > [arquivo] | Gera um novo arquivos, lembrando que ela pode ser sobrescrita |
| >> [arquivo] | Adiciona a saida ao arquivos |


## AJUDA

| Atalho | Descrição |
| ------ | ----------|
| [comando] -h | Exibe ajuda do comando |
| [comando] --help | Exibe ajuda do comando |
| [comando] help | Exibe ajuda do comando |
| reset | Reseta sua tela atual no terminal |
| man [comando] | Exibe ajuda para o seu 'comando' |
| whatis [comando] | Dá uma descrição de uma linha de 'comando' |

## COMANDOS PARA GIT

| Atalho | Descrição |
| ------ | ----------|
| [comando] git init | Inicia um projeto git na pasta atual. |