# PageTitle 

Componente que recebe como children o h1 de uma página e add a barrinha amarela ou azul antes do texto ("| Titulo 1") . 

## Requisitos funcionais

- Deve ser possível passar um texto como children e este receber o estilo e a "barrinha"

## Pasta no projeto
- src\components\PageTitle

## Guia de Desenvolvimento

### Uso

Como implementar

```js
import { PageTitle } from "components/PageTitle";

export function Exemplo() {
    return (
      <PageTitle>
          Titulo 
      </PageTitle >
    )
}
```
 

  
### Props

- Children 
 
**Nome e Tipo**
  
- Children: React.ReactNode 
 
