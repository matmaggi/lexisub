# LexiSub

**Glossário inteligente para tradução e legendagem: a IA lê suas legendas e monta o glossário de nomes, lugares e expressões.**

O LexiSub analisa as legendas de um projeto com IA e cria um glossário com personagens (e gênero), lugares, organizações, títulos e expressões, com sugestão de tradução e notas. A cada episódio novo, ele mostra só os termos novos para você aprovar.

## Formatos aceitos
SRT, DFXP, PXTT, TTML e TTAL (vários arquivos de uma vez).

## Funcionalidades

### Projetos
- Título e **contexto do projeto** (sinopse, público, tom, observações do cliente), usados na análise.
- **Projetos recentes** salvos no navegador, com aviso de alterações ainda não exportadas.
- Novo projeto, abrir projeto (.xlsx) e exportar projeto. Abrir de novo um projeto que já está na memória atualiza o mesmo projeto, sem criar uma cópia.

### Análise com IA
- **Claude, ChatGPT/OpenAI, Gemini, Groq (plano gratuito), OpenRouter (modelos gratuitos)** ou **qualquer serviço compatível com a API da OpenAI**, inclusive Ollama e LM Studio rodando no seu computador. Também há o **modo manual** (copiar o prompt e colar a resposta de qualquer chat, sem chave de API).
- **Salvar chave (opcional):** a chave só fica guardada no navegador se você marcar essa opção.
- Idiomas de origem e de destino configuráveis (padrão: inglês → português do Brasil).
- Divide automaticamente o material em partes quando ele é grande. Cada parte recebe os termos já encontrados nas anteriores e o glossário existente, para manter as mesmas traduções.
- **Nova tentativa automática** quando o limite de uso do serviço é atingido ou há falha temporária.
- **Nada se perde se uma parte falhar:** o que já foi analisado é aproveitado, e o botão *Tentar de novo as partes que faltaram* repete só o que deu errado.
- **Custo estimado** antes e **custo real** depois da análise.
- Usa os nomes de personagens que vêm nos metadados de arquivos TTAL como pista.
- Descarta termos que não aparecem de fato nas legendas (considerando singular e plural).
- Lê arquivos em UTF-8, UTF-16 e Windows-1252, e mantém falas que são só números ou que começam com palavras como “OK:”.

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
- **Termos excluídos** não voltam a ser sugeridos; o botão *Restaurar* devolve o termo ao glossário.

### Glossário
- Tabela editável, com cores por tipo e gênero.
- Busca que ignora acentos (“Joao” encontra “João”), filtros por tipo e gênero, ordenação por coluna.
- **↩ Desfazer** a última alteração (edições, exclusões, aceites e análises).
- **Ocorrências:** em quais episódios cada termo aparece, com filtro por arquivo.
- Incluir termos manualmente.

### Exportação
- **Excel (.xlsx)** formatado, com abas de glossário, informações do projeto e termos excluídos.
- **Copiar em texto:** gera instruções prontas para colar em uma ferramenta de tradução ou IA (termos, nomes femininos, masculinos e de gênero desconhecido).

## Privacidade
Projetos e legendas ficam salvos apenas no seu navegador; a chave de API, só se você marcar *Salvar chave*. O texto das legendas só é enviado para a IA escolhida quando você clica em *Analisar legendas*.
