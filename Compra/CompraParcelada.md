Algoritmo "semnome"
//  
//  
// Descrição   : Aqui você descreve o que o programa faz! (função)
// Autor(a)    : Nome do(a) aluno(a)
// Data atual  : 14/05/2021
Var
// Seção de Declarações das variáveis 
   valor_produto, parcelas :real
   total_compra, total_final :real
   juros5, juros10 : inteiro
Inicio

      escreva ("Qual o valor do Produto ?")
      leia (valor_produto)
      escreval ("Valor do Produto: ",valor_produto)
      escreva ("qual a quantidade de parcelas ?")
      leia (parcelas)
       juros5 <-5
       juros10 <-10
      total_compra <- (valor_produto / parcelas)

      escreval ("Total da compra: ",parcelas,"x",total_compra," Reais ")
         se (parcelas >3) e (parcelas<6)  entao
            total_compra <- valor_produto + (valor_produto * juros5)/ 100
            total_final <- total_compra / parcelas
            escreval ("Valor com juros de 5% ")
            escreval ("Valor com juros", total_compra," parcelas : ",parcelas,"x",total_final,"R$")

         senao

            se (parcelas >6) e (parcelas<13)  entao
               total_compra <- valor_produto + (valor_produto * juros10)/ 100
               total_final <- total_compra / parcelas
               escreval ("Valor com juros de 10% ")
               escreval ("Valor com juros", total_compra," parcelas : ",parcelas,"x",total_final,"R$")

            senao

 
                  se (parcelas > 12) entao

                  escreval("Não parcelamos MAIS que 12x")

               fimse

            fimse


         fimse
