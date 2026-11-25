# PMI-GO — downloads

Assistente do PMI/SPM (Sistema de Patrimônio Mobiliário) do Governo de Goiás · Polícia Civil do Estado de Goiás ·
uso interno.

O PMI-GO é um painel no próprio computador para consultar bens, ver o patrimônio da unidade, acompanhar o inventário,
gerar relatórios (Excel, CSV e Termo de Responsabilidade em PDF) e, se houver uma IA instalada, analisar a situação
da unidade. **O PMI-GO só lê o PMI; movimentação só com prévia e confirmação de quem usa.**

## Baixar a versão mais nova: 0.11.0

| Arquivo | Para quê | Tamanho |
|---|---|---|
| [**PMI-GO-Setup-0.11.0.exe**](https://github.com/windson83/pmi-go-versoes/releases/download/v0.11.0/PMI-GO-Setup-0.11.0.exe) | Instalador (já traz o Python) | 38 MB |
| [PMI-GO-Manual.pdf](https://github.com/windson83/pmi-go-versoes/releases/download/v0.11.0/PMI-GO-Manual.pdf) | Manual do usuário, passo a passo com telas | 7 MB |
| [PMI-GO-Manual-Tecnico.pdf](https://github.com/windson83/pmi-go-versoes/releases/download/v0.11.0/PMI-GO-Manual-Tecnico.pdf) | Manual técnico, para a TI | 624 KB |

**Novidades da 0.11.0 — Relatório de uma nota fiscal**

- Relatórios e arquivos: novo relatório de uma nota fiscal — todos os bens da nota, onde cada um está hoje (unidade e localização) e o caminho de cada um, com data, nº da movimentação, unidade e sala de destino.
- Na sua unidade, em várias ou no órgão inteiro; Procurar a nota mostra as notas com esse número (compras diferentes) para escolher uma ou todas.
- Agrupar por unidade onde está hoje, localização ou tipo de bem; situação todas ou só ativos; com ou sem o histórico de movimentação (o lido fica guardado e as próximas vezes são rápidas).
- PDF, Excel (abas Bens da nota, Movimentações, por unidade, localização, espécie e situação) e CSV.
- Pelo Claude: ferramenta pmi_relatorio_nota. Só leitura.

Todas as versões: [página de versões](https://github.com/windson83/pmi-go-versoes/releases).

## Como instalar

1. Baixe o **PMI-GO-Setup-0.11.0.exe** (link acima).
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
  (PowerShell: `Get-FileHash .\PMI-GO-Setup-0.11.0.exe -Algorithm SHA256`).

---

## Desenvolvimento e suporte

**Elder Windson Taveira Gonçalves** — Chefe da Divisão de Telecomunicações · Delegacia-Geral – DGPC  
✉ elder.windson@pc.goias.gov.br · ☏ (62) 3201-2592 · policiacivil.go.gov.br
