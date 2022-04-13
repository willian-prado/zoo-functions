## Projeto Zoo Functions

> Sétimo projeto do módulo de Fundamentos do curso de desenvolvimento web da Trybe.

**Contexto**

Neste projeto utilizamos às principais funcionalides do ES6, como arrow functions , template literals , spread operator , parâmetro rest e object destructuring. 
Também podemos experimentar com as HOFs (Higher Order Functions) de JS mais utilizadas, tais como `forEach`, `map`, `filter`, `reduce`, `every`, `sort`, `find`, entre outras.

**Objetivo do projeto**

Desenvolver um sistema de relatório de um zoológico. O sistema possui informações a respeito dos animais presentes no zoológico, colaboradores, horários de funcionamento e uma tabela de preços que varia de acordo com a idade das pessoas que o visitam.

**Principais habilidades desenvolvidas nesse trabalho:**

- Produzir código legível, conciso e expressivo utilizando as novas funcionalidades do ES6
- Utilizar as _Higher Order Functions_ para manipular e criar arrays
- Escolher a _Higher Order Function_ mais adequada para a obtenção de um resultado esperado
- Aprender a usar de forma conjunta as _Higher Order Functions_
- Interpretar testes unitários e produzir soluções que atendam a eles

**Tecnologias utilizadas**
- <a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/javascript/javascript-original.svg" title="JavaScript" align="center" height="30"/>  - JavaScript</a>

---

### Lista de requisitos propostos:

#### Obrigatórios

**1. IMPLEMENTE A FUNÇÃO getSpeciesByIds**

  Esta função é responsável pela busca das espécies de animais por id. Ela retorna um array contendo as espécies referentes aos ids passados como parâmetro, podendo receber um ou mais ids.

**2. IMPLEMENTE A FUNÇÃO getAnimalsOlderThan**

  Esta função, a partir do nome de uma espécie e uma idade mínima, verifica se todos os animais daquela espécie possuem a idade mínima especificada.
  Ela deve retornar um valor booleano.

**3. IMPLEMENTE A FUNÇÃO getEmployeeByName**

   Esta função é responsável pela busca das pessoas colaboradoras através do primeiro ou do último nome delas

**4. IMPLEMENTE A FUNÇÃO createEmployee**

  A função, a partir de informações recebidas nos parâmetros, é capaz de criar um objeto equivalente ao de uma pessoa colaboradora, retornando-o.
  Ela deve criar um novo colaborador a partir de objetos contendo `informações pessoais` e `gerentes e animais gerenciados`.

  **Observações técnicas**

  - O parâmetro `personalInfo` recebe um objeto que contém o `id`, o `firstName` e o `lastName`
  - O parâmetro `associatedWith` recebe um objeto que contém dois array: `managers` e `responsibleFor`

**5. IMPLEMENTE A FUNÇÃO isManager**

  Verifica se uma pessoa colaboradora, a partir de seu id, ocupa cargo de gerência.
  Ela deve retornar um valor booleano

**6. IMPLEMENTE A FUNÇÃO addEmployee**

  A função irá adicionar uma nova pessoa colaboradora no final do array `employees`, presente no arquivo `data.js`.

**7. IMPLEMENTE A FUNÇÃO countAnimals**

  Esta função é responsável por contabilizar a quantidade de animais.

  **Observações técnicas**

  - Sem parâmetros, retorna um objeto
  - Com o nome de uma espécie de animal, retorna um número

**8. IMPLEMENTE A FUNÇÃO calculateEntry**

  A partir da quantidade de visitantes e a faixa etária de cada um, esta função é responsável por retornar o preço total a ser cobrado

  **Observações técnicas**

  - O parâmetro `entrants` recebe um objeto que contém as chaves `Adult`, `Child` e `Senior`, com suas respectivas quantidades de pessoas

**9. IMPLEMENTE A FUNÇÃO getAnimalMap**

  A função é responsável pelo mapeamento geográfico das espécies e seus animais, podendo ainda filtrá-los por ordem alfabética e gênero, por exemplo.

  **Observações técnicas**

  - Sem parâmetros, a função retorna animais categorizados por localização
  - Com a opção `includeNames: true` especificada, retorna nomes de animais
  - Com a opção `sorted: true` especificada, retorna nomes de animais ordenados
  - Com a opção `sex: 'female'` ou `sex: 'male'` especificada, retorna somente nomes de animais macho/fêmea
  - Com a opção `sex: 'female'` ou `sex: 'male'` especificada e a opção `sort: true` especificada, retorna somente nomes de animais macho/fêmea com os nomes dos animais ordenados
  - Só retorna informações ordenadas e com sexo se a opção `includeNames: true` for especificada

**10. IMPLEMENTE A FUNÇÃO getSchedule**

  A função é responsável por disponibilizar as informações de horário para uma consulta, que pode querer ter acesso a todo o cronograma da semana ou apenas o cronograma de um dia específico

  **Observações técnicas**
  
  - Sem parâmetros, retorna um cronograma legível para humanos
  - Se um único dia for passado, retorna somente este dia em um formato legível para humanos

**11. IMPLEMENTE A FUNÇÃO getOldestFromFirstSpecies**

  A função, passado o id de um funcionário, encontra a primeira espécie de animal gerenciado pelo funcionário, e retorna um array com nome, sexo e idade do
  animal mais velho dessa espécie.

**12. IMPLEMENTE A FUNÇÃO increasePrices**

  A função é responsável por aumentar o preço das visitas, com base no valor de aumento recebido no parâmetro, em porcentagem.
  Ao passar uma porcentagem, incrementa todos os preços, arrendondados em duas casas decimais

**13. IMPLEMENTE A FUNÇÃO getEmployeeCoverage**

  A função é responsável por consultar as espécies pela qual a pessoa colaborada, recebida no parâmetro através de seu `id`, `firstName` ou `lastName`, é responsável

  **Observações técnicas**
  
  - Sem parâmetros, a função retorna uma lista de funcionários e os animais pelos quais eles são responsáveis
  - Com o id de um funcionário, retorna os animais pelos quais o funcionário é responsável
  - Com o primeiro nome de um funcionário, retorna os animais pelos quais o funcionário é responsável
  - Com o último nome de um funcionário, retorna os animais pelos quais o funcionário é responsável
