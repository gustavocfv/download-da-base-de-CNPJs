# download-da-base-de-CNPJs
Script em Python para realizar o download automatizado dos arquivos públicos da base de CNPJs brasileiros da Receita Federal.

Os arquivos que compõem a base de dados estão no link: https://www.gov.br/receitafederal/pt-br/assuntos/orientacao-tributaria/cadastros/consultas/dados-publicos-cnpj

O script lê o site da Receita e encontra os links para download dos arquivos. A célula 11 traz a definição da função que realiza o download de um arquivo. Nessa função, é preciso alterar a variável path com o caminho da pasta onde os arquivos serão salvos.

Após realizar o download, é preciso extrair os arquivos dos zips e renomeá-los acrescentando um ponto antes de CSV. Cada um dos 10 arquivos de cada categoria (EMPRESA, ESTABELECIMENTO, SÓCIOS) traz todas as linhas da base completa, mas apenas algumas colunas, com uma chave única (CNPJ BÁSICO) para realizar os joins entre os arquivos e gerar a tabela completa. Esse processo será automatizado numa segunda etapa.
