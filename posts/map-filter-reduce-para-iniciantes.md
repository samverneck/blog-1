

## Iniciantes

```js
const NUMEROS = [1, 2, 3, 4, 5, 6, 7, 8, 9]

const mapear = (arr, fn) => arr.map(fn)

const elevadoAoQuadrado = (num) => num * num
const elevadoAoCubo = (num) => num * num * num
const posicoes = (num, posicao) => {
  if (posicao % 2 === 0) return 'posição par: ' + posicao
  else return 'posição ímpar: ' + posicao
}
const andaUmaPosicao = (num, posicao) => {
  if (posicao === 0) return NUMEROS[posicao+1]
  if (posicao !== NUMEROS.length-1 && posicao > 0) return NUMEROS[posicao+1]
  else return NUMEROS[0]
}
// Em uma linha com IF ternário
//const posicoes = (num, posicao) => (posicao % 2 === 0) ? `posição par: ${posicao}` : `posição ímpar: ${posicao}`


const aoQuadrado = mapear(NUMEROS, elevadoAoQuadrado)
// [ 1, 4, 9, 16, 25, 36, 49, 64, 81 ]
const aoCubo = mapear(NUMEROS, elevadoAoCubo)
// [ 1, 8, 27, 64, 125, 216, 343, 512, 729 ]
const posicoesNoArray = mapear(NUMEROS, posicoes)
/* [ 'posição par: 0',
  'posição ímpar: 1',
  'posição par: 2',
  'posição ímpar: 3',
  'posição par: 4',
  'posição ímpar: 5',
  'posição par: 6',
  'posição ímpar: 7',
  'posição par: 8' ]
*/
const umaPosicaoParaFrente = mapear(NUMEROS, andaUmaPosicao)
// [ 2, 3, 4, 5, 6, 7, 8, 9, 1 ]

const tudoJuntoEMisturado = NUMEROS.map(andaUmaPosicao).map(elevadoAoQuadrado).map(elevadoAoCubo)
// [ 64, 729, 4096, 15625, 46656, 117649, 262144, 531441, 1 ]
```



const posicoes = (num, posicao) => 
  (posicao % 2 === 0) 
    ? 'posição par: ' + posicao
    : 'posição ímpar: ' + posicao

```js
const filtrar = (arr, fn) => arr.filter(fn)

const apenasPares = (num) => (num % 2 === 0)
const apenasImpares = (num) => (num % 2 !== 0)

const pares = filtrar(NUMEROS, apenasPares)
const impares = filtrar(NUMEROS, apenasImpares)
```


## Experientes


```js
[
  {
      "ci_cod": 11122016100,
      "ci_titulo": "MEDIÇÕES EXTERNA",
      "ci_vm": "0,00",
      "ci_vr": "0,00",
      "ci_erro": "0,00",
      "ci_incerteza": "0,00",
      "ci_unidade": "mm",
      "ci_erro_incerteza": "0,00",
      "ci_criterio_aceitacao": "0,00",
      "ci_situacao": "------",
      "_id": "584e2f7a3e663748e71c1fd3",
      "ci_subtitulo": false
  },
  {
      "ci_cod": 11122016101,
      "ci_titulo": "MEDIÇÕES EXTERNA",
      "ci_vm": "1,30",
      "ci_vr": "1,30",
      "ci_erro": "0,00",
      "ci_incerteza": "0,01",
      "ci_unidade": "mm",
      "ci_erro_incerteza": "0,01",
      "ci_criterio_aceitacao": "0,18",
      "ci_situacao": "aprovado",
      "_id": "584e2f7a3e663748e71c1fd2",
      "ci_subtitulo": false
  },
  {
      "ci_cod": 11122016102,
      "ci_titulo": "MEDIÇÕES EXTERNA",
      "ci_vm": "100,00",
      "ci_vr": "100,00",
      "ci_erro": "0,00",
      "ci_incerteza": "0,01",
      "ci_unidade": "mm",
      "ci_erro_incerteza": "0,01",
      "ci_criterio_aceitacao": "0,18",
      "ci_situacao": "aprovado",
      "_id": "584e2f7a3e663748e71c1fd1",
      "ci_subtitulo": false
  },
  {
      "ci_cod": 11122016103,
      "ci_titulo": "MEDIÇÕES EXTERNA",
      "ci_vm": "200,00",
      "ci_vr": "200,00",
      "ci_erro": "0,00",
      "ci_incerteza": "0,01",
      "ci_unidade": "mm",
      "ci_erro_incerteza": "0,01",
      "ci_criterio_aceitacao": "0,18",
      "ci_situacao": "aprovado",
      "_id": "584e2f7a3e663748e71c1fd0",
      "ci_subtitulo": false
  },
  {
      "ci_cod": 11122016104,
      "ci_titulo": "MEDIÇÕES EXTERNA",
      "ci_vm": "300,00",
      "ci_vr": "300,00",
      "ci_erro": "0,00",
      "ci_incerteza": "0,01",
      "ci_unidade": "mm",
      "ci_erro_incerteza": "0,01",
      "ci_criterio_aceitacao": "0,18",
      "ci_situacao": "aprovado",
      "_id": "584e2f7a3e663748e71c1fcf",
      "ci_subtitulo": false
  },
  {
      "ci_cod": 11122016105,
      "ci_titulo": "MEDIÇÕES EXTERNA",
      "ci_vm": "500,00",
      "ci_vr": "500,00",
      "ci_erro": "0,00",
      "ci_incerteza": "0,01",
      "ci_unidade": "mm",
      "ci_erro_incerteza": "0,01",
      "ci_criterio_aceitacao": "0,18",
      "ci_situacao": "aprovado",
      "_id": "584e2f7a3e663748e71c1fce",
      "ci_subtitulo": false
  },
  {
      "ci_cod": 11122016106,
      "ci_titulo": "MEDIÇÕES EXTERNA",
      "ci_vm": "592,00",
      "ci_vr": "592,00",
      "ci_erro": "0,00",
      "ci_incerteza": "0,01",
      "ci_unidade": "mm",
      "ci_erro_incerteza": "0,01",
      "ci_criterio_aceitacao": "0,18",
      "ci_situacao": "aprovado",
      "_id": "584e2f7a3e663748e71c1fcd",
      "ci_subtitulo": false
  },
  {
      "ci_cod": 11122016107,
      "ci_titulo": "MEDIÇÃO INTERNA",
      "ci_vm": "40,00",
      "ci_vr": "39,998",
      "ci_erro": "0,002",
      "ci_incerteza": "0,010",
      "ci_unidade": "0",
      "ci_erro_incerteza": "0,012",
      "ci_criterio_aceitacao": "0,18",
      "ci_situacao": "aprovado",
      "_id": "584e2f7a3e663748e71c1fcc",
      "ci_subtitulo": false
  },
  {
      "ci_cod": 11122016108,
      "ci_titulo": "MEDIÇÃO PROFUNDIDADE",
      "ci_vm": "0,00",
      "ci_vr": "0,00",
      "ci_erro": "0,00",
      "ci_incerteza": "0,00",
      "ci_unidade": "0,00",
      "ci_erro_incerteza": "0,00",
      "ci_criterio_aceitacao": "0,00",
      "ci_situacao": "-------",
      "_id": "584e2f7a3e663748e71c1fcb",
      "ci_subtitulo": false
  },
  {
      "ci_cod": 11122016109,
      "ci_titulo": "MEDIÇÃO RESSALTO",
      "ci_vm": "50,00",
      "ci_vr": "50,00",
      "ci_erro": "0,00",
      "ci_incerteza": "0,01",
      "ci_unidade": "mm",
      "ci_erro_incerteza": "0,01",
      "ci_criterio_aceitacao": "0,18",
      "ci_situacao": "aprovado",
      "_id": "584e2f7a3e663748e71c1fca",
      "ci_subtitulo": false
  },
  {
      "ci_cod": 11122016110,
      "ci_titulo": "PARELELISMO",
      "ci_vm": "0,00",
      "ci_vr": "0,00",
      "ci_erro": "0,00",
      "ci_incerteza": "0,00",
      "ci_unidade": "-------",
      "ci_erro_incerteza": "0,00",
      "ci_criterio_aceitacao": "0,00",
      "ci_situacao": "-------",
      "_id": "584e2f7a3e663748e71c1fc9",
      "ci_subtitulo": false
  },
  {
      "ci_cod": 11122016111,
      "ci_titulo": "EXTERNA",
      "ci_vm": "25,00",
      "ci_vr": "25,00",
      "ci_erro": "0,00",
      "ci_incerteza": "0,01",
      "ci_unidade": "mm",
      "ci_erro_incerteza": "0,01",
      "ci_criterio_aceitacao": "0,18",
      "ci_situacao": "aprovado",
      "_id": "584e2f7a3e663748e71c1fc8",
      "ci_subtitulo": false
  },
  {
      "ci_cod": 11122016112,
      "ci_titulo": "INTERNA",
      "ci_vm": "0,00",
      "ci_vr": "0,00",
      "ci_erro": "0,00",
      "ci_incerteza": "0,00",
      "ci_unidade": "-------",
      "ci_erro_incerteza": "0,00",
      "ci_criterio_aceitacao": "0,00",
      "ci_situacao": "-------",
      "_id": "584e2f7a3e663748e71c1fc7",
      "ci_subtitulo": false
  }
]
```

### select

Vamos selecionar apenas o campo `ci_titulo`:

```js
> const field = 'ci_titulo'
> const select = (e, i) => ({ [field]: e[field] })
> arr.map(select)
[ { c_titulo: 'MEDIÇÕES EXTERNA' },
  { c_titulo: 'MEDIÇÕES EXTERNA' },
  { c_titulo: 'MEDIÇÕES EXTERNA' },
  { c_titulo: 'MEDIÇÕES EXTERNA' },
  { c_titulo: 'MEDIÇÕES EXTERNA' },
  { c_titulo: 'MEDIÇÕES EXTERNA' },
  { c_titulo: 'MEDIÇÕES EXTERNA' },
  { c_titulo: 'MEDIÇÃO INTERNA' },
  { c_titulo: 'MEDIÇÃO PROFUNDIDADE' },
  { c_titulo: 'MEDIÇÃO RESSALTO' },
  { c_titulo: 'PARELELISMO' },
  { c_titulo: 'EXTERNA' },
  { c_titulo: 'INTERNA' } ]

```

### where

```js
> const where = (e, i) => parseFloat(e.ci_vm.replace(',', '.')) >= 500 
> arr.filter(where)
[ { ci_cod: 11122016105,
    ci_titulo: 'MEDIÇÕES EXTERNA',
    ci_vm: '500,00',
    ci_vr: '500,00',
    ci_erro: '0,00',
    ci_incerteza: '0,01',
    ci_unidade: 'mm',
    ci_erro_incerteza: '0,01',
    ci_criterio_aceitacao: '0,18',
    ci_situacao: 'aprovado',
    _id: '584e2f7a3e663748e71c1fce',
    ci_subtitulo: false },
  { ci_cod: 11122016106,
    ci_titulo: 'MEDIÇÕES EXTERNA',
    ci_vm: '592,00',
    ci_vr: '592,00',
    ci_erro: '0,00',
    ci_incerteza: '0,01',
    ci_unidade: 'mm',
    ci_erro_incerteza: '0,01',
    ci_criterio_aceitacao: '0,18',
    ci_situacao: 'aprovado',
    _id: '584e2f7a3e663748e71c1fcd',
    ci_subtitulo: false } ]
```


### order by
```js
> const by = 'ci_vm'
> const order = {'ASC': (a, b) => a - b, 'DESC': (a, b) => a + b}
> const orderBy = (a, b) => order.ASC(parseFloat(a[by].replace(',', '.')),parseFloat(b[by].replace(',', '.')))
> arr.sort(orderBy)
[ { ci_cod: 11122016100,
    ci_titulo: 'MEDIÇÕES EXTERNA',
    ci_vm: '0,00',
    ci_vr: '0,00',
    ci_erro: '0,00',
    ci_incerteza: '0,00',
    ci_unidade: 'mm',
    ci_erro_incerteza: '0,00',
    ci_criterio_aceitacao: '0,00',
    ci_situacao: '------',
    _id: '584e2f7a3e663748e71c1fd3',
    ci_subtitulo: false },
  { ci_cod: 11122016112,
    ci_titulo: 'INTERNA',
    ci_vm: '0,00',
    ci_vr: '0,00',
    ci_erro: '0,00',
    ci_incerteza: '0,00',
    ci_unidade: '-------',
    ci_erro_incerteza: '0,00',
    ci_criterio_aceitacao: '0,00',
    ci_situacao: '-------',
    _id: '584e2f7a3e663748e71c1fc7',
    ci_subtitulo: false },
  { ci_cod: 11122016110,
    ci_titulo: 'PARELELISMO',
    ci_vm: '0,00',
    ci_vr: '0,00',
    ci_erro: '0,00',
    ci_incerteza: '0,00',
    ci_unidade: '-------',
    ci_erro_incerteza: '0,00',
    ci_criterio_aceitacao: '0,00',
    ci_situacao: '-------',
    _id: '584e2f7a3e663748e71c1fc9',
    ci_subtitulo: false },
  { ci_cod: 11122016108,
    ci_titulo: 'MEDIÇÃO PROFUNDIDADE',
    ci_vm: '0,00',
    ci_vr: '0,00',
    ci_erro: '0,00',
    ci_incerteza: '0,00',
    ci_unidade: '0,00',
    ci_erro_incerteza: '0,00',
    ci_criterio_aceitacao: '0,00',
    ci_situacao: '-------',
    _id: '584e2f7a3e663748e71c1fcb',
    ci_subtitulo: false },
  { ci_cod: 11122016101,
    ci_titulo: 'MEDIÇÕES EXTERNA',
    ci_vm: '1,30',
    ci_vr: '1,30',
    ci_erro: '0,00',
    ci_incerteza: '0,01',
    ci_unidade: 'mm',
    ci_erro_incerteza: '0,01',
    ci_criterio_aceitacao: '0,18',
    ci_situacao: 'aprovado',
    _id: '584e2f7a3e663748e71c1fd2',
    ci_subtitulo: false },
  { ci_cod: 11122016111,
    ci_titulo: 'EXTERNA',
    ci_vm: '25,00',
    ci_vr: '25,00',
    ci_erro: '0,00',
    ci_incerteza: '0,01',
    ci_unidade: 'mm',
    ci_erro_incerteza: '0,01',
    ci_criterio_aceitacao: '0,18',
    ci_situacao: 'aprovado',
    _id: '584e2f7a3e663748e71c1fc8',
    ci_subtitulo: false },
  { ci_cod: 11122016107,
    ci_titulo: 'MEDIÇÃO INTERNA',
    ci_vm: '40,00',
    ci_vr: '39,998',
    ci_erro: '0,002',
    ci_incerteza: '0,010',
    ci_unidade: '0',
    ci_erro_incerteza: '0,012',
    ci_criterio_aceitacao: '0,18',
    ci_situacao: 'aprovado',
    _id: '584e2f7a3e663748e71c1fcc',
    ci_subtitulo: false },
  { ci_cod: 11122016109,
    ci_titulo: 'MEDIÇÃO RESSALTO',
    ci_vm: '50,00',
    ci_vr: '50,00',
    ci_erro: '0,00',
    ci_incerteza: '0,01',
    ci_unidade: 'mm',
    ci_erro_incerteza: '0,01',
    ci_criterio_aceitacao: '0,18',
    ci_situacao: 'aprovado',
    _id: '584e2f7a3e663748e71c1fca',
    ci_subtitulo: false },
  { ci_cod: 11122016102,
    ci_titulo: 'MEDIÇÕES EXTERNA',
    ci_vm: '100,00',
    ci_vr: '100,00',
    ci_erro: '0,00',
    ci_incerteza: '0,01',
    ci_unidade: 'mm',
    ci_erro_incerteza: '0,01',
    ci_criterio_aceitacao: '0,18',
    ci_situacao: 'aprovado',
    _id: '584e2f7a3e663748e71c1fd1',
    ci_subtitulo: false },
  { ci_cod: 11122016103,
    ci_titulo: 'MEDIÇÕES EXTERNA',
    ci_vm: '200,00',
    ci_vr: '200,00',
    ci_erro: '0,00',
    ci_incerteza: '0,01',
    ci_unidade: 'mm',
    ci_erro_incerteza: '0,01',
    ci_criterio_aceitacao: '0,18',
    ci_situacao: 'aprovado',
    _id: '584e2f7a3e663748e71c1fd0',
    ci_subtitulo: false },
  { ci_cod: 11122016104,
    ci_titulo: 'MEDIÇÕES EXTERNA',
    ci_vm: '300,00',
    ci_vr: '300,00',
    ci_erro: '0,00',
    ci_incerteza: '0,01',
    ci_unidade: 'mm',
    ci_erro_incerteza: '0,01',
    ci_criterio_aceitacao: '0,18',
    ci_situacao: 'aprovado',
    _id: '584e2f7a3e663748e71c1fcf',
    ci_subtitulo: false },
  { ci_cod: 11122016105,
    ci_titulo: 'MEDIÇÕES EXTERNA',
    ci_vm: '500,00',
    ci_vr: '500,00',
    ci_erro: '0,00',
    ci_incerteza: '0,01',
    ci_unidade: 'mm',
    ci_erro_incerteza: '0,01',
    ci_criterio_aceitacao: '0,18',
    ci_situacao: 'aprovado',
    _id: '584e2f7a3e663748e71c1fce',
    ci_subtitulo: false },
  { ci_cod: 11122016106,
    ci_titulo: 'MEDIÇÕES EXTERNA',
    ci_vm: '592,00',
    ci_vr: '592,00',
    ci_erro: '0,00',
    ci_incerteza: '0,01',
    ci_unidade: 'mm',
    ci_erro_incerteza: '0,01',
    ci_criterio_aceitacao: '0,18',
    ci_situacao: 'aprovado',
    _id: '584e2f7a3e663748e71c1fcd',
    ci_subtitulo: false } ]

```

### group by

```js
const by = 'ci_titulo'
const groupBy = (select, element) => {
  (select[element[by]] = select[element[by]] || []).push(element)
  return select
} 
> arr.reduce(g, {})
{ 'MEDIÇÕES EXTERNA': 
   [ { ci_cod: 11122016100,
       ci_titulo: 'MEDIÇÕES EXTERNA',
       ci_vm: '0,00',
       ci_vr: '0,00',
       ci_erro: '0,00',
       ci_incerteza: '0,00',
       ci_unidade: 'mm',
       ci_erro_incerteza: '0,00',
       ci_criterio_aceitacao: '0,00',
       ci_situacao: '------',
       _id: '584e2f7a3e663748e71c1fd3',
       ci_subtitulo: false },
     { ci_cod: 11122016101,
       ci_titulo: 'MEDIÇÕES EXTERNA',
       ci_vm: '1,30',
       ci_vr: '1,30',
       ci_erro: '0,00',
       ci_incerteza: '0,01',
       ci_unidade: 'mm',
       ci_erro_incerteza: '0,01',
       ci_criterio_aceitacao: '0,18',
       ci_situacao: 'aprovado',
       _id: '584e2f7a3e663748e71c1fd2',
       ci_subtitulo: false },
     { ci_cod: 11122016102,
       ci_titulo: 'MEDIÇÕES EXTERNA',
       ci_vm: '100,00',
       ci_vr: '100,00',
       ci_erro: '0,00',
       ci_incerteza: '0,01',
       ci_unidade: 'mm',
       ci_erro_incerteza: '0,01',
       ci_criterio_aceitacao: '0,18',
       ci_situacao: 'aprovado',
       _id: '584e2f7a3e663748e71c1fd1',
       ci_subtitulo: false },
     { ci_cod: 11122016103,
       ci_titulo: 'MEDIÇÕES EXTERNA',
       ci_vm: '200,00',
       ci_vr: '200,00',
       ci_erro: '0,00',
       ci_incerteza: '0,01',
       ci_unidade: 'mm',
       ci_erro_incerteza: '0,01',
       ci_criterio_aceitacao: '0,18',
       ci_situacao: 'aprovado',
       _id: '584e2f7a3e663748e71c1fd0',
       ci_subtitulo: false },
     { ci_cod: 11122016104,
       ci_titulo: 'MEDIÇÕES EXTERNA',
       ci_vm: '300,00',
       ci_vr: '300,00',
       ci_erro: '0,00',
       ci_incerteza: '0,01',
       ci_unidade: 'mm',
       ci_erro_incerteza: '0,01',
       ci_criterio_aceitacao: '0,18',
       ci_situacao: 'aprovado',
       _id: '584e2f7a3e663748e71c1fcf',
       ci_subtitulo: false },
     { ci_cod: 11122016105,
       ci_titulo: 'MEDIÇÕES EXTERNA',
       ci_vm: '500,00',
       ci_vr: '500,00',
       ci_erro: '0,00',
       ci_incerteza: '0,01',
       ci_unidade: 'mm',
       ci_erro_incerteza: '0,01',
       ci_criterio_aceitacao: '0,18',
       ci_situacao: 'aprovado',
       _id: '584e2f7a3e663748e71c1fce',
       ci_subtitulo: false },
     { ci_cod: 11122016106,
       ci_titulo: 'MEDIÇÕES EXTERNA',
       ci_vm: '592,00',
       ci_vr: '592,00',
       ci_erro: '0,00',
       ci_incerteza: '0,01',
       ci_unidade: 'mm',
       ci_erro_incerteza: '0,01',
       ci_criterio_aceitacao: '0,18',
       ci_situacao: 'aprovado',
       _id: '584e2f7a3e663748e71c1fcd',
       ci_subtitulo: false } ],
  'MEDIÇÃO INTERNA': 
   [ { ci_cod: 11122016107,
       ci_titulo: 'MEDIÇÃO INTERNA',
       ci_vm: '40,00',
       ci_vr: '39,998',
       ci_erro: '0,002',
       ci_incerteza: '0,010',
       ci_unidade: '0',
       ci_erro_incerteza: '0,012',
       ci_criterio_aceitacao: '0,18',
       ci_situacao: 'aprovado',
       _id: '584e2f7a3e663748e71c1fcc',
       ci_subtitulo: false } ],
  'MEDIÇÃO PROFUNDIDADE': 
   [ { ci_cod: 11122016108,
       ci_titulo: 'MEDIÇÃO PROFUNDIDADE',
       ci_vm: '0,00',
       ci_vr: '0,00',
       ci_erro: '0,00',
       ci_incerteza: '0,00',
       ci_unidade: '0,00',
       ci_erro_incerteza: '0,00',
       ci_criterio_aceitacao: '0,00',
       ci_situacao: '-------',
       _id: '584e2f7a3e663748e71c1fcb',
       ci_subtitulo: false } ],
  'MEDIÇÃO RESSALTO': 
   [ { ci_cod: 11122016109,
       ci_titulo: 'MEDIÇÃO RESSALTO',
       ci_vm: '50,00',
       ci_vr: '50,00',
       ci_erro: '0,00',
       ci_incerteza: '0,01',
       ci_unidade: 'mm',
       ci_erro_incerteza: '0,01',
       ci_criterio_aceitacao: '0,18',
       ci_situacao: 'aprovado',
       _id: '584e2f7a3e663748e71c1fca',
       ci_subtitulo: false } ],
  PARELELISMO: 
   [ { ci_cod: 11122016110,
       ci_titulo: 'PARELELISMO',
       ci_vm: '0,00',
       ci_vr: '0,00',
       ci_erro: '0,00',
       ci_incerteza: '0,00',
       ci_unidade: '-------',
       ci_erro_incerteza: '0,00',
       ci_criterio_aceitacao: '0,00',
       ci_situacao: '-------',
       _id: '584e2f7a3e663748e71c1fc9',
       ci_subtitulo: false } ],
  EXTERNA: 
   [ { ci_cod: 11122016111,
       ci_titulo: 'EXTERNA',
       ci_vm: '25,00',
       ci_vr: '25,00',
       ci_erro: '0,00',
       ci_incerteza: '0,01',
       ci_unidade: 'mm',
       ci_erro_incerteza: '0,01',
       ci_criterio_aceitacao: '0,18',
       ci_situacao: 'aprovado',
       _id: '584e2f7a3e663748e71c1fc8',
       ci_subtitulo: false } ],
  INTERNA: 
   [ { ci_cod: 11122016112,
       ci_titulo: 'INTERNA',
       ci_vm: '0,00',
       ci_vr: '0,00',
       ci_erro: '0,00',
       ci_incerteza: '0,00',
       ci_unidade: '-------',
       ci_erro_incerteza: '0,00',
       ci_criterio_aceitacao: '0,00',
       ci_situacao: '-------',
       _id: '584e2f7a3e663748e71c1fc7',
       ci_subtitulo: false } ] }

```

