<p align="center">
  <img src="./logo.png" width="280" alt="Conteris Logo"/>
</p>

# Conteris - Download Repository

Repositório oficial para distribuição dos instaladores do **Conteris - Gerenciador de PDFs**.

Aqui você encontra as versões compiladas para Windows do aplicativo.

## ⬇️ Downloads Disponíveis

> 🔒 **Arquivos protegidos por senha.**
> Entre em contato com a equipe para obter a senha de acesso.

### Versão Mais Recente
- [**Conteris v1.2.5 (ZIP)**](https://github.com/DiogoBenicio/conteris-download/releases/download/v1.2.5/Conteris_Installer_v1.2.5.zip) _(Recomendado)_

### Versões Anteriores
- [**Conteris v1.2.4 (ZIP)**](https://github.com/DiogoBenicio/conteris-download/releases/download/v1.2.4/Conteris_Installer_v1.2.4.zip)
- [**Conteris v1.2.3 (ZIP)**](https://github.com/DiogoBenicio/conteris-download/releases/download/v1.2.3/Conteris_Installer_v1.2.3.zip)
- [**Conteris v1.2.2 (ZIP)**](https://github.com/DiogoBenicio/conteris-download/releases/download/v1.2.2/Conteris_Installer_v1.2.2.zip)
- [**Conteris v1.2.1 (ZIP)**](https://github.com/DiogoBenicio/conteris-download/releases/download/v1.2.1/Conteris_Installer_v1.2.1.zip)
- [Conteris v1.1.1 (ZIP)](https://github.com/DiogoBenicio/conteris-download/releases/download/v1.1.1/Conteris_Installer_v1.1.1.zip)
- [Conteris v1.0.0 (ZIP)](https://github.com/DiogoBenicio/conteris-download/releases/download/v1.0.0/Conteris_Installer_v1.0.0.zip)

---

## 📝 Histórico de Versões

### v1.2.5 (Atual)
**NF – Grupos (novo sistema completo):**
- Tipos excluídos configuráveis — páginas com tipos marcados vão para *Páginas Excluídas* e não entram em nenhum grupo.
- Auto-grupos — tipos de página podem ser direcionados automaticamente a um grupo fixo nomeado, sem depender de separadores início/fim.
- Botão *Agrupar+* permite criar um novo grupo manualmente e arrastar páginas para ele via Drag & Drop.
- Ao criar um grupo via Agrupar+, um card de exportação é gerado automaticamente na seção de configuração.
- Grupos vazios são removidos automaticamente após mover todas as páginas; card de exportação removido junto.
- Grupos protegidos (*Sem Classificação* e *Páginas Excluídas*) nunca são removidos automaticamente.
- Sessão e grupos persistem ao salvar e reabrir o projeto — layout completo restaurado.
- Auto-grupos incluídos na seção de configuração de exportação.
- Redesign visual do card Separadores com hierarquia clara e alinhamento padronizado.

**NF – Algoritmo:**
- Modos só-início, só-fim e ambos funcionam corretamente com exclusões e auto-grupos.
- OverlayGroupPicker e grupo *Páginas Excluídas* corrigidos.

**Correções:**
- **ERR-6B64** (KeyError: 'row\_widget') eliminado ao carregar projetos no módulo NF.
- Splash screen sem borda cinza — logo renderizada via SVG nativo (QSvgRenderer).
- Ícone do .exe corrigido com ICO de fundo branco e path absoluto no spec.

**UI / Visual:**
- Fontes e ícones maiores em todos os módulos.
- Sombra suave nos ícones azul e vermelho da logo.

**Build:**
- `build_windows.bat` usa `pyzipper` — gera ZIP protegido sem precisar do 7-Zip.

**Manual:**
- Reescrito com estrutura completa, logo no cabeçalho e seção dedicada a Grupos.

**Testes:**
- Testes unitários para modelos, lógica de grupos e assets da logo adicionados.

### v1.2.4
- **Recurso**: Galeria de todas as páginas com visualização completa do PDF.
- **Recurso**: Âncoras secundárias configuráveis por tipo de página.
- **Recurso**: Extração inteligente de `{nome}` e `{empresa}` com reconhecimento automático.

### v1.2.3
- **Recurso**: Âncoras dinâmicas no Separador de NF — número ilimitado de âncoras por tipo de página; lógica OR por vírgula (ex: `"Nota Fiscal, NF-e"`).
- **Recurso**: Edição manual do tipo de página diretamente na interface.
- **UI**: Todas as seções de lista migradas para `QGridLayout` com cabeçalhos explicativos em ambos os módulos.
- **UI**: Modais e previews exibidos como overlay gráfico dentro da janela principal.
- **UI**: Overlays padronizados, FlowLayout corrigido e janela com scroll.
- **UI**: Animações suaves — fade nas transições, modais com deslizamento e escurecimento, feedback de clique nos cards.
- **Configuração**: Caminhos de PDF removidos das configurações JSON exportadas.
- **Correção**: Lógica de posicionamento de monitor removida — janelas abrem corretamente sem conflitos multi-monitor.
- **Build**: `build_windows.bat` corrigido (CRLF, log de diagnóstico, percentagens de progresso).

### v1.2.2
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

### v1.1.1
- **Novo**: Busca elástica (Fuzzy Matching) para nomes.
- **Novo**: Banco de dados de nomes expandido (incluindo femininos comuns).
- **Novo**: Logs de auditoria persistentes em arquivo.
- **Novo**: Visualizador de texto RAW aprimorado (todas as páginas).
- **Melhoria**: Metadados de versão e fabricante no executável Windows.

### v1.0.0
- Lançamento inicial.
- Separação por âncoras simples.
- Interface PySide6.

---

## Como Instalar

1. Baixe o arquivo `.zip` da versão desejada acima.
2. Extraia o `.zip` (senha fornecida pela equipe).
3. Execute o instalador `.exe` e siga as instruções na tela.
4. O manual de utilização será instalado junto com o programa e há um atalho no Menu Iniciar.

---

**Licença:** Este software é distribuído sob os termos definidos no arquivo [LICENSE](./LICENSE).
**Desenvolvido por Conteris Team**
