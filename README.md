# Conteris - Download Repository

Repositório oficial para distribuição dos instaladores do **Conteris - Separador de Holerites**.

Aqui você encontra as versões compiladas para Windows do aplicatvo.

## ⬇️ Downloads Disponíveis

> 🔒 **Arquivos protegidos por senha.**
> Entre em contato com a equipe para obter a senha de acesso.

### Versão Mais Recente
- [**Conteris v1.2.2 (ZIP)**](./Conteris_Installer_v1.2.2.zip) _(Recomendado)_

### Versões Anteriores
- [Conteris v1.2.1 (ZIP)](./Conteris_Installer_v1.2.1.zip)
- [Conteris v1.2.0 (ZIP)](./Conteris_Installer_v1.2.0.zip)
- [Conteris v1.1.1 (ZIP)](./Conteris_Installer_v1.1.1.zip)
- [Conteris v1.0.0 (ZIP)](./Conteris_Installer_v1.0.0.zip)

---

## 📝 Histórico de Versões

### v1.2.2 (Atual)
- **UI**: Padronização visual completa entre os módulos Salários e Notas Fiscais.
- **UI**: Módulo NF exibe resultados apenas após clicar nos botões de processamento.
- **Refatoração**: `PdfService` singleton com cache de documentos para melhor desempenho.
- **Refatoração**: Tema centralizado, `MessageMixin` e pool de `PageIcon` — menos uso de memória.
- **Recurso**: Banco de nomes brasileiros expandido.
- **Correção**: Janelas e modais abrem sempre no monitor principal em configurações multi-monitor.
- **Testes**: 146/146 testes passando.

### v1.2.1
- **Novo**: Identidade visual oficial — novo ícone e logo com gradiente azul/vermelho e sombra projetada.
- **Novo**: Arquivo `.ico` multi-resolução com 6 tamanhos (16×16 a 256×256).
- **Correção**: Logo exibia nome "conteri" (sem o "s") — viewBox corrigido.
- **Limpeza**: Removidos arquivos SVG genéricos não utilizados da pasta `icons/`.
- **Manual**: Capa com nova logo e nova seção 5 dedicada ao módulo Separador de Notas Fiscais.

### v1.2.0
- **Correção**: Inclusão da pasta `resources` na instalação para permitir edição externa do arquivo `names.txt`.
- **Correção**: Ajustes no manual do usuário.

### v1.1.0
- **Novo**: Busca elástica (Fuzzy Matching) para nomes.
- **Novo**: Banco de dados de nomes expandido (incluindo femininos comuns).
- **Novo**: Logs de auditoria persistentes em arquivo.
- **Novo**: Visualizador de texto RAW aprimorado (todas as páginas).
- **Melhoria**: Metadados de versão e fabricante no executável Windows.
- **UI**: Atualização de rodapé e ícones.

### v1.0.0
- Lançamento inicial.
- Separação por âncoras simples.
- Interface PySide6.

---

## Como Instalar

1. Baixe o arquivo `.exe` da versão desejada acima.
2. Execute o instalador e siga as instruções na tela.
3. O manual de utilização será instalado junto com o programa e há um atalho no Menu Iniciar.

---

**Licença:** Este software é distribuído sob os termos definidos no arquivo [LICENSE](./LICENSE).
**Desenvolvido por Conteris Team**
