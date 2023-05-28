
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

## Find/Replace

#### Buscar um texto e substituir em todo o arquivo (um item por linha)
    :%s/texto-atual/texto-novo

#### Buscar um texto e substituir tudo que encontrar em todo o arquivo 
    :%s/texto-atual/texto-novo/g
    

#### Buscar um texto e substituir (confirmar antes da substituicao) 
    :%s/texto-atual/texto-novo/gc
    
#### Substituir texto dentro das linhas selecionadas 
    # Aperte : e após os simbolos que já aparecem no input <:'<,'>> digite:
    s/texto-atual/texto-novo
    
    # Exemplo
    :'<,'>s/text-center/text-right
    
#### Apagar todas as linhas que contem uma palavra
    :%g/texto-a-deletar/d
    
    # Exemplo apagando todas as divs
    :%g/div/d
    
#### Apagar todas as linhas que NÃO contem uma palavra
    :%v/texto-a-deletar/d
    
    # Exemplo apagando todas as divs
    :%v/div/d
    
#### Substituir em varios arquivos (Necessario plugin Telescope)
    # Abrir tela de busca por conteudo dentro dos arquivos
    f + g
    
    # Apos a busca apertar:
    ctrl + q
    
    # Apertar : e digitar o seguinte:
    cdo s/texto-atual/texto-novo
    
    # Pode-se usar o /g para substituir todos resultos de uma mesma linha e /c para confirmar antes de substituir
