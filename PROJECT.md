## STATUS:

O código não realiza a função proposta pelo desafio.

## O QUE FOI REALIZADO:

O código utiliza a biblioteca Pandas para realizar a leitura do arquivo CSV.

Inicialmente é realizado o tratamento das colunas, eliminando elementos que possam impossibilitar operações entre as mesmas através da função '.apply', que retira "R$" e "h" das colunas que  informam respectivamente preço e tempo para entrega.

Posteriormente é realizado a conversão de alguns valores para possibilitar a utilização dos mesmos em operações através da função '.astype'

Notando algumas reptições de cidades de destino optei por agrupar as linhas pelas cidades e empresas com '.groupby', para obter uma melhor visualização.

## PROBLEMA/LIMITAÇÃO

Depois de realizar o '.groupby' a intenção era analisar o data frame pelos níveis do índice e por meio de testes condicionais eliminar as empresas que não atendecem as condições, ao final obtendo um novo data frame. 


