# Terminal Cheatsheet para Mac (Fundamentos)

Tradução inicial por [zeluizr](https://github.com/zeluizr)

Tradução e revisão por [mateuscard](https://github.com/mateuscard)

_As letras estão maiúsculas apenas com o intuito de facilitar a leitura. Caps lock deve estar desativado._

------------

## ATALHOS

| Atalho | Descrição |
| ----------- | ----------- |
| Ctrl + A | Vai ao início da linha em que você está digitando. Este atalho também funciona para a maioria dos campos de entrada de texto do sistema. O Netbeans é uma exceção |
| Ctrl + E | Vai ao final da linha em que você está digitando. Este atalho também funciona para a maioria dos campos de entrada de texto do sistema. O Netbeans é uma exceção |
| Ctrl + L | Limpa a tela |
| Command + K | Limpa a tela |
| Ctrl + U | Remove a linha que antecede a posição do cursor |
| Ctrl + K | Remove a linha que sucede a posição do cursor |
| Ctrl + W | Remove a palavra antes da posição do cursor usando o espaço em branco como delimitador | 
| Ctrl + Y | Cola o que foi cortado pelo último comando de corte |
| Ctrl + H | Faz o mesmo que o backspace |
| Ctrl + C | Cancela o que está sendo executado e limpa a linha |
| Ctrl + D | Sai do shell atual quando nenhum processo estiver em execução |
| Ctrl + Z | Coloca o que está sendo executado em segundo plano. Pode ser restaurado pelo comando `fg` |
| Ctrl + _ | Desfaz o último comando |
| Ctrl + T | Troca os dois caracteres que antecedem a posição do cursor |
| Ctrl + F | Move a posição do cursor um caractere para frente |
| Ctrl + B | Move a posição do cursor um caractere para trás |
| Option + → | Move a posição do cursor uma palavra para frente |
| Option + ← | Move a posição do cursor uma palavra para trás |
| Esc + T | Troca as duas palavras que antecedem a posição do cursor |
| Esc + Backspace | Remove a palavra que antecede a posição do cursor usando caracteres não alfabéticos como delimitadores 
| Tab | Preenche automaticamente o nome de arquivos e pastas

## COMANDOS PRINCIPAIS

| Atalho | Descrição |
| ----------- | ----------- |
| cd [pasta] | Altera o diretório |
| cd | Vai ao diretório `home`|
| cd / | Vai ao diretório raiz |
| cd - | Volta ao diretório anterior |
| ls | Lista os arquivos |
| ls -l | Lista os arquivos no formato lista |
| ls -a | Lista os arquivos incluindo os ocultos |
| ls -lh | Lista os arquivos com detalhes legíveis |
| ls -R | Lista os arquivos recursivamente |
| sudo [comando] | Executa um comando com privilégios de seguração do superusuário (Super User DO) |
| open [arquivo] | Abre o arquivo (simula o duplo clique) |
| top | Exibe os processos ativos. Pressione `q`para sair |
| nano [arquivo] | Abre o arquivo usando o editor nano |
| vim [arquivo] | Abre o arquivo usando o editor vim |
| clear | Limpa a tela |
| reset | Redefine a tela do terminal |

## COMANDOS DE ENCADEAMENTO

| Atalho | Descrição |
| ----------- | ----------- |
| [comando-a]; [comando-b] | Executa primeiro o comando A e depois o B independente do sucesso de A |
| [comando-a] && [comando-b] | Executa o comando B somente se A suceder |
| [comando-a] \|\| [comando-b] | Executa o comando B somente se A falhar |
| [comando-a] & | Executa o comando A em segundo plano |

## COMANDOS DE TUBULAÇÃO

| Atalho | Descrição |
| ----------- | ----------- |
| [comando-a] \| [comando-b] | Executa o comando A e depois passa o resultado para o comando B |

## COMANDOS DE HISTÓRICO

| Atalho | Descrição |
| ----------- | ----------- |
| history n | Mostra o que foi digitado anteriormente - adicione um número para ver somente os n últimos itens |
| Ctrl + r  | Pesquisa interativamente por comandos digitados anteriormente |
| ![value] | Executa o último comando digitado que começa com `value` |
| ![value]:p | Imprime no console o último comando digitado que começa com `value`|
| !! | Executa o último comando digitado |
| !!:p | Imprime no console o último comando digitado |

## COMANDOS DE GERENCIAMENTO DE ARQUIVOS

| Atalho | Descrição |
| ----------- | ----------- |
| touch [arquivo] | Cria um novo arquivo |
| pwd | Realiza o caminho completo até o diretório de trabalho |
| . | Pasta atual |
| .. | Diretório parente/anexo |
| ls -l .. | Lista os arquivos do diretório parente |
| cd ../../ | Move a posição dois níveis acima |
| cat | Concatena para a tela |
| rm [arquivo] | Remove um arquivo |
| rm -i [arquivo] | Remove um arquivo e requesita confirmacão |
| rm -r [diretório] | Remove um diretório e seus conteúdos |
| rm -f [arquivo] | Força a remoção sem confirmação |
| cp [arquivo] [novo-arquivo] | Copiar arquivo para novo-arquivo |
| cp [arquivo] [diretório] | Copiar arquivo para o diretório |
| mv [arquivo] [novo-nome-do-arquivo] | Move ou renomeia o arquivo |
| pbcopy < [arquivo] | Copia o conteúdo do arquivo para a área de transferência |
| pbpaste | Cola o conteúdo da área de transferência |
| pbpaste > [arquivo] | Cola o conteúdo da área de transferência no arquivo |

## COMANDOS DE GERENCIAMENTO DE DIRETÓRIO

| Atalho | Descrição |
| ----------- | ----------- |
| mkdir [diretório] | Cria um novo diretório |
| mkdir -p [diretório]/[diretório] | Cria diretórios ordenados |
| rmdir [diretório] | Remove diretório (opera apenas em diretórios vazios) |
| rm -R [diretório] | Remove o diretório e seu conteúdo |
| less [arquivo]| Entrega o resultado do arquivo de saída em blocos do tamanho da tela |
| [comando] > [arquivo] | Adiciona o resultado ao arquivo - lembre-se que ela será substituída |
| [comando] >> [arquivo] | Anexa o resultado ao arquivo existente |
| [comando] < [arquivo] | Avisa ao comando para ler o conteúdo de um arquivo |

## COMANDOS DE BUSCA

| Atalho | Descrição |
| ----------- | ----------- |
| find [diretório] -name [padrão-de-pesquisa] | Procura por arquivos |
| grep [padrão-de-pesquisa] [arquivo] | Procura por todas as linhas que contêm o padrão |
| grep -r [padrão-de-pesquisa] [diretório] | Procura recursivamente, em todos os arquivos, no diretório especificado todas as linhas que contêm o padrão |
| grep -v [padrão-de-pesquisa] [arquivo] | Procura por todas as linhas que NÃO contêm o padrão |
| grep -i [padrão-de-pesquisa] [arquivo] | Procura por todas as linhas que contêm o padrão sem diferenciar as letras maiúsculas das minúsculas |
| mdfind [padrão-de-pesquisa] | Pesquisa `Spotlight` por arquivos (nomes, conteúdo e outros metadados) |
| mdfind -onlyin [diretório] -name [padrão] | Pesquisa `Spotlight` por arquivos nomeados como o padrão no diretório especificado |

## COMANDOS DE AJUDA

| Atalho | Descrição |
| ----------- | ----------- |
| [comando] -h | Oferece ajuda |
| [comando] --help | Oferece ajuda |
| info [comando] | Oferece ajuda |
| man [comando] | Mostra o manual de ajuda para [comando] |
| whatis [comando] | Fornece uma descrição do [comando] em uma linha |
| apropos [padrão-de-pesquisa] | Procura por comandos com palavras-chave na descrição |