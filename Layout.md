# Layout

Componente construido com Material Ui e customizado de acordo com nosso design system.

## Requisitos funcionais

- Nesse comonente possui o Header e sidebar da plataforma. No header possui Dropdown com os blogs daquela empresa, notificações, botão que direciona para telas Meus dados, Gerenciar usuários, Gerenciar projetos, 

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
 

