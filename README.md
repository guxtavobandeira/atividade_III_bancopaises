RESOLUÇÃO DAS QUESTÕES:

1. Selecione todos os dados dos países da tabela_paises;

CÓDIGO:

select * from tabela_paises

FOTO:
![Captura de Tela (51)](https://github.com/guxtavobandeira/atividade_III_bancopaises/assets/111713549/efccb8a7-ae56-4554-b8f6-b2f23e42bb4b)

2. Selecione todas as cidades cujo país seja brazil;

CÓDIGO:

select cidade

from tabela_paises

where pais='Brazil'

FOTO:

![Captura de Tela (52)](https://github.com/guxtavobandeira/atividade_III_bancopaises/assets/111713549/392b05b2-311d-400b-ba1e-1958bc2819c2)


3. Selecione todas as cidades cuja região(estado) é ceará;

CÓDIGO:

select cidade

from tabela_paises

where regiao='Ceará'

FOTO:

![Captura de Tela (53)](https://github.com/guxtavobandeira/atividade_III_bancopaises/assets/111713549/aeccc82d-8809-44ba-8d62-d57f395359ca)

4. Utilize a função count para saber quantas regiões(estados) existem na China,
utilize também o group by;

CÓDIGO:

select regiao, count(regiao) as total_regioes_china

from tabela_paises

where pais='China' group by regiao

FOTO:

![Captura de Tela (54)](https://github.com/guxtavobandeira/atividade_III_bancopaises/assets/111713549/c4a4e63b-a7a0-4903-b956-e73d8107e076)

5. Quais regiões, diferentes, existem no Canadá?

CÓDIGO:

select count(distinct regiao) as total_regioes

from tabela_paises

where pais='Canada'

FOTO:

![Captura de Tela (60)](https://github.com/guxtavobandeira/atividade_III_bancopaises/assets/111713549/9d2f4b63-ccde-4931-8eac-97e380bb8784)


6. Quantos países diferentes existem na tabela 'tabela_paises';

CÓDIGO:

select count(distinct pais) as total_paises

from tabela_paises

FOTO:

![Captura de Tela (59)](https://github.com/guxtavobandeira/atividade_III_bancopaises/assets/111713549/dd5f9b88-3b43-4407-9147-ec4c866cfb7c)


7. Quantas cidades diferentes existem no brazil;

CÓDIGO:

select count(distinct cidade)

from tabela_paises

where pais='Brazil'

FOTO:

![Captura de Tela (57)](https://github.com/guxtavobandeira/atividade_III_bancopaises/assets/111713549/21497847-6102-44f3-8d4b-8822249a9074)

8. Selecione os países e quantas regiões cada país possui;

CÓDIGO:

select pais,count(pais) as total_regioes

from tabela_paises

group by pais

FOTO:

![Captura de Tela (58)](https://github.com/guxtavobandeira/atividade_III_bancopaises/assets/111713549/acb2437f-2ce5-49aa-b42c-90fdd98a8282)

9. Quantas pessoas com nome começando em 'João' existem no banco?
CÓDIGO:
FOTO:
10. Quantas pessoas têm o nome John?
CÓDIGO:
FOTO:
11. Ordene os nomes dos países sem repetição em ordem alfabética;

CÓDIGO:

select distinct pais

from tabela_paises

order by pais

FOTO:

![Captura de Tela (61)](https://github.com/guxtavobandeira/atividade_III_bancopaises/assets/111713549/3b0fa802-8966-4d01-8a31-2dfd68c27b2b)













