# Aplicação de Cálculo de Impostos

Este projeto em C# demonstra uma aplicação simples de cálculo de impostos que processa clientes individuais e clientes jurídicos. A aplicação calcula e exibe o valor do imposto e o valor total a ser pago pelos clientes com base nos valores das compras.

## Arquivos

### `Clientes.cs`

A classe `Clientes` serve como classe base tanto para clientes individuais quanto para clientes jurídicos. Ela define propriedades como `Nome`, `Endereco`, `Valor` (Valor da Compra), `Valor_imposto` (Valor do Imposto) e `Total`. A classe também contém um método virtual `Pagar_Imposto` que calcula o valor do imposto e o valor total a ser pago com base no valor da compra fornecido.

### `Pessoa_Juridica.cs`

A classe `Pessoa_Juridica` estende a classe `Clientes` e representa um cliente jurídico. Ela introduz propriedades como `Cnpj` (Número de Registro da Empresa) e `Ie` (Número de Inscrição Estadual). O método `Pagar_Imposto` nesta classe substitui o método da classe base para calcular o imposto de forma diferente para pessoas jurídicas.

### `Pessoa_Fisica.cs`

A classe `Pessoa_Fisica` também estende a classe `Clientes` e representa um cliente individual. Ela introduz propriedades como `cpf` (Número de Identificação de Pessoa Física) e `rg` (Número do Documento de Identidade).

### `Program.cs`

A classe `Program` contém o método `Main`, que é o ponto de entrada da aplicação. Ela solicita ao usuário informações sobre o cliente, incluindo se é uma pessoa física ou jurídica. Dependendo do tipo de cliente, o programa cria dinamicamente uma instância de `Pessoa_Fisica` ou `Pessoa_Juridica`. Em seguida, coleta informações adicionais específicas para o tipo de cliente e calcula o valor do imposto e o valor total usando o método `Pagar_Imposto` sobrescrito. Por fim, exibe todas as informações relevantes sobre o cliente e os detalhes do pagamento.

## Como Usar

1. Clone o repositório para sua máquina local.
2. Abra o projeto em seu ambiente de desenvolvimento C# preferido.
3. Compile e execute a aplicação.
4. Siga as instruções na tela para inserir as informações do cliente e os valores das compras.
5. A aplicação exibirá o valor do imposto e o valor total calculado para o cliente fornecido.

Sinta-se à vontade para explorar e modificar o código para personalizar ainda mais a aplicação de acordo com suas necessidades.

## Instalação do .NET e Dependências

Para executar a aplicação, você precisará do .NET Core SDK instalado em sua máquina. Siga estes passos:

1. Faça o download e instale o .NET Core SDK apropriado para seu sistema operacional a partir do site oficial da Microsoft: [Download .NET](https://dotnet.microsoft.com/download)

2. Clone este repositório para sua máquina local usando o Git:

git clone [https://github.com/seu-usuario/seu-repositorio.git](https://github.com/DevHefesto/Aplicacao-de-calculo-de-imposto)https://github.com/DevHefesto/Aplicacao-de-calculo-de-imposto

3. Navegue até o diretório do projeto:

```cd nome-do-projeto```

4. Execute o seguinte comando para restaurar as dependências:

```dotnet restore```

5. Compile o projeto:

```dotnet build```

6. Execute a aplicação:

```dotnet run```

## Tecnologias Utilizadas

- Linguagem: C#
- Plataforma: .NET Core
- Frontend: HTML, CSS
- IDE Recomendada: Visual Studio, Visual Studio Code

Lembre-se de que este projeto é um exemplo básico e pode ser expandido com mais recursos e funcionalidades, conforme necessário.