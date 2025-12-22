# Anotações sobre a linguagem de programação C#.

## Anotações durante o estudo do treinamento em C# no Microsoft Learn e presquisas avulsas.

O C# funciona através do SDK .NET

Link para Download: https://dotnet.microsoft.com/pt-br/download

Comando para visualizar a versão do .NET instalado: 

`dotnet --version` / `dotnet --list-sdks`

Caso após a instalação do .NET o comando `dotnet --version` não esteja funcionando, seguir os seguintes passos: 

- Abrir a opções avançadas do computador usando os comando windows + R e digitar sysdm.cpl;
- Ir na aba Avançado;
- Selecionar a opção “Variáveis de Ambiente”;
- Na parte de Variáveis do sistema, selecionar a opção “Path” e clicar em “Editar”;
- Procurar pelo caminho “C:\Program Files\dotnet\” e verificar se na lista de caminhos não há nenhum outro caminho terminado com \dotnet\ que esteja acima do caminho informado;
- Caso haja, clique no primeiro caminho informado e depois clique em “Mover para Cima”;
- Salve tudo e reinicie o PowerShell ou CMD;
- O comando **dotnet --version não** é executado porque o PoweShell ou CMD estão encontrando mais de um caminho para execução do dotnet.exe. Devido a isso ocorre um conflito na hora da utilização da aplicação, sendo necessário a correção do Path nas Configurações Avançadas de Sistema. 

Extensões para o VS Code: 

- C# Dev Kit - microsoft.com
- C# - microsoft.com
- C# Extensions - JosKreativ

C# é uma linguagem com Case Sensitive. A linguagem faz diferença entre letras maiúsculas e minúsculas. Exemplo: Console.WriteLine(); ≠ console.writeline();

Para iniciar um novo console e criar um programa: 

`dotnet new console;`

Extensão do arquivo do C#: .cs;

Comando de print na tela: 

`Console.WriteLine()` & `Console.Write()`

- Diferença: **WriteLine** realiza uma quebra de linha para a próxima impressão na tela, já **Write** sem a presença do Line não faz essa quebra de linha. 

Comando para execução de arquivo por meio do terminal: `dotnet run;`

### Literais de caracteres: 

Aspas simples criam um caractere literal, um **char literal**. Ela vai aceitar apenas **um único** caractere. Já as aspas duplas criam um um dado do tipo **string**. Um valor literal é algo que não sofre altração, é um valor constante. 

Para a impressão de um caractere literal usa-se o comando: 

`Console.WriteLine('b')`

### Literais interiros

Comando para a coleta de uma informação que o usuário digitar: 

`Console.ReadLine()`

O **Console.ReadLine()** vai retornar uma informação em formato de String. Para converter uma String para algum tipo de valor numérico, usa-se o método Parse. Forma de aplicação: 

`nome-da-var = int.Parse(Console.ReadLine());`

A partir do console, a variável (nome-da-var) vai receber uma informação (ReadLine()) que será transformada em um tipo inteiro (int.Parse()).
