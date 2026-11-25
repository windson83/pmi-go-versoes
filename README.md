# PMI-GO — downloads

Assistente do PMI/SPM (Sistema de Patrimônio Mobiliário) do Governo de Goiás · Polícia Civil do Estado de Goiás ·
uso interno.

O PMI-GO é um painel no próprio computador para consultar bens, ver o patrimônio da unidade, acompanhar o inventário,
gerar relatórios (Excel, CSV e Termo de Responsabilidade em PDF) e, se houver uma IA instalada, analisar a situação
da unidade. **O PMI-GO só lê o PMI; movimentação só com prévia e confirmação de quem usa.**

## Baixar a versão mais nova: 0.11.1

| Arquivo | Para quê | Tamanho |
|---|---|---|
| [**PMI-GO-Setup-0.11.1.exe**](https://github.com/windson83/pmi-go-versoes/releases/download/v0.11.1/PMI-GO-Setup-0.11.1.exe) | Instalador (já traz o Python) | 38 MB |
| [PMI-GO-Manual.pdf](https://github.com/windson83/pmi-go-versoes/releases/download/v0.11.1/PMI-GO-Manual.pdf) | Manual do usuário, passo a passo com telas | 7 MB |
| [PMI-GO-Manual-Tecnico.pdf](https://github.com/windson83/pmi-go-versoes/releases/download/v0.11.1/PMI-GO-Manual-Tecnico.pdf) | Manual técnico, para a TI | 629 KB |

**Novidades da 0.11.1 — Relatórios em abas e filtros de clicar na nota fiscal**

- Relatórios e arquivos em três abas, uma para cada tipo: Patrimônio da unidade, Movimentação no período e Nota fiscal (a última usada fica aberta). O campo Unidade só aparece onde vale.
- Nota fiscal com os 3 passos do relatório de movimentação: depois de Procurar a nota, os filtros mostram o que existe nela (unidade onde está hoje, tipo de bem, sala, situação, ano de aquisição) com quantos bens tem cada um, para só marcar ou desmarcar; também item e data de aquisição.
- Contagem na hora: "Com os filtros: 84 de 294 bens"; a contagem de cada opção já considera os outros filtros. O que fica de fora nem tem o histórico lido (mais rápido).
- Colunas escolhidas (o tombamento sempre aparece), as mesmas na tela, no PDF, no Excel e no CSV.
- Pelo Claude: pmi_relatorio_nota aceita itens, espécies, unidades onde está hoje, anos de aquisição e colunas.

Todas as versões: [página de versões](https://github.com/windson83/pmi-go-versoes/releases).

## Como instalar

1. Baixe o **PMI-GO-Setup-0.11.1.exe** (link acima).
2. Dê dois cliques nele. Se o Windows avisar *"O Windows protegeu o computador"*, clique em **Mais informações** →
   **Executar assim mesmo**.
3. Clique em **Avançar** até o fim. Se o computador não tiver o Python, o instalador coloca sozinho
   (não precisa ser administrador). Leva de 2 a 6 minutos.
4. O painel abre no navegador: informe **o seu** CPF e a senha do Portal Goiás.
5. Pronto. O atalho **PMI-GO** fica no Menu Iniciar e na Área de Trabalho.

**O Windows bloqueou o Setup?** Se aparecer *"Uma política de Controle de Aplicativo bloqueou este arquivo"*
(Controle Inteligente de Aplicativos), fale com o suporte (contato no fim da página): há um instalador alternativo,
entregue sob pedido.

## Como atualizar

O PMI-GO confere se há versão nova quando o painel abre. Se houver, baixa daqui, confere a assinatura digital e
instala; o painel reinicia em 1 a 3 minutos. Se preferir decidir a hora, desligue a instalação automática na
configuração do painel: ele mostra o aviso **"Saiu o PMI-GO x.y.z"** com o botão **Atualizar agora**. Seu login e
suas configurações continuam. O arquivo `PMI-GO-atualizacao-x.y.z.bin` de cada versão é o pacote da atualização
automática: não precisa baixá-lo.

## Segurança

- Baixe o PMI-GO **só desta página**.
- A senha do Portal Goiás é digitada no próprio painel e fica no cofre do Windows. Ninguém do suporte e nenhuma IA
  pede a sua senha.
- O PMI-GO só se atualiza sozinho com pacote baixado desta página **e assinado digitalmente** pelo PMI-GO; se a
  instalação falhar, ele volta para a versão anterior. Nunca pede senha para atualizar.
- Para conferir se o arquivo chegou íntegro, compare o hash SHA-256 com o `SHA256SUMS.txt` da versão
  (PowerShell: `Get-FileHash .\PMI-GO-Setup-0.11.1.exe -Algorithm SHA256`).

---

## Desenvolvimento e suporte

**Elder Windson Taveira Gonçalves** — Chefe da Divisão de Telecomunicações · Delegacia-Geral – DGPC  
✉ elder.windson@pc.goias.gov.br · ☏ (62) 3201-2592 · policiacivil.go.gov.br
