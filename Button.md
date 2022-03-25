# Button 

Componente construido com Material Ui e customizado de acordo com nosso design system.

## Requisitos funcionais

- Deve ser possivel criar um botão e passar texto e/ ou icones atráves de prop. Este componente herda props de ButtonProps que tras tipagem das funções onChange, OnClick e muitos outros. 

## Pasta no projeto
- src\components\Button

## Guia de Desenvolvimento

### Uso

Como implementar

```js
import { AvatarPerfil } from "components/AvatarPerfil";

export function Exemplo() {
    return (
      <Button onClick={onClose}>
          Texto
          <Icone />
      </Button >
    )
}
```
 

  
### Props

- Children 
- ButtonProps [Leia mais](https://mui.com/pt/components/buttons/)

**Nome e Tipo**
  
- Children: React.ReactNode 
 
