# SelectGroup 

Componente construido com Material Ui e customizado de acordo com nosso design system.

## Requisitos funcionais

- Deve ser possivel criar componentes de Select e MultiSelect que recebem Option como children, o estado e um renderValue.    
 

## Pasta no projeto
- src\components\SelectGroup/Select
- src\components\SelectGroup/MultiSelect
- src\components\SelectGroup/Option


## Guia de Desenvolvimento

### Uso

Existem páginas no projeto para pegar de base caso a documentação não seja o suficiente

Como implementar

Select

```js
import {
  SelectOption
} from '@mui/base';
import { Option } from 'components/SelectGroup/Option';
import { Select } from 'components/SelectGroup/Select';
import { default as React, useState } from 'react';


export function Exemplo() {

  const [selecionado, setSetSelecionado] = useState();

  function renderValue(option: SelectOption<number | string>) {
    if (option == null) {
      return <span>select an option...</span>
    }

    return <span>{option.label}</span>
  }
 

  return (
       <Select value={selecionado} renderValue={renderValue} onChange={(num) => num && setSetSelecionado(num)}>
        <Option value={10}>opção 1</Option>
        <Option value={20}>opção 2</Option>
        <Option value={30}>opção 3</Option>
      </Select> 
    )
}
```
 
MultiSelect

```js

import {
  SelectOption
} from '@mui/base';
import { MultiSelect } from 'components/SelectGroup/MultiSelect';
import { Option } from 'components/SelectGroup/Option';
import React, { useState } from 'react';


export function Exemplo() {
   const [selecionados, setSeleionados] = useState<(string | number)[]>([]);

    function rendervalue(option: SelectOption<string | number>[]) {
      if (option == null || option.length == 0) {
        return <span>select one or more options...</span>
      }
      return <span>{option.map(val => val.label).join(", ")}</span>
    } 

  return (
        <MultiSelect value={selecionados} onChange={(value: (string | number)[]) => setSeleionados(value)} renderValue={rendervalue}>
          <Option key={10} value={'10'}>opção 1</Option>
          <Option key={20} value={'20'}>opção 2</Option>
          <Option key={30} value={'30'}>opção 3</Option>
        </MultiSelect> 
        )
}
```

  
### Props

- Children 
- value
- onChange
- renderValue
 
**Nome e Tipo**
  
- Children: React.ReactNode 
- value: string | number)[] 
- onChange: string | number)[]) => void 
- renderValue: <string | number>[] 
 
