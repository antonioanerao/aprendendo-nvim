## Comandos nvim

#### Direcionais
- **h** esquerda
- **j** baixo
- **k** cima
- **l** esquerda

#### Salvar/sair do arquivo
- **:w** salvar
- **:wq** salvar e sair
- **:w** nomeArquivo cria o arquivo e salva
- **:wq** nomeArquivo cria o arquivo, salva e sai

#### Ir para o fim da linha
    Tecla (Shift + $)

#### Copiar linha onde está o cursor 
    Tecla: yy
    
#### Colar texto copiado onde está o cursor
    Tecla: p

#### Visual Mode 
    Seleciona o texto ao mover com os direcionais
    Tecla: v
    
#### Line Mode
    Seleciona várias linhas com os direcionais
    Tecla: Shift + v
    Tecla (o): Ir para o lado oposto da seleção

#### Block Mode
    Seleciona blocos de texto com os direcionais
    Tecla: CTRL + v
    
    Tecla (o): Ir para o lado oposto da seleção
    Tecla (Shift + I): Adiciona texto no local da seleção nas linhas selecionadas
    
    Tecla (Shift + $): Vai para o fim da seleção
    Tecla (Shift + a): Posiciona o insert no fim da seleção para adicionar texto à todas as linhas
    
#### Criar novo arquivo a partir de um arquivo aberto no nvim
    :enew
    
#### Abrir um novo arquivo
    :e nomeArquivo
    
#### Listar arquivos abertos
    :ls
    
#### Abrir um dos arquivos listados com o :ls
    :b númeroArquivo
    
#### Navegar entre arquivos abertos
    CTRL + 6
        
    
#### Dois arquivos recentes dividindo a tela horizontalmente
    :split / :sp   
    
#### Dois arquivos recentes dividindo a tela verticalmente
    :vsplit / :vs   
    

#### Trocar o cursor entre splits
    CTRL + W e depois algum direcional
    
    
#### Nova aba
    :tabnew
 
#### Ir para aba anterior
    :tabp
    
#### Ir para próxima aba
    :tabn

#### Avançar/voltar x abas
    :tabn/:tabp qntAbas
    
    *Os comandos de sair/salvar/sair sem salvar podem ser aplicados a vários arquivos
    Ex: :wa :wqa :qa!
    
   
## Anotações rápidas sobre tmux (versão customizada [nesse repo](https://github.com/antonioanerao/dotfiles))

#### Iniciar tmux

    $ tmux
    
#### Abrir nova aba tmux

    # CTRL + Espaço > c
    
#### Navegar entre as abas abertas

    $ CTRL + Espaço > Número da aba
    
    
#### Dividir a tela do tmux em 2 (vertical)

    $ CTRL + Espaço > SHIFT + 5
    
#### Alterar entre telas divididas

    $ CTRL + Espaço > setas direcionais 
    
#### Aumentar ou diminuir o tamanho de uma tela dividida

    $ CTRL + Espaço + seta direcional (apertar a seta repetidas vezes, sem soltar o CTRL + Espaço)
    
#### Abrir lista de comandos

    $ CTRL + Espaço > :
    
#### Fechar todas as sessões do tmux

    $ tmux kill-server
    
#### Fazer um "detach" do tmux sem encerrar a sessão
    
    $ CTRL + Espaço > D
    
#### Listar todas as sessões tmux

    $ tmux ls
    
#### Voltar para uma sessão específica

    $ tmux attach-session -t número-da-sessão
