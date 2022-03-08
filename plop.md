
# Plop - Geração de componentes

## Descrição

Essa documentação demostra como criar um componente no projeto com Plop. O Plop é um lib que automatiza o chato trabalho de criar pastas e arquivos para nossos componentes.

## Uso

Para usar o Plop, você precisará certificar-se de instalar de forma global o plop na sua maquina:
```
npm install -g plop
```

Após isso, confirma que o seguinte script esteja no arquivo package.json:

```
"gen": "plop --plopfile ./generators/plopfile.mjs",
```
##  Como executar o script
---

### No terminal

Abra o terminal no projeto e digite:
```
npm run gen [NomeDoComponente]
```


*Se tudo deu certo, foi gerada uma nova pasta destro de components com o [NomeDoComponente].* 

### Erros comuns

*Se der erro e o mesmo for no sentido que o comando é inesistente ou não reconhecido, instale o plop globalmente novamente:*

```
npm install -g plop
```
*Não é possivel ter dois componentes com o mesmo nome, caso [NomeDoComponente] seja repetido os arquivos não serão criados.*

*Adicionamos validação para nomeação correta dos arquivos, estamos usando o padrão CamelCase.*


### Estrutura da pasta criada com o Plop

```

[NomeDoComponente]/                    # Root component.
|- index.tsx                           # Arquivo de exportação geral.
|- [NomeDoComponente].tsx              # Logica do component.
|- [NomeDoComponente].stories.tsx      # Configuração dos stories do component para o storybook.
|- [NomeDoComponente].styled.ts       # Arquivo de estilização do component com styled do mateial ui.
|- [NomeDoComponente].test.tsx         # Arquivo para testes unitários do componente.
|- [NomeDoComponente].type.tsx         # Arquivo de tipagem do componente.

```
 
 
 
## Documentação

-   [Plop](https://plopjs.com/) 

## Duvidas

-   Manda mensagem no grupo do skype
