# Ambiente de Desenvolvimento

Para o desenvolvimento do nosso código gráfico, usaremos a biblioteca OpenGL por intermédio do OpenTK, com a linguagem C# (SDK .NET) e a IDE VSCode.  

## SDK .NET

O primeiro passo é instalar o SDK do .NET Core para poder programar na linguagem C#.  

> [!WARNING]  
> Iremos usar a versão: .NET 10.0  
<https://www.microsoft.com/net/download>  

### Testar o SDK .NET

Para os passos a seguir, é possível utilizar o prompt do Windows (`cmd`), o terminal do macOS ou o próprio terminal do [VSCode](#ide-vscode).  
Crie uma nova pasta que será o diretório do projeto OpenTK no VSCode e navegue até ela. Neste exemplo, o nome da pasta será `OlaMundo`:  

```console
mkdir OlaMundo
cd OlaMundo
```

Em seguida, crie uma `Console Application` nessa pasta:  

```console
dotnet new console
```

Nesse ponto, um novo arquivo `Program.cs`, contendo um método `main`, é criado. Para executar o projeto, digite:  

```console
dotnet run
```

Se o projeto foi criado corretamente, após a sua execução, deve aparecer a mensagem `Hello, World!` no terminal.  
Observe que foram criados dois arquivos no projeto:  

- OlaMundo.csproj  
- Program.cs  

E as pastas:

- bin  
- obj  

## IDE VSCode

O segundo passo é instalar a IDE VSCode (ou outra de sua escolha).  

<https://code.visualstudio.com/>  

Não esqueça também de instalar a extensão para C# <https://marketplace.visualstudio.com/items?itemName=ms-dotnettools.vscode-dotnet-runtime> e estas extensões:

- C# Dev Kit: <https://marketplace.visualstudio.com/items?itemName=ms-dotnettools.csdevkit>  
- IntelliCode for C# Dev Kit: <https://marketplace.visualstudio.com/items?itemName=ms-dotnettools.vscodeintellicode-csharp>  

Se necessário, há mais informações sobre extensões do VSCode em: [https://code.visualstudio.com/docs/editor/extension-gallery](https://code.visualstudio.com/docs/editor/extension-gallery "https://code.visualstudio.com/docs/editor/extension-gallery")  

As extensões que eu uso podem ser vistas em: <https://github.com/dalton-reis/dalton-reis/blob/main/_._/VSCode/VsCodeExtensoes.md>  

### Testar o VSCode

Para testar a IDE VSCode, abra o projeto criado.  

## Toolkit OpenTK

O terceiro passo é fazer com que o projeto criado use as dependências do Toolkit OpenTK (para usar o OpenGL no C#):  

```console
dotnet add package OpenTK --version 4.9.4
```

### Testar o OpenTK

Nesse ponto, para testar se o OpenTK está funcionando, acrescente a linha `using OpenTK;` no cabeçalho da classe do arquivo `Program.cs`:  

```csharp
using OpenTK;
```

Se nenhum erro ocorrer, o OpenTK já estará disponível para uso.  
Caso ocorra algum erro de `undefined command`, tente executar o comando no terminal para recarregar as dependências do projeto:  

```console
dotnet restore
```

## ⏭ [Unidade 2](../Unidade2/README.md "Unidade 2")  
