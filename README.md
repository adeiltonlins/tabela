# tabela
SELECT CODIGO, NOME FROM CLIENTES
WHERE CODIGO = 10
SELECT CODIGO, NOME FROM CLIENTES
WHERE UF = ‘RJ’
SELECT CODIGO, NOME FROM CLIENTES
WHERE CODIGO >= 100 AND CODIGO <= 500
SELECT CODIGO, NOME FROM CLIENTES
WHERE UF = ‘MG’ OR UF = ‘SP’
SELECT CLIENTES.CODIGO, CLIENTES.NOME, PEDIDOS.DATA
FROM CLIENTES, PEDIDOS
SELECT A.CODIGO, A.DESCRICAO, B.DESCRICAO
FROM PRODUTOS A JOIN COMPONENTES B
ON (A.CODIGO = B.CODPRODUTO)
WHERE A.CATEGORIA = 1 OR A.CATEGORIA = 2
ORDER BY A.CATEGORIA, A.DESCRICAO
WHERE CLIENTES.CODIGO = PEDIDOS.CODCLIENTE
