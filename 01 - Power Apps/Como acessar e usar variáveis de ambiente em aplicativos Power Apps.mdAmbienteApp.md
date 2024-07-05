# Como acessar e usar variáveis de ambiente em aplicativos Power Apps

Olá pessoal, no artigo de hoje mostrarei um jeito simples e prático de como podemos acessar as variáveis de ambiente a partir de um aplicativo em Power Apps. Neste exemplo será utilizado um aplicativo do tipo Canvas.

No nosso cenário já temos a variável de ambiente criada na solução.

![Imagem 1: Tabela Documentos](https://media.licdn.com/dms/image/D4D12AQE78Af7KVnlSA/article-inline_image-shrink_400_744/0/1718395974628?e=1725494400&v=beta&t=2o1sSjCThhpVIYl-fErSbhO3z_UXfVef8ZzFvcSZx40)

Dentro do aplicativo precisaremos adicionar a seguinte conexão:

![Imagem 2: Tabela Documentos](https://media.licdn.com/dms/image/D4D12AQGTQ73OgCUNJQ/article-inline_image-shrink_400_744/0/1718396116188?e=1725494400&v=beta&t=2hwph0yc_MvBGTA7CkC3D-o198UWUulzu0h-IFPAXyQ)

E para acessar o valor desta variável, usaremos a seguinte fórmula:

# LookUp('Environment Variable Definitions'; 'Schema Name'="cpq_varStorage").'Default Value'

Após aplicado a fórmula, conseguimos acessar o valor desta variável seja para armazenar em variáveis locais ou globais, campos de texto e etc.

Mais detalhes sobre as variáveis de ambiente podem ser obtidos na documentação da Microsoft.
