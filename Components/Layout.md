# Layout

Componente construido com Material Ui e customizado de acordo com nosso design system.

## Requisitos funcionais

- Nesse componente possui o Header e sidebar da plataforma.
- No header possui Dropdown com os blogs da empresa logada, trazendo dados de utilização do blog selecionado. Menu que direiona para telas: Meus dados, Gerenciar usuários, Gerenciar projetos, financeiro e deslogar da plataforma. Possui campo de notificações.
- Sidebar contém navegação com botões para as telas de Dashboard, Dicas de otimização, Ranking de palavras chave, Ajuda. Mostra o blog selecionado e os dados da quantidade de artigos atravéz de uma barra de progresso.

## Pasta no projeto
- src\components\Layout

## Guia de Desenvolvimento

### Uso

Como implementar

```js
import { Layout } from "components/Layout";

export function Exemplo() {
   return (
        <Layout>
            <Router />
            
        </Layout>
}
```
 
  
### Props

- Children 
- LayoutProps

**Nome e Tipo**
  
- Children: React.ReactNode 
 

