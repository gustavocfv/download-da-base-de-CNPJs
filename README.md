# download-da-base-de-CNPJs
Script em Python para realizar o download automatizado dos arquivos públicos da base de CNPJs brasileiros da Receita Federal.

Os arquivos que compõem a base de dados estão no link: https://www.gov.br/receitafederal/pt-br/assuntos/orientacao-tributaria/cadastros/consultas/dados-publicos-cnpj

O script lê o site da Receita e encontra os links para download dos arquivos. A célula 13 traz um laço recorrente que baixa os arquivos para a máquina local: basta substituir o caminho da pasta para salvar na variável path.
