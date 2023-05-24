## Anotações rápidas sobre tmux 
    (versão customizada [nesse repo](https://github.com/antonioanerao/dotfiles))

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
