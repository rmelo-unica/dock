# DataGrid 

Componente construido com Material Ui e customizado de acordo com nosso design system.

## Requisitos funcionais

- Deve ser possivel criar uma datagrid (tabela) com filtro, ordenação, pesquisa e ações. 
- A listagem da tabela deve ser páginada e responsiva.


## Pasta no projeto
- src\components\DataGrid 

## Guia de Desenvolvimento

### Uso

Como implementar

```js
import { Card } from "components/Card";

export function Exemplo() {

    const { data } = useExemplo(Exemplo);
    
      const columns: GridColDef[] = [
        {
            field: 'titulo',
            headerName: 'Título',
            description: 'Título do artigo',
            type: 'text',
            flex: 5.5,
            minWidth: 300
        },
        {
            field: 'autor',
            headerName: 'Autor',
            description: 'Autor do artigo',
            flex: 2.5,
            minWidth: 100
        } 
    ];

    return (
      <DataGrid
          data={data}
          columns={columns}
          filterableFields={["titulo"]}
          hasSearchBox
          hasPagination
      />
    )
}
```
 

  
### Props

- Children 
- CardProps [Leia mais](https://mui.com/pt/components/cards/)

**Nome e Tipo**
  
- Children: React.ReactNode 
- data: T[];
- columns: GridColDef[];
- hasSearchBox?: boolean;
- hasPagination?: boolean;
- filterableFields?: Array<keyof T>;
- refreshHandler: () => void;
- editHandler?: (id: number) => void;
- removeHandler?: (id: number) => void;
  
*** Veja demais props no arquivo DataGrid.types.ts do componente
  
**** No projeto temos a implementação em algumas páginas.
