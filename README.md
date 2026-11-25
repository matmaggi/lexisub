# LexiSub

**Glossário inteligente para tradução e legendagem: a IA lê suas legendas e monta o glossário de nomes, lugares e expressões.**

O LexiSub analisa as legendas de um projeto com IA e cria um glossário com personagens (e gênero), lugares, organizações, títulos e expressões, com sugestão de tradução e notas. A cada episódio novo, ele mostra só os termos novos para você aprovar.

## Formatos aceitos
SRT, DFXP, PXTT, TTML e TTAL (vários arquivos de uma vez).

## Funcionalidades

### Projetos
- Título e **contexto do projeto** (sinopse, público, tom, observações do cliente), usados na análise.
- **Projetos recentes** salvos no navegador, com aviso de alterações ainda não exportadas.
- Novo projeto, abrir projeto (.xlsx) e exportar projeto.

### Análise com IA
- **Claude, ChatGPT/OpenAI ou Gemini** pela API, ou **modo manual** (copiar o prompt e colar a resposta de qualquer chat, sem chave de API).
- Idioma de destino configurável (padrão: português do Brasil).
- Divide automaticamente o material em partes quando ele é grande.
- **Custo estimado** antes e **custo real** depois da análise.
- Usa os nomes de personagens que vêm nos metadados de arquivos TTAL como pista.
- Descarta termos que não aparecem de fato nas legendas (considerando singular e plural).

### Tipos de termo
- **CHARACTER:** personagens e pessoas citadas, com gênero (M, F ou ?), apelidos e honoríficos (ex.: "Dr. Hale" → "Dra. Hale").
- **LOCATION:** países, cidades, bairros, ruas, edifícios, estabelecimentos e lugares fictícios.
- **ORGANIZATION:** empresas, instituições, agências, grupos, equipes e facções.
- **TITLES:** livros, filmes, séries, músicas, jogos, programas e outras obras citadas.
- **PHRASE:** gírias, jargões, bordões, expressões idiomáticas e frases recorrentes.

### Episódios novos
- Termos novos vão para uma **lista de revisão**: aceitar ou excluir um por um, ou todos de uma vez.
- **Sugestões de atualização:** quando um diálogo novo revela o gênero de um personagem que estava "?".
- Termos editados à mão nunca são sobrescritos pela IA (marcados com um ponto laranja).
- **Termos excluídos** não voltam a ser sugeridos; podem ser restaurados ou liberados.

### Glossário
- Tabela editável, com cores por tipo e gênero.
- Busca, filtros por tipo e gênero, ordenação por coluna.
- **Ocorrências:** em quais episódios cada termo aparece, com filtro por arquivo.
- Incluir termos manualmente.

### Exportação
- **Excel (.xlsx)** formatado, com abas de glossário, informações do projeto e termos excluídos.
- **Copiar em texto:** gera instruções prontas para colar em uma ferramenta de tradução ou IA (termos, nomes femininos, masculinos e de gênero desconhecido).

## Privacidade
Projetos, legendas e chave de API ficam salvos apenas no seu navegador. O texto das legendas só é enviado para a IA escolhida quando você clica em *Analisar legendas*.
