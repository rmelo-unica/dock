
# Logo

Componente construido com Material Ui e customizado de acordo com nosso design system.

## Requisitos funcionais
- Deve ser possivel adicionar o Logo do projeto.

## Pasta no projeto
- src\components\Logo

## Guia de Desenvolvimento

### Uso

Como implementar

```js
import { Logo } from "components/Logo";

export function Exemplo() {
   return (
      <Logo variant="dark" size="sm" />
}
```
 
  
### Props

- variant
- size 
- className
- LogoProps

**Nome e Tipo**
  
- Children: React.ReactNode 
- variant: "dark" | "light";
- size?: "sm" | "md" | "lg";
- className?: string;
 

