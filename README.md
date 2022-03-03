# ADS-2022-1
Repository created as a part of a continuous assessment required by the professor responsible for Logic in Programming
Algoritmo "atividade24"
   Var
      PRECO, VA, VI, NOVO_PRECO: real
      CATEGORIA: inteiro
      SITUACAO: caractere

Inicio
   escreva ("Qual o preço de seu produto? ")
   leia (PRECO)
   escreva ("Qual a categoria de seu produto? ")
   leia (CATEGORIA)
   se (PRECO <= 25) entao
      se (CATEGORIA = 1) entao
         VA <- PRECO*0.05
      fimse
      se (CATEGORIA = 2) entao
         VA <- PRECO*0.08
      fimse
      se (CATEGORIA = 3) entao
         VA <- PREÇO*0.1
      fimse
   fimse
   
   se (PRECO > 25) entao
      se (CATEGORIA = 1) entao
         VA <- PRECO*0.12
      fimse
      se (CATEGORIA = 2) entao
         VA <- PRECO*0.15
      fimse
      se (CATEGORIA = 3) entao
         VA <- PRECO*0.18
      fimse
   fimse
   escreva ("O valor do aumento é de: ", VA)
   
   se (CATEGORIA = 2) ou (SITUACAO = "R") entao
      VI <- PRECO*0.05
   senao
      VI <- PRECO*0.08
   fimse
   escreva (". O valor do imposto é de: ", VI)
   
   NOVO_PRECO <- PRECO + VI
   se (NOVO_PRECO <= 50) entao
      escreva ("O novo preço é de: ", NOVO_PRECO, ". Classificação: Barato.")
   fimse
   se (NOVO_PRECO > 50) e (NOVO_PRECO < 120) entao
      escreva ("O novo preço é de: ", NOVO_PRECO, ". Classificação: Normal.")
   fimse
   se (NOVO_PRECO >= 120) entao
      escreva ("O novo preço é de: ", NOVO_PRECO, ". Classificação: Caro")
   fimse
Fimalgoritmo
