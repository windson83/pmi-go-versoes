# PMI-GO — downloads

Assistente do PMI/SPM (Sistema de Patrimônio Mobiliário) do Governo de Goiás · Polícia Civil do Estado de Goiás ·
uso interno.

O PMI-GO é um painel no próprio computador para consultar bens, ver o patrimônio da unidade, acompanhar o inventário,
gerar relatórios (Excel, CSV e Termo de Responsabilidade em PDF) e, se houver uma IA instalada, analisar a situação
da unidade. **O PMI-GO só lê o PMI; movimentação só com prévia e confirmação de quem usa.**

## Baixar a versão mais nova: 0.10.0

| Arquivo | Para quê | Tamanho |
|---|---|---|
| [**PMI-GO-Setup-0.10.0.exe**](https://github.com/windson83/pmi-go-versoes/releases/download/v0.10.0/PMI-GO-Setup-0.10.0.exe) | Instalador (já traz o Python) | 37 MB |
| [PMI-GO-Manual.pdf](https://github.com/windson83/pmi-go-versoes/releases/download/v0.10.0/PMI-GO-Manual.pdf) | Manual do usuário, passo a passo com telas | 7 MB |
| [PMI-GO-Manual-Tecnico.pdf](https://github.com/windson83/pmi-go-versoes/releases/download/v0.10.0/PMI-GO-Manual-Tecnico.pdf) | Manual técnico, para a TI | 621 KB |

**Novidades da 0.10.0 — Pesquisa por nota fiscal e tipo de bem clicando**

- Consultar bens: campo Nota fiscal — todos os bens da mesma nota, na sua unidade, em várias unidades ou no órgão inteiro, com ou sem pontos e zeros na frente (20.943 = 020943).
- Resumo da nota em cima da lista: data, série, bens, unidades, espécies, valor de aquisição e empenho; se o mesmo número for de compras diferentes, escolha a nota certa com um clique.
- Botão Tipo de bem: grupo → classe → espécie em três colunas, com quantos bens cada um tem; marque uma espécie (ex.: cadeira giratória), uma classe ou um grupo inteiro — ou procure pelo nome. A etiqueta mostra o caminho (grupo › classe).
- Unidade(s): a caixa das unidades fica à vista, para escolher uma ou várias; no órgão inteiro, os botões "unidade …" de Refinar levam a pesquisa para a unidade clicada. "Limpar tudo" ao lado das etiquetas.
- O filtro por espécie, grupo ou classe também acha os bens que vieram só da lista do órgão (sem o código da espécie).
- Pelo Claude: pmi_pesquisar ganhou nota_fiscal, nota_data, grupo, classe e especie; pmi_tipos_de_bem lista grupos, classes e espécies. Só leitura.

Todas as versões: [página de versões](https://github.com/windson83/pmi-go-versoes/releases).

## Como instalar

1. Baixe o **PMI-GO-Setup-0.10.0.exe** (link acima).
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
  (PowerShell: `Get-FileHash .\PMI-GO-Setup-0.10.0.exe -Algorithm SHA256`).

---

## Desenvolvimento e suporte

**Elder Windson Taveira Gonçalves** — Chefe da Divisão de Telecomunicações · Delegacia-Geral – DGPC  
✉ elder.windson@pc.goias.gov.br · ☏ (62) 3201-2592 · policiacivil.go.gov.br
