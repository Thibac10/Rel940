# Rel940

O REL940 trata-se de um shell para uso exclusivo de linha de comando (CLI). A forma como está implementado aqui apresenta comandos para criação de relatórios e chamadas de scripts externos com um visual limpo e "amigável". Esse shell foi criado para ser um centralizador de tarefas em lotes.

Os parâmetros aqui presentes estão apenas para exemplo. Com certeza esses serão alterados/adaptados para seu uso.

A execução do shell é simples, e possui apenas dois parametros adicionais de execução:

## Execução:

user@machine # 
```rel940.sh -noemail -noprint```

`-noemail` : Executa o shell sem o envio de e-mails.

`-noprint` : Executa o shell sem impressões de relatórios.


Vamos então ao processo de instalação:

## Instalação

A instalação é simples e requer apenas que seja configurado os arquivos e diretórios declarados na área de VARIÁVEIS marcados como `CONFIG` no início do shell rel940. Como mencionado anteriormente, tudo aqui será adaptado de acordo com a necessidade de quem estiver implementando.

#### Sugestão de Estrutura de Diretórios:

**DIRETÓRIO RAIZ:**

```
- rel940.sh           (shell principal para execução)
- modules             (diretório onde ficam os módulos do rel940)
- log                 (diretório de logs)
- temp                (diretorio para processamento temporário)
- mail                (diretório com textos para envio por e-mail)
- relatorios_diarios  (diretório destino dos relatórios gerados)
- imprimir            (diretório onde serão armazenados os documentos que foram impressos)
```

![Exemplo de Estrutura](Exemplo_de_Estrutura.png)

## Prints:

- Print 1
  
![Execução 01](prints_de_execucao/execucao_01.png)

- Print 2

![Execução 02](prints_de_execucao/execucao_02.png)

- Chamada de Shell / Comando Externo
  
![Execução 01](prints_de_execucao/chamada_shell_externo.png)

- Tela de Lançamento de dados da Planilha Geral
  
![Execução 02](prints_de_execucao/lancamento_dados_planilha_geral.png)

- Tela para verificação dos dados lançados
![Execução 01](prints_de_execucao/atualizacao_planilha_geral.png)

- Tela de finalização do Shell
![Execução 02](prints_de_execucao/tela_de_finalizacao.png)
