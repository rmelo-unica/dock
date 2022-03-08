
# Plop - Geração de componentes

## Descrição

Essa documentação demostra como criar um componente no projeto com Plop. O Plop é um lib que automatiza o chato trabalho de criar pastas e arquivos para nossos componentes.

## Uso

Para usar o Plop, você precisará certificar-se de instalar de forma global o plop na sua maquina:
```
npm install -G plop
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


### Estrutura da pasta criada com o Plop


```
MyComponent/                    # Root component.
|- index/        				# Arquivo de exportação geral.
|- MyComponent.tsx      		# Logica do component.
|- MyComponent.stories.tsx      # Configuração dos stories do component para o storybook.
|- MyComponent.styled.tsx 		# Arquivo de estilização do component com styled do mateial ui.
|- MyComponent.test.tsx			# Arquivo para testes unitários do component..
```
 
 
## Documentação

-   [Plop](https://plopjs.com/) 

## Duvidas

-   Manda mensagem no grupo do skype
