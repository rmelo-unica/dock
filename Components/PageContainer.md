
# PageContainer 

Componente que engloba uma página e add a margin padrão em relação ao header e ao sidebar. 

## Requisitos funcionais

- Quando add PageContainer englobando o tsx da página a mesma deve ficar alinhada igual as demais.

## Pasta no projeto
- src\components\PageContainer

## Guia de Desenvolvimento

### Uso

Como implementar

```js
import { PageContainer } from "components/PageContainer";

export function Exemplo() {
    return (
      <PageContainer>
          // TSX da página 
      </PageContainer >
    )
}
```
 

  
### Props

- Children 
 
**Nome e Tipo**
  
- Children: React.ReactNode 
 
