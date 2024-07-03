# Download de anexos da coluna do tipo ‘Arquivo’ do Dataverse a partir de um aplicativo em Power Apps

Olá pessoal, no artigo de hoje mostrarei um jeito simples e prático de como podemos recuperar o conteúdo da coluna do tipo ‘File’ do Dataverse para exibir e efetuar o download a partir de um aplicativo em Power Apps. Neste exemplo será utilizado um aplicativo do tipo Canvas.

No nosso cenário já temos uma tabela criada no Dataverse com alguns dados preenchidos.

![Imagem 1: Tabela Documentos](https://media.licdn.com/dms/image/D4D12AQHRHIpKEXCoZg/article-inline_image-shrink_1500_2232/0/1676154138026?e=1725494400&v=beta&t=6KMLnnCFxLFFX72dm_vFDI4yDM2v2ynjjOSduosur4Y)

Criaremos uma galeria para exibir os documentos e adicionaremos um controle de anexo. Para isso adicione um formulário na sua tela e defina a tabela que contem os arquivos como fonte de dados deste formulário, assim conseguiremos obter a coluna de controle de anexos, copiar e inserir dentro da nossa galeria.

![Imagem 2: Galeria de Documentos](https://media.licdn.com/dms/image/D4D12AQEcw1VEIlnMwg/article-inline_image-shrink_1500_2232/0/1676154205053?e=1725494400&v=beta&t=TQxhesF9nHUMGCnqJCiFPukRwVl6438OkfTc0n_7uNo)

![Imagem 3: Galeria com o controle de anexos ](https://media.licdn.com/dms/image/D4D12AQFAnlQa47OwGw/article-inline_image-shrink_1500_2232/0/1676154346945?e=1725494400&v=beta&t=nD-z7yCezB7QytNkRPo_ydsGWlRyFadIJDsaAFJEH7Y)

Na aba avançado do controle de anexo, iremos definir a propriedade 'Items' com a seguinte fórmula:

![Imagem 4: Fórmula da propriedade 'Items'](https://media.licdn.com/dms/image/D4D12AQFH59vnZJz7MA/article-inline_image-shrink_1500_2232/0/1676154834880?e=1725494400&v=beta&t=feDbKatCarWLhap4ZGpGOuG1Pk6PHWAUSxtS2TSChYc)

Ainda na aba avançado do controle de anexo, iremos definir as propriedades 'Name' e 'Value' com a seguinte fórmula:

![Imagem 5: Propriedades 'Name' e 'Value'](https://media.licdn.com/dms/image/D4D12AQEAQQVTc0TJiQ/article-inline_image-shrink_1500_2232/0/1676154946177?e=1725494400&v=beta&t=wJgesyWGrL1BMuPuHyHvxi1-jYrCrXHaUBZHG2V4i3U)

Muito importante definir estas propriedades acima, pois por padrão ambos os campos veem com o valor 'DisplayName' e se o 'Value' não for alterado, irá retornar o seguinte erro:

![Imagem 6: Mensagem de erro](https://media.licdn.com/dms/image/D4D12AQE_6IQYc2DJBQ/article-inline_image-shrink_1500_2232/0/1676155219788?e=1725494400&v=beta&t=yFJ0hE_HfT7jPFEzcLPAcy5pZycD-5aXvJuHhQF5RhQ)

Feito todo o procedimento acima basta apenas clicar no ícone ou nome do arquivo na galeria que o download irá iniciar.

![Imagem 7: Download do arquivo](https://media.licdn.com/dms/image/D4D12AQH81GvFLATAnw/article-inline_image-shrink_1500_2232/0/1676155359365?e=1725494400&v=beta&t=nMMU3d3yed09jU8dpKMJHFIVa_Cmu128O8V5AbJuOlM)
