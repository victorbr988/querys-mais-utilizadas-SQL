
# 📌 Funções mais usadas no SQL

Aqui você encontrará meu resumo sobre as funções
que mais são utilizadas para tratamento de dados.

## 👥 Authors

- [@Victor_Gabriel](https://www.github.com/victorbr988)
- [@Trybe](https://www.betrybe.com/)

## 📝 Documentation

[Documentação SQL](https://dev.mysql.com/doc/)

## 📜 Roadmap

### Manipulação de strings 

<details>
<summary>SELECT UCASE</summary>
<br>
Converte o texto da string para caixa alta
```javascript
	SELECT UCASE('oi, eu sou uma string');
```
</details> 

- SELECT LCASE() => Converte o texto da string para caixa baixa
    Exemplo SELECT LCASE('oi, eu sou uma string');

- SELECT REPLACE() => Substitui as ocorrências de umas substring em uma string
    Exemplo 
    SELECT REPLACE('oi, eu sou uma string', 'string', 'cadeia de caracteres');

- SELECT LEFT() => Retorna a parte ESQUERDA de uma string de acordo com a quantidade de caracteres especificados.
    Exemplo 
    SELECT LEFT('oi, eu sou uma string', 3);

- SELECT RIGHT() => Retorna a parte DIREITA de uma string de acordo com a 
    quantidade de caracteres especificados.
    Exemplo
    SELECT RIGHT('oi, eu sou uma string', 3);

- SELECT CHAR_LENGTH() => Exibe o tamanho, em caracteres, da string, a função LENGTH retorna o tamanho em bytes.
    Exemplo
    SELECT CHAR_LENGTH('oi eu sou uma string')

- SELECT SUBSTRING() => Extrai parte de uma string de acordo com o índice de um caractere inicial e a quantidade de caracteres a extrair, se a quantidade de caracteres a extrair não for definida, então a string será extraída do índice definido, até o seu final.
    Exemplo 
    SELECT SUBSTRING('oi eu sou uma string', 5, 2)
    SELECT SUBSTRING('oi eu sou uma string', 5)

### Condicionais IF, CASE

Sintaxe: SELECT IF (condição, valor_si_verdadeiro, valor_se_falso);

OBS: A condicional CASE é a mais adequada quando temos uma situação de múltiplas condições.

sintaxe:
CASE
	WHEN condição, THEN  valor_se_verdadeiro;
	WHEN condição, THEN  valor_se_verdadeiro;
	WHEN condição, THEN  valor_se_verdadeiro;
ELSE condição para falso

END AS nome_para_coluna => termina a query colocando essas condições dentro de uma coluna chamada valor

### Funções matemáticas

Além das tradicionais +, -, * e /. Temos também:

- DIV: retorna o resultado inteiro de uma divisão, ignorando as casas decimais de um número.

- MOD: retorna o resto de divisão como resultado.
    Exemplo:
    SELECT 10 MOD 3;

- ROUND: arrendoda os valores e permite também que você possa especificar quantas casa decimais quer, passando um número como segundo parâmetro.

- CEIL: arredonda os valores para o valor mais alto SEMPRE

- FLOOR: arredonda os valores para o valor mais baixo SEMPRE

- POW: recebe dois numeros por parâmetros e o segundo vira expoente do segundo

- SQRT: retorna a raiz quadrada de um número

- RAND: gera um valor aleatório entre 0 e 1

- ROUND: gera valores aleatórios entre números especificados
    Exemplo
    SELECT ROUND(7 + (RAND() * 6));
- AVG: retorna a média aritmética


