# Eventos-DIO
Aula prática, mostrando os Eventos em JS/HTML na prática!


# DOM (Document Object Model):

O DOM HTML é um padrão de como acessar e modificar os elementos HTML de uma página!


-----------------------------------------------------------------------------------

## Selecionando os Elementos de Uma Página:

Podemos usar o:

	 -> document.getElementById('id')
	// Devemos passar a ID como parâmetro, e obteremos como resultado toda a tag da ID

	 -> document.getElementsByTagName('TagName')
	// Devemos passar como parâmetro a TagName, e obteremos como retorno mais de uma TAG.
	Por isso, devemos usá-la quando precisamos de mais de um retorno de um mesmo tipo, como
	uma lista

	 -> document.getElementsByClassName('ClassName')
	// Retorna a classe inteira, do começo da tag até o seu fechamento


-----------------------------------------------------------------------------------

## Adicionar e Deletar Elementos:

document.createElement(element)      //      Cria um novo elemento HTML          
document.removeChild(element)        //	     Remove um elemento
document.appendChild(elemento)       //	     Adiciona um elemento
document.replaceChild(new, old)      //      Substitui um elemento


-----------------------------------------------------------------------------------

## Trabalhando com Estilos:

			   (HTML)

<div id = "meu-elemento" class = "classe">

</div>

			(CSS)

const meuElemento = document.getElementById("meu-elemento");

meuElemento.classList.add("novo-estilo");
// Adiciona a classe "novo-estilo"

meuElemento.classList.remove("classe");
// Remove a classe "classe", que está presente no código HTML

meuElemento.classList.toggle("dark-mode"); 
// Adiciona a classe "dark-mode", caso ela não exista hoje


-----------------------------------------------------------------------------------

## Acessando Diretamente o CSS de um Elemento:

document.ElementsByTagName("nomeDaTagName").style.color = "blue";


-----------------------------------------------------------------------------------

## Eventos:

mouseover: Ação ao passar o mouse sobre determinada parte da página.
mouseout: Ação ao tirar o mouse de determinada parte da página.
click: Ação ao clicar em determinada parte da página.
dbclick: Ação ao dar um clique duplo em determinada parte da página.
Change: Ação ao recarregar a página.
load: Ação ao terminar de recarregar a página.

	
	## Como Realizar um Evento:


## Diretamente no Javascript, cria um evento que vai ser acionado no momento em que o 
usuário realizar determinada ação. EXEMPLO:

const botao = document.getElementById("minhaId");
botao.addEventListener("click", outraFuncao);


## Diretamente no HTML, digite um evento. EXEMPLO:

<h1 onclick = mudaTexto(this)" Clique aqui! </h1>

<script>
	function mudaTexto(id) {
		id.innerHTML = "Mudei!";
	}
</script>


-----------------------------------------------------------------------------------

