# Contribuindo para o Glossário Belem An.C

Obrigado por seu interesse em contribuir para a tradução Bíblica Belem An.C!

## Tipos de Contribuição

### 1. Sugestão de Tradução

Para sugerir uma nova tradução ou melhoria:

1. Abra uma **Issue** usando o template "Sugestão de Tradução"
2. Forneça todas as informações solicitadas:
   - Palavra original (com alfabeto original)
   - Número Strong's
   - Tradução literal sugerida
   - Justificativa etimológica
   - Exemplos bíblicos (2-3 versículos)

### 2. Correção de Erro

Para reportar erros no glossário:

1. Abra uma **Issue** usando o template "Erro no Glossário"
2. Indique claramente o erro e a correção proposta

### 3. Pull Request

Para contribuir diretamente com código:

1. Fork este repositório
2. Crie uma branch: `gloss/palavra-strongsXXXX`
3. Faça suas alterações
4. Execute validação local: `jq empty *.json`
5. Commit com mensagem descritiva
6. Abra Pull Request com justificativa completa

## Princípios de Tradução

Todas as contribuições devem seguir os princípios da tradução Belem An.C:

| Princípio | Descrição |
|-----------|-----------|
| **Literalidade** | Tradução palavra-por-palavra sempre que possível |
| **Transparência** | Intervenções marcadas com `[ ]` |
| **Consistência** | Mesma palavra = mesma tradução em todo o texto |
| **Etimologia** | Priorizar raiz etimológica sobre uso teológico moderno |
| **Neutralidade** | Sem viés denominacional |

## Formato do Glossário

```json
{
  "palavra_original": "tradução_literal"
}
```

Para entradas mais complexas:
```json
{
  "G3056": {
    "original": "λόγος",
    "transliteration": "logos",
    "literal": "palavra",
    "notes": "Justificativa da tradução"
  }
}
```

## Processo de Revisão

1. **Validação automática** - CI verifica sintaxe JSON
2. **Revisão por tradutores** - Mínimo 2 revisores
3. **Verificação de consistência** - Comparação com traduções existentes
4. **Merge** - Após aprovação, merge para main
5. **Sync** - Glossário sincronizado automaticamente com API

## Código de Conduta

- Respeite outros contribuidores
- Mantenha foco no texto bíblico, não em doutrinas
- Argumente com fontes acadêmicas
- Aceite feedback construtivo

## Dúvidas

Use a aba **Discussions** para perguntas gerais sobre tradução.

---

**A Culpa é das Ovelhas** - Ecossistema de Tradução Bíblica Literal
