Algoritmo "Cadastro de material de limpeza"

Var
 produto : caractere
   quantidade, opcao : inteiro


Inicio
quantidade <- 0

   repita

      escreval("====== CONTROLE DE ESTOQUE ======")
      escreval("1 - Adicionar material")
      escreval("2 - Retirar material")
      escreval("3 - Ver estoque")
      escreval("4 - Sair")
      escreva("Escolha uma opcao: ")
      leia(opcao)

      escolha opcao

         caso 1
            escreva("Digite o nome do material: ")
            leia(produto)

            escreva("Quantidade para adicionar: ")
            leia(opcao)

            quantidade <- quantidade + opcao

            escreval("Material adicionado com sucesso!")

         caso 2
            escreva("Quantidade para retirar: ")
            leia(opcao)

            se opcao <= quantidade entao
               quantidade <- quantidade - opcao
               escreval("Material retirado!")
            senao
               escreval("Estoque insuficiente!")
            fimse

         caso 3
            escreval("Produto: ", produto)
            escreval("Quantidade em estoque: ", quantidade)

         caso 4
            escreval("Encerrando sistema...")

         outrocaso
            escreval("Opcao invalida!")

      fimescolha

   ate opcao = 4

fimalgoritmo

