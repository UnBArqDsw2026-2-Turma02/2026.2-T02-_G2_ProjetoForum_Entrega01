# 1.3.4.2. Modelo de Ata

Modelo a ser duplicado para o registro de cada reunião realizada pelo grupo.

Ao criar uma nova ata:
1. Nomeie o arquivo de forma descritiva e sequencial, por exemplo
   `ata-01-onboarding.md`.
2. Salve o arquivo na pasta correta: reuniões com a equipe toda vão em
   `docs/Base/iniciativas_extras/atas_reuniao/gerais/`; reuniões internas de
   um subgrupo vão em
   `docs/Base/iniciativas_extras/atas_reuniao/subequipe_0X/` (crie a pasta
   se ainda não existir).
3. Adicione o link ao [_sidebar.md](../../../_sidebar.md), na subseção
   "Reuniões Gerais" ou "Reuniões por Subequipe" correspondente, e também ao
   Sumário do `docs/README.md`.
4. Inclua uma linha correspondente na
   [Tabela de Rastreabilidade](./rastreabilidade.md), na tabela certa
   (Reuniões Gerais ou a subequipe correspondente).

---

## Ata XX - Título da Reunião

**Data:** dd/mm/aaaa
**Subgrupo:** (geral / Subequipe_01 / Subequipe_02 / Subequipe_03)
**Canal:** (Google Meet / WhatsApp)
**Liderança responsável:** _A preencher_

### Participantes
| Nome do Membro | Presente |
| -- | :-: |
| _A preencher_ | |

### Gravação

Se houver vídeo da reunião publicado como não listado no YouTube,
incorpore-o (substitua `ID_DO_VIDEO`):

```html
<div style="text-align: center;">
  <iframe width="560" height="315" src="https://www.youtube.com/embed/ID_DO_VIDEO" title="Título da reunião" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
</div>
```

### Resumo
_Um parágrafo resumindo o objetivo e o resultado principal da reunião._

### Pauta
1. _A preencher_

### Detalhes da discussão
_Por tópico, com o timestamp do vídeo entre parênteses quando disponível
(ex. `(00:03:53)`), para permitir navegar direto ao ponto do vídeo._

### Encaminhamentos
| Responsável | Encaminhamento |
| -- | -- |
| _A preencher_ | |

### Comprobatório
_Link direto do vídeo, ou outra evidência da reunião (print, arquivo,
etc.)._
