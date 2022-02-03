Otavio Reis: WEB Developer e instrutor na <https://education.github.com/experts> também.

Introdução o Git e Github - pontos em destaque.

**\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_**

# **1.Introdução ao GIT**

## 1.1 Entendendo o que é Git e sua importância.

` `O GIT foi criado em 2005 por linus Torvalds, é um sistema de versionamento de código distribuído. GIT (opensource) e Github(podem ter planos pagos) são tecnologias diferentes mas complementares.

` `Bitbucket

` `BItkeeper

` `CVS


### 1.1.1 Benefícios de aprender ambas tecnologias juntas:

- Controle de versão.
- Armazenamento em nuvem
- Trabalho em equipe
- Melhorar seu código
- Reconhecimento.


**\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_**
# **2. Navegação via command line interface e instalação**


## **2.1. Comandos básicos para um bom desempenho no terminal**

- **GUI (Graphic User interface) vs CLI(Command line interface):**

**O Que vamos aprender a fazer?**

- Mudar de pasta
- Listar as pastas
- Criar pastas/arquivos
- Deletar pastas/arquivos



**Windows derivado do shell**

- **cd** - “change directory” vai para a base do diretório comando cd ou cd/ windows para entrar na pasta e pode consultar as pastas abaixo. **cd..** retrocede.
- **dir** - abreviação de diretório listar (comando dentro do terminal “cmd”) lista todas os diretorios no lixux é **ls.**
- **mkdir -** cria um novo diretório (criar workspace)
- **rmdir -** apaga pasta assim: >rmdir nomedodiretorio /S /Q (Significado de flags S e Q?)
- **tab -** autocompleta
- **cls - “**clearscreen” limpa a tela linux ctrl+L
- **del -** deleta apenas arquivos

“silence on success” terminal não retornou nada é sinal que deu certo

- **>echo** funciona assim: >echo nome do arquivo > nomedoarquivo.tipodoarquivo cria um arquivo no formato indicado



**Linux derivado do bash**

- cd
- ls
- mkdir
- rm -rf

## **2.1. Realizando a instalação do Git.**
No windows:

Baixar o git no site do Git diretamente.

- verificar se as opções “Git Bash Here” e “Git GUI Here”.
- mantém o Vim como editor mesmo.
- Deixar o Git decidir “Master”.
- Git Credential Manager Core.

Se quiser aprender para linux Ubuntu voltar no minuto 9:00 do video.

\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_
# **3. Entendendo como o GIT funciona por baixo dos panos**

- **SHA1** - Secure Hash Algorithm - é um conjunto de funções hash critptográficas projetadas pela NSA (Agência de Segurança Nacional dos EUA);

` `**Puxar no minuto 8:00 aplicação e colar aqui**

## **3.1 Objetos Internos do Git**
- **Objetos fundamentais** - Blobs contém metadados (tipo, tamanho e conteúdo)(echo ‘conteúdo’ | git hash-object no git retorna o Sha1 da sting (gera 1 tipo de objeto **min 1:15 e corrigir**)ou echo -e  'conteúdo’ | open ssl sha1 (gera outro tipo) para gerar o mesmo  echo -e  'blob 9\0conteúdo’ | open ssl sha1 (gera outro tipo) ) , tree também contém metadados e guarda o nome do arquivo e monta uma estrutura apontando para outras árvores e blobs, e commits junta todos os objetos anteriores e carimbo de tempo(buscar como verificar o histórico).


- **Sistema Distribuído** - Disponibilidade para varias maquinas.
- **Segurança** -  Em versões confiaveis.

## **3.2 Chave SSH e Token**

Chave SSH - é uma conexão criptografada, precisa configurar com o CLI com Git bash.



**\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_**
# **4. Primeiros comandos com Git.**

## **4.1 Iniciando o Git e criando uma commit**.



- **Iniciar o Git** - Git init - A pasta .git não aparece por ser uma pasta gerencial oculta. A flag **“-a”** exibe no git bash essa pasta oculta. 
- Arquivos **Markdown** são uma forma mais humana de escrever artigos html. A quantidade de # indica o “ h”, ex: h1=#; h2=##, h3=### … Nome do arquivo é nomedoarquivo.md (ele usa o Typora para editar na ajuda há uma referência).

` `\*\*texto\*\* fica em negrito

- **Iniciando o versionamento** - Git add -  **git add \* (com asterisco cobre todos os arquivos da pasta).**
- **Criando um commit** - Git commit - **git commit -m "commit inicial"**

![](Aspose.Words.a06ff966-755b-4793-a70c-684236fc4255.001.png)

**\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_**
# **5. Ciclo de vida dos arquivos no Git.**
##
## **5.1 Passo a passo no ciclo de vida**

**Git init cria um repositório -**  tracked e untracked.

- git add move direto para staged
- se modificar depois disso ele sai de unmodified para modified. Se der um add vai direto para staged de novo.
- se nao modificar e remover volta para untracked.
- staged prepara para o commit.
- o commit retorna para o unmodified.

![](Aspose.Words.a06ff966-755b-4793-a70c-684236fc4255.002.png)

**git add**

![](Aspose.Words.a06ff966-755b-4793-a70c-684236fc4255.002.png)

**verificação de status, criação de nova pasta e movimentação do arquivo:**

![](Aspose.Words.a06ff966-755b-4793-a70c-684236fc4255.002.png)


**Arquivo adicional para indexar**


![](Aspose.Words.a06ff966-755b-4793-a70c-684236fc4255.003.png)

\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_
# **6. Introdução ao GIThub**
##
## **6.1 Trabalhando com o GitHub**


![](Aspose.Words.a06ff966-755b-4793-a70c-684236fc4255.004.png)

\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_
# **7. Resolvendo conflitos**
##
## **7.1 Como os conflitos acontecem no GitHub e como resolvê-los**

` `2 pessoas alterando o código na mesma linha geralmente causa problemas.  O GitHub fala para o último a subir na mesma linha para 

` `**Mensagem de conflito:**

![](Aspose.Words.a06ff966-755b-4793-a70c-684236fc4255.005.png)

**A solução com caso é utilizar o comando “pull” para puxar no caso abaixo ao fazer isso deu um erro de merge:**

![](Aspose.Words.a06ff966-755b-4793-a70c-684236fc4255.006.png)

**Aponta um arquivo que você não tem localmente. Por isso o conflito. Em branco ele está puxando o arquivo faltante para alterar manualmente. verificação com Typora e bloco de notas. no head é a mais recente.  dos iguais para baixo a versão que estava no github.** 


![](Aspose.Words.a06ff966-755b-4793-a70c-684236fc4255.007.png)

**pode apagar o que ele fez a princípio e depois colocou abaixo** 

![](Aspose.Words.a06ff966-755b-4793-a70c-684236fc4255.008.png)

**conflito de dois arquivos modificados - both modified**

![](Aspose.Words.a06ff966-755b-4793-a70c-684236fc4255.009.png)

**colocando a versão final com a resolução do conflito**

![](Aspose.Words.a06ff966-755b-4793-a70c-684236fc4255.010.png)

**Como baixar um código um repositório do github para o local.  conferindo o repositório**

![](Aspose.Words.a06ff966-755b-4793-a70c-684236fc4255.011.png)

**para clonar um código basta copiar aquela url e usar o comando - git clone**

![](Aspose.Words.a06ff966-755b-4793-a70c-684236fc4255.012.png)

**opções de download direto**

![](Aspose.Words.a06ff966-755b-4793-a70c-684236fc4255.013.png)
