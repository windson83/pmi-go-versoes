# PMI-GO — downloads

Assistente do PMI/SPM (Sistema de Patrimônio Mobiliário) do Governo de Goiás · Polícia Civil do Estado de Goiás ·
uso interno.

O PMI-GO é um painel no próprio computador para consultar bens, ver o patrimônio da unidade, acompanhar o inventário,
gerar relatórios (Excel, CSV e Termo de Responsabilidade em PDF) e, se houver uma IA instalada, analisar a situação
da unidade. **O PMI-GO só lê o PMI; movimentação só com prévia e confirmação de quem usa.**

## Baixar a versão mais nova: 0.9.0

| Arquivo | Para quê | Tamanho |
|---|---|---|
| [**PMI-GO-Setup-0.9.0.exe**](https://github.com/windson83/pmi-go-versoes/releases/download/v0.9.0/PMI-GO-Setup-0.9.0.exe) | Instalador (já traz o Python) | 37 MB |
| [PMI-GO-Instalador-sem-exe-0.9.0.zip](https://github.com/windson83/pmi-go-versoes/releases/download/v0.9.0/PMI-GO-Instalador-sem-exe-0.9.0.zip) | Instalador sem .exe (se o Windows bloquear o Setup) | 35 MB |
| [PMI-GO-Manual.pdf](https://github.com/windson83/pmi-go-versoes/releases/download/v0.9.0/PMI-GO-Manual.pdf) | Manual do usuário, passo a passo com telas | 7 MB |
| [PMI-GO-Manual-Tecnico.pdf](https://github.com/windson83/pmi-go-versoes/releases/download/v0.9.0/PMI-GO-Manual-Tecnico.pdf) | Manual técnico, para a TI | 594 KB |

**Novidades da 0.9.0 — Painel interativo do patrimônio**

- Tela Patrimônio com painel interativo (como no Power BI): clique no grupo (ex.: Bens de informática), na espécie (ex.: webcam) e veja em qual sala, setor ou estoque ela está; cada clique filtra todos os quadros.
- "Todas as unidades": o mesmo painel no órgão inteiro, com o quadro Unidade — por exemplo, onde estão todos os rádios. Mostra o que o índice do órgão tem (lido do PMI com o seu login).
- Caixa "Procurar item" (webcam, rádio, notebook…), faixa com os filtros escolhidos (✕ para tirar), indicadores e a lista de bens do que está filtrado, com "Baixar planilha (CSV)".
- A lista completa do Termo de Responsabilidade continua, na aba "Lista completa (Termo)".
- Relatório de movimentação: novo filtro Item (ex.: "webcam; rádio") para trazer só esses bens.
- Pelo Claude: ferramenta pmi_onde_esta (onde estão hoje os bens de um item, na unidade ou no órgão) e o parâmetro itens em pmi_movimentacoes. Só leitura.

Todas as versões: [página de versões](https://github.com/windson83/pmi-go-versoes/releases).

## Como instalar

1. Baixe o **PMI-GO-Setup-0.9.0.exe** (link acima).
2. Dê dois cliques nele. Se o Windows avisar *"O Windows protegeu o computador"*, clique em **Mais informações** →
   **Executar assim mesmo**.
3. Clique em **Avançar** até o fim. Se o computador não tiver o Python, o instalador coloca sozinho
   (não precisa ser administrador). Leva de 2 a 6 minutos.
4. O painel abre no navegador: informe **o seu** CPF e a senha do Portal Goiás.
5. Pronto. O atalho **PMI-GO** fica no Menu Iniciar e na Área de Trabalho.

**O Windows bloqueou o Setup?** Se aparecer *"Uma política de Controle de Aplicativo bloqueou este arquivo"*
(Controle Inteligente de Aplicativos), use o [**PMI-GO-Instalador-sem-exe-0.9.0.zip**](https://github.com/windson83/pmi-go-versoes/releases/download/v0.9.0/PMI-GO-Instalador-sem-exe-0.9.0.zip): clique com o botão direito >
**Extrair tudo**, abra a pasta e dê dois cliques em **Instalar PMI-GO.cmd**. Instala o mesmo PMI-GO pelo Python
oficial, que o Windows permite.

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
  (PowerShell: `Get-FileHash .\PMI-GO-Setup-0.9.0.exe -Algorithm SHA256`).

---

## Desenvolvimento e suporte

**Elder Windson Taveira Gonçalves** — Chefe da Divisão de Telecomunicações · Delegacia-Geral – DGPC  
✉ elder.windson@pc.goias.gov.br · ☏ (62) 3201-2592 · policiacivil.go.gov.br
