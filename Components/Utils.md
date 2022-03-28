# Utils

Componente construido com Material Ui e customizado de acordo com nosso design system.

## Requisitos funcionais
- Deve ser possivel criar componentes de Acesso negado e Nao Encontrado.

## Pasta no projeto
- src\components\Utils

## Guia de Desenvolvimento

### Uso

Como implementar

```js
AcessoNegado

import AcessoNegado from "components/Utils/AcessoNegado";

if (!token) return <AcessoNegado />;

NaoEncontrado 

import NaoEncontrado from "components/Utils/NaoEncontrado";

const DeslogadoRoute: React.FC = () => {
    return (
        <Switch>
            <Route path="*" component={NaoEncontrado} />
        </Switch>
    );
};


```
  
### Props


**Nome e Tipo**



