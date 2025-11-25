# 🔍 Validador de Densidade Semântica (SD)

**Framework:** Semantic Latent Engineering (SLE)
**Ferramenta:** Scientific Validation Hub
**Status:** Production Ready

---

### ⚡ Quick Start (Modo Assistido)
Não quer analisar códigos? Deixe a IA fazer isso.

1.  **Configure:** Na célula de código abaixo, altere as variáveis `name_to_test` (Nome do seu Agente) e `domain_to_test` (O que ele deve fazer).
2.  **Execute:** Clique no botão de Play (▶) na célula.
3.  **Valide:** Abra o Assistente Gemini (ícone ✨) e cole o prompt abaixo:

> "Atue como Auditor de Engenharia de Software. Analise o output da validação abaixo. Se o status for 'PASS', gere um código Markdown para um Badge verde escrito 'Scientific Validation: PASSING'. Se for 'FAIL', explique qual métrica falhou (Minimalismo ou Densidade Vetorial)."

# Instalação das dependências de vetorialização (HuggingFace)
!pip install sentence-transformers -q
print("✅ Motor Vetorial instalado. Carregando modelos neurais...")
