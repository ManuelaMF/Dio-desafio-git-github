# Anotações Introdução à Lógica e à programação

### Usando o "*Portugol*" como base o professor apresentou alguns códigos para trabalhar com programação

- Use para quebrar linhas "\n"

- Use "+" para fazer concatenação

- Quando for uma condição falsa utilizar "senao" + "{" (ele fecha só)

- Quando for uma condição verdadeira utilizar "se" + "{"

- Para adicionar comentário use "//" (similar ao -m do git)

- Quando usar contador utilize "++" para indicar que ele deve contar +1

- Para que o software escreva algo utilize o comando "escreva"

- Para que leia o que você escreveu digite "leia" (semelhante ao comando "echo" do git)

- "real" indica que as variáveis são quebradas

- "inteiro" indica que variáveis são inteiras

- "cadeia" indica caráter textual ou caracteres (ex: quando quero que a pessoa escreve algum nome)

- use o comando "faca" para iniciar repetição

- Use o comando "enquanto" para delimitar a repetição

  

  -------------------------------------------------------------------------------------------------------------------------------------

  

  ##### Exemplo 1: Comando escreva/leia (real e cadeia)

  

programa
{
	

	funcao inicio()
	{
		real janeiro,fevereiro,marco,abril,soma,media
		cadeia funcionario
		
		escreva ("digite o nome do funcionário:")
		leia(funcionario)
		escreva("Digite o valor das vendas de Janeiro:")
		leia(janeiro)
		escreva("Digite o valor das vendas de Fevereiro:")
		leia(fevereiro)
		escreva("Digite o valor das vendas de Março:")
		leia(marco)
		escreva("Digite o valor das vendas de Abril:")
		leia(abril)
	
		soma = (janeiro+fevereiro+marco+abril)
	
		media = (janeiro+fevereiro+marco+abril)/4
	
		escreva(" O funcionário " + funcionario + " obvete " + soma + " em vendas")
		escreva(" O funcionário " + funcionario + " obteve a media de vendas: " + media)
	}
}

-------------------------------------------------------------------------------------------------------------------------------------------

##### Exemplo 2: comando faça/enquanto

programa
{
	
	funcao inicio()
	{
		inteiro contador=0
		cadeia informacao [][]={{"João","8199713-8760","Recife-PE"},{"Rebeca","8799587-8866","São Paulo-SP"},{"Carla", "859955-9965","Goiania-GO"}}
	
		faca{
	
			escreva ("nome: " + informacao[contador][0] + " Telefone: " + informacao[contador][1] + " Cidade: " + informacao[contador][2] + "\n")
			contador ++


​			
		}enquanto(contador<=2)
	
	}
}

-------------------------------------------------------------------------------------------------------------------------------------------

##### Exemplo 03: Comando Se/Senao

// função: calcular média de vendas
// autor: Manuela Fernandes

programa
{
	
	funcao inicio()
	{
		real janeiro,fevereiro,marco,abril,soma,media
		cadeia funcionario
		
		escreva ("digite o nome do funcionário:")
		leia(funcionario)
		escreva("Digite o valor das vendas de Janeiro:")
		leia(janeiro)
		escreva("Digite o valor das vendas de Fevereiro:")
		leia(fevereiro)
		escreva("Digite o valor das vendas de Março:")
		leia(marco)
		escreva("Digite o valor das vendas de Abril:")
		leia(abril)
	
		soma = (janeiro+fevereiro+marco+abril)
	
		media = (janeiro+fevereiro+marco+abril)/4
	
		escreva(" O funcionário " + funcionario + " obvete " + soma + " em vendas")
		
		escreva("\n" + " O funcionário " + funcionario + " obteve a media de vendas: " + media)

// calcular média de vendas e verificar se é maior ou menor que R$ 5000
		se(media>=5000) {
			escreva("\n" + "Parabéns!! você receberá 5% sobre a comissão")
			
		}
	
		// caso a média seja menor que R$ 5000 recebe menos comissão
		
		se(media<5000) {
			escreva("\n" + "infelizmente você não atingiu a meta")
			
		}
	}
}

________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________

