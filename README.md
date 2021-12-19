# Avaliacao_Senai-

 Nesse repositório está presente, as duas questões propostas na avaliação de 60 pontos, da matéria Lógica de Programação
 Questão 1:
  	/*	Uma empresa concederá um aumento de salário aos seus funcionários, variável de acordo com o cargo, conforme a tabela abaixo.
			Faça um algoritmo que leia o salário e o cargo de um funcionário e calcule o novo salário. Se o cargo do funcionário não estiver na tabela, ele deverá, então, receber 40% de aumento. 
			Mostre o salário antigo, o novo salário e a diferença. 
			Código Cargo  Percentual
			 101   Gerente   10%
			 102  Engenheiro 20%
			 103  Técnico    30%    */
programa
{
	
	funcao inicio()
	{
		cadeia nomeDoCargo = " "
		inteiro CodigoCargo
		real salarioAntigo = 0.0, novoSalario = 0.0, diferencaSalario = 0.0

		escreva(" ============================================================= \n")
		escreva(" Escolha o seu cargo: \n (101)Gerente \t (103) Técnico \n (102)Engenheiro \n ")
		escreva(" OBS: Caso o seu cargo não tenha aparecido acima, não tem problema, pode digitar ele aqui \n Digite aqui o número do seu cargo: ")
		leia(CodigoCargo)
		limpa()

		escreva(" ============================================================= \n")
		escreva(" Digite o seu salário R$: ")
		leia(salarioAntigo)
		limpa()

		escolha(CodigoCargo){
			caso 101:
				novoSalario = (salarioAntigo * 10/100) + salarioAntigo
				nomeDoCargo = " Gerente "
				
			pare
			caso 102:
				novoSalario = (salarioAntigo * 20/100) + salarioAntigo
				nomeDoCargo = " Engenheiro "
				
			pare
			caso 103:
				novoSalario = (salarioAntigo * 30/100) + salarioAntigo
				nomeDoCargo = " Técnico "
				
			pare
			caso contrario:
				novoSalario = (salarioAntigo * 40/100) + salarioAntigo
				nomeDoCargo = " Outros não alistados "
				
			}
			diferencaSalario = novoSalario - salarioAntigo  
			escreva(" Como o seu cargo é o =  ", nomeDoCargo ," E o seu salário era de R$: " , salarioAntigo,  " | " , " Você recebeu aumento e a partir de agora seu salário será de R$ " , novoSalario , " | " , " Isso significa uma diferença(em reais) de R$ " , diferencaSalario)
		
	}
}

FIM DA QUESTÃO 1 
============================================

INÍCIO DA QUESTÃO 2:

/*Faça um programa que leia valores digitados em uma matriz 3 x 4 de tipo inteiro, 
	substitua seus elementos negativos por 0 e imprima a matriz. */


programa
{
	
	funcao inicio()
	{
		
    inteiro lagrimas[3][4] 
		inteiro l = 0, c = 0 
		para(l=0; l<3 ; l++) 
			para(c = 0 ; c<4 ; c++){ 
				escreva(" Entre com o elemento linha =  ", l , " e coluna  ", c , " = ") 
				leia(lagrimas[l][c]) 
				limpa() 
				
				} 
				escreva(" Por favor aguarde, estamos fazendo a verificação na Matriz, se existe algum valor negativo \n")
				escreva(" \n Imprimindo a Matriz - Lagrimas, com a substituição dos valores neagtivos por '0' \n ")
					para(l=0;l<3;l++){
						para(c=0;c<4;c++){
							se(lagrimas[l][c]<0){
								lagrimas[l][c] = 0
								} escreva("\n Valor na linha =  ", l, " e na coluna ", c , " = ", lagrimas[l][c])	
						             
							} } escreva(" \n\n Fim da Execução \n ", " ========================================== ")
					
	} 		
}

FIM DA QUESTÃO 2
==============================================
