<h1 align="center"> Padrão de estilo de código com Python </h1>
<p align="left">🚀 Neste github procuramos estabelecer um padrão nos códigos em Python
que iremos utilizar,  iremos apresentar alguns exemplos porem no final desse documento criamos algumas referências que podem auxiliar a sanar possíveis dúvidas que possam ocorrer.</p>

<h2 align="left"> Nome de variáveis e constantes </h2>

<h3 align="left"> 
    Variáveis
</h3>
<ol>
    <li> Nome todo em minúsculo.</li>
    <li> Utilização de snake case.</li>
    <li> Nome deve ser auto explicativo.</li>
</ol> 

```
    messages_lower_case = ['mensagem um', 'mensagem dois', 'mensagem quatro']
    number_messages = 3
```

<h3 align="left"> 
    Constantes
</h3>
<ol>
    <li> Nome todo em maiúsculo.</li>
    <li> Utilização de snake case.</li>
    <li> Nome deve ser auto explicativo.</li>
</ol> 

```python
DB_MESSAGE = 'https://banco-message'
URL_REQUEST_IMAGE = 'https://banco-images'
```

<h3 align="left"> 
    Funções
</h3>
<ol>
    <li> Nome todo em minúsculo.</li>
    <li> Utilização de snake case.</li>
    <li> Nome deve ser auto explicativo.</li>
    <li> As variáveis devem estar tipadas.</li>
    <li> A saida da função deve estar tipadas.</li>
    <li> Deve ser utilizado docstring para documentar a funções.</li>
</ol>

```python
def soma_dois_inteiros(inteiro_a:int, inteiro_b:int)->int:
    """ Função que realiza a soma de dois números inteiros.
        Args:
            numero_a: primeiro números inteiro da soma.
            numero_b: segundo números inteiro da soma.
        Returns:
            resultado: soma dois números inteiros.
        Raises:
            raise: formato de dados invalidos.
    """
    if type(inteiro_a) != int or type(inteiro_b) != int:
        raise Exception("Formato de dados invalidos")

    return inteiro_a + inteiro_b
```

<h2 align="left"> Referencias </h2>

<p align="left"> 
    <a href="https://realpython.com/python-pep8/">🔗 How to Write Beautiful Python Code With PEP 8</a>
</p>

<p align="left"> 
    <a href="https://www.python.org/dev/peps/pep-0008/">🔗 PEP 8 -- Style Guide for Python Code</a>
</p>

<p align="left">
    <a href="https://www.youtube.com/watch?v=yEighFc_bZM&t=2145s">🔗 Live de Python #84 -Type Hints e anotações de funções</a>
</p>