

# Plop - Geração de componentes

## Descrição

Essa documentação demostra como criar um componente no projeto com Plop. O Plop é um lib que automatiza o chato trabalho de criar pastas e arquivos para nossos componentes.

## Uso

Para usar o Plop, você precisará certificar-se de que a dependência esteja no package.json do sistema.

### Estrutura da pasta criada com o Plop


```
MyComponent/                   # Root do componente.
|- index/        			         # Arquivo de exportação geral.
|- MyComponent.tsx      		   # Logica do componente.
|- MyComponent.stories.tsx     # Configuração dos stories do componente para o storybook.
|- MyComponent.styled.tsx 		 # Arquivo de estilização do componente com styled do mateial ui.
|- MyComponent.test.tsx			   # Arquivo para testes unitários do componente.
|- MyComponente.types.ts       # Arquivo de tipagens do componente.

```

Como executar o script
---

### No terminal

Abra o terminal no projeto e digite:

```
npm run gen [NomeDoComponente]
```
*Se tudo deu certo, foi gerada uma nova pasta destro de components com o [NomeDoComponente].*
 
## Documentação

-   [Plop](https://plopjs.com/) 

## Duvidas

-   Manda mensagem no grupo do skype
