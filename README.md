# PMI-GO — downloads

Assistente do PMI/SPM (Sistema de Patrimônio Mobiliário) do Governo de Goiás · Polícia Civil do Estado de Goiás ·
uso interno.

O PMI-GO é um painel no próprio computador para consultar bens, ver o patrimônio da unidade, acompanhar o inventário,
gerar relatórios (Excel, CSV e Termo de Responsabilidade em PDF) e, se houver uma IA instalada, analisar a situação
da unidade. **O PMI-GO só lê o PMI; movimentação só com prévia e confirmação de quem usa.**

## Baixar a versão mais nova: 0.7.0

| Arquivo | Para quê | Tamanho |
|---|---|---|
| [**PMI-GO-Setup-0.7.0.exe**](https://github.com/windson83/pmi-go-versoes/releases/download/v0.7.0/PMI-GO-Setup-0.7.0.exe) | Instalador (já traz o Python) | 36 MB |
| [PMI-GO-Instalador-sem-exe-0.7.0.zip](https://github.com/windson83/pmi-go-versoes/releases/download/v0.7.0/PMI-GO-Instalador-sem-exe-0.7.0.zip) | Instalador sem .exe (se o Windows bloquear o Setup) | 34 MB |
| [PMI-GO-Manual.pdf](https://github.com/windson83/pmi-go-versoes/releases/download/v0.7.0/PMI-GO-Manual.pdf) | Manual do usuário, passo a passo com telas | 6 MB |
| [PMI-GO-Manual-Tecnico.pdf](https://github.com/windson83/pmi-go-versoes/releases/download/v0.7.0/PMI-GO-Manual-Tecnico.pdf) | Manual técnico, para a TI | 510 KB |

**Novidades da 0.7.0 — Relatório de movimentação de bens no período**

- Novo relatório em Relatórios: quais bens saíram da unidade (ou chegaram) num período — o bem, a unidade e a localização de destino, a data e onde ele está hoje — agrupado por tipo de bem, com subtotais.
- Período de/até ou por meses (por exemplo junho, julho e agosto de 2026); saídas ou entradas; realizadas ou pendentes; você desmarca as informações que não quer (como o tombamento anterior).
- Sai em PDF institucional, Excel (agrupado, resumo e tabela para tratar) e CSV; o nome da unidade, que o PMI corta, sai completo e as linhas repetidas pelo PMI aparecem uma vez só.
- Pelo Claude: "quais bens saíram da DTEL em julho?" (ferramenta pmi_movimentacoes, só leitura).
- O instalador e a atualização automática consertam sozinhos o pip 26.2.1, que no Windows impedia instalar ou atualizar o PMI-GO.

Todas as versões: [página de versões](https://github.com/windson83/pmi-go-versoes/releases).

## Como instalar

1. Baixe o **PMI-GO-Setup-0.7.0.exe** (link acima).
2. Dê dois cliques nele. Se o Windows avisar *"O Windows protegeu o computador"*, clique em **Mais informações** →
   **Executar assim mesmo**.
3. Clique em **Avançar** até o fim. Se o computador não tiver o Python, o instalador coloca sozinho
   (não precisa ser administrador). Leva de 2 a 6 minutos.
4. O painel abre no navegador: informe **o seu** CPF e a senha do Portal Goiás.
5. Pronto. O atalho **PMI-GO** fica no Menu Iniciar e na Área de Trabalho.

**O Windows bloqueou o Setup?** Se aparecer *"Uma política de Controle de Aplicativo bloqueou este arquivo"*
(Controle Inteligente de Aplicativos), use o [**PMI-GO-Instalador-sem-exe-0.7.0.zip**](https://github.com/windson83/pmi-go-versoes/releases/download/v0.7.0/PMI-GO-Instalador-sem-exe-0.7.0.zip): clique com o botão direito >
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
  (PowerShell: `Get-FileHash .\PMI-GO-Setup-0.7.0.exe -Algorithm SHA256`).

---

## Desenvolvimento e suporte

**Elder Windson Taveira Gonçalves** — Chefe da Divisão de Telecomunicações · Delegacia-Geral – DGPC  
✉ elder.windson@pc.goias.gov.br · ☏ (62) 3201-2592 · policiacivil.go.gov.br
