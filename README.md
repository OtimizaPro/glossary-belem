# Glossário Belem An.C - Tradução Bíblica Colaborativa

> Glossário colaborativo para a tradução literal da Bíblia Belem An.C 2025

## Sobre

Este repositório contém os glossários de tradução do **Hebraico**, **Grego Koiné** e **Aramaico** utilizados na tradução Bíblia Belem An.C 2025.

A tradução segue o princípio de **literalidade rígida** (*ipsis litteris*), onde:

- Zero interpretação do tradutor
- Preservação de tempos verbais, ordem sintática e partículas
- Intervenções mínimas, marcadas com `[ ]`
- O leitor faz a interpretação, não o tradutor

## Estrutura

```
glossary-belem/
├── greek/
│   ├── glossary.json         # Mapeamentos Grego → PT-BR
│   ├── strongs.json          # Referências Strong's
│   └── alternatives.json     # Traduções alternativas
├── hebrew/
│   ├── glossary.json         # Mapeamentos Hebraico → PT-BR
│   ├── strongs.json          # Referências Strong's
│   └── alternatives.json     # Traduções alternativas
├── aramaic/
│   └── glossary.json         # Mapeamentos Aramaico → PT-BR
├── keep-original/
│   └── sacred-names.json     # Palavras mantidas no original
└── CONTRIBUTING.md           # Guia de contribuição
```

## Como Contribuir

### Sugerir Nova Tradução

1. Abra uma **Issue** com o template "Translation Suggestion"
2. Inclua:
   - Palavra original (com transliteração)
   - Número Strong's
   - Tradução literal sugerida
   - Justificativa linguística/etimológica
   - Exemplos de uso bíblico (2-3 versículos)

### Submeter Pull Request

1. Fork este repositório
2. Crie branch: `gloss/palavra-strongsXXXX`
3. Edite o JSON apropriado
4. Submeta PR com justificativa completa

### Revisão

- Toda sugestão passa por revisão de **2 tradutores**
- Após aprovação, o glossário é sincronizado automaticamente com a API

## Princípios de Tradução

| Princípio | Descrição |
|-----------|-----------|
| **Literalidade** | Tradução palavra-por-palavra quando possível |
| **Transparência** | Intervenções marcadas com `[ ]` |
| **Consistência** | Mesma palavra grega/hebraica = mesma tradução |
| **Etimologia** | Priorizar raiz etimológica sobre uso teológico |
| **Neutralidade** | Sem viés denominacional ou escola teológica |

## Formato JSON

```json
{
  "G3056": {
    "original": "λόγος",
    "transliteration": "logos",
    "literal": "palavra",
    "notes": "Do verbo legō (falar). Preservar como 'palavra' em todos os contextos.",
    "references": ["João 1:1", "Apocalipse 19:13"]
  }
}
```

## Licença

Copyright 2025 Anderson Costa Belem - A Culpa é das Ovelhas

O glossário é disponibilizado para uso não-comercial e fins de estudo bíblico.

---

**Ecossistema A Culpa é das Ovelhas** | [Site](https://aculpaedasovelhas.org) | [API](https://biblia.aculpaedasovelhas.org)
