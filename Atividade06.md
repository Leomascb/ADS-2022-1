# ADS-2022-1
Repository created as a part of a continuous assessment required by the professor responsible for Logic in Programming
Algoritmo "atividade06"
   Var
      A, B, M, D, P: real
      X: caractere
Inicio
   escreva ("Qual operação deseja realizar? ")
   leia (X)
      se (X = "multiplicação") então
         leia (A, B)
         P <- A*B
         escreva (P)
      fimse
      
      se (X = "diferença") então
         leia (A, B)
         se (A > B) então
            D <- A - B
         senão
            D <- B - A
         fimse
         escreva (D)
      fimse

      se (X = "média") então
         leia (A, B)
            M <- (A + B)/2
         escreva (M)
      fimse
      
      se (X <> "multiplicação") e (X <> "média") e (X <> "diferença") então
         escreva ("Sua opção é inválida.")
      fimse
Fimalgoritmo
