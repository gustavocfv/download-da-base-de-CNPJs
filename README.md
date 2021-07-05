# download-da-base-de-CNPJs
Script em Python para realizar o download automatizado dos arquivos públicos da base de CNPJs brasileiros da Receita Federal.

Os arquivos que compõem a base de dados estão no link: https://www.gov.br/receitafederal/pt-br/assuntos/orientacao-tributaria/cadastros/consultas/dados-publicos-cnpj

O script lê o site da Receita e encontra os links para download dos arquivos. A célula 11 traz a definição da função que realiza o download de um arquivo. Nessa função, é preciso alterar a variável path com o caminho da pasta onde os arquivos serão salvos.

Após realizar o download, é preciso extrair os arquivos dos zips e renomeá-los acrescentando um ponto antes de CSV. Cada um dos 10 arquivos de cada categoria (EMPRESA, ESTABELECIMENTO, SÓCIOS) traz parte das linhas da base completa, e todas as colunas (sem cabeçalho), o que siginifica que é possivel juntá-los numa base única através de um append (embora seja necessária muita memória, principalmente para as bases de ESTABELECIMENTOS - estou estudando uma forma de exportar isso para o formato de  banco de dados). Os layouts das bases podem ser acessados aqui: https://www.gov.br/receitafederal/pt-br/assuntos/orientacao-tributaria/cadastros/consultas/arquivos/NOVOLAYOUTDOSDADOSABERTOSDOCNPJ.pdf. Esse processo será automatizado num segundo projeto.
