# Como usar o index.html

Manual de uso. Atualizado em **26/11/2026**.

As regras de comportamento e os limites de cada aparelho estão em
`claude/regras_de_trabalho.md`. O que **não pode mudar** sem você mandar está
em `claude/o_que_ja_esta_certo.md`. A limpeza dos brutos está em
`claude/vassoura_brutos.md`.

O trabalho hoje é no **Windows**, mais iPad e iPhone na gravação. As partes
sobre Mac estão guardadas aqui para quando a equipe migrar.

---

## Onde o site mora

```
repositório:  otimizacao_cc
endereço:     krettlibruna.github.io/otimizacao_cc/
```

O repositório foi **renomeado em 12/11/2026** — antes era
`otimizacao_cifra_club`. O `gerador_tp_fluxo_cifra`, mais antigo, **não existe
mais**. Se algum desses dois nomes aparecer em algum lugar, está desatualizado.

## Abrir e atualizar

- **Para usar:** sempre pelo endereço acima. No iPad e no iPhone é obrigatório
  abrir pelo site — arquivo baixado não roda lá.
- **Para atualizar:** no repositório `otimizacao_cc`, *Add file → Upload files
  → Commit changes*, substituindo o `index.html`.
- O arquivo tem ~2,2 MB porque as bibliotecas vêm embutidas. Por isso funciona
  no 4G, no wi-fi da empresa e offline depois de carregar.

### Depois de subir, como fazer o aparelho pegar a versão nova

**Primeiro, o jeito simples:**

- **iPad e iPhone:** puxar a página pra baixo. Na maioria das vezes resolve.
- **Computador:** Ctrl+F5 (Cmd+Shift+R no Mac).

Se a novidade não aparecer, são dois motivos possíveis:

1. **O GitHub ainda não publicou.** Leva um ou dois minutos depois do Commit.
   Espera um pouco e puxa de novo.
2. **O navegador insistiu na versão guardada.** Acontece mais quando você abre
   pelo ícone da tela de início em vez do Safari.

**A garantia, para o segundo caso:** acrescentar `?v=` e um número ao fim do
endereço.

```
krettlibruna.github.io/otimizacao_cc/?v=37
```

**O número só precisa ser diferente do último que você usou.** Pode seguir em
ordem: 37, 38, 39… Funciona nos três aparelhos.

> **O último número anotado aqui foi `?v=36`, em 29/10.** Se você subiu versões
> depois disso sem anotar, siga a partir do que usou por último — e anote o
> novo nesta linha.

### Como saber se o que está no ar é a versão nova

Não existe marca de versão na tela (de propósito: o cabeçalho fica limpo).
Confira assim:

1. **No GitHub**, o `index.html` tem que estar com **~2,2 MB** e a data do
   commit de hoje. Arquivo bem menor que isso é versão antiga.
2. **Pela tela**, a versão de 26/11 tem:
   - a **logo nova** (adesivo: violão e "cifraclub" com contorno branco)
   - o botão **+ uma cena** embaixo da tabela de cenas, **no fluxo Padrão**
   - **nenhuma caixa amarela** quando a tabela de cenas está vazia
   - **5000K** na lista de Kelvin da microaula
   - um PDF com roteiro de reels entra **sem** as cenas do reels

No alto da página: a logo do Cifra Club à esquerda, **🌙 Escuro / ☀️ Claro** à
direita, e **Limpar tudo** zera as três abas. Cada aba tem o seu **Limpar esta
aba** embaixo — e na aba Fluxo ele zera **os três modelos** daquela aula, que é
o certo, porque os três são o mesmo fluxo visto de jeitos diferentes.

---

## O que sai quando você aperta Salvar

**Um arquivo só:**

```
nome_da_aula.pdf
```

Na microaula o nome sai como **dia_mês_instrutor** — `10_11_caico.pdf` —, a
partir da data de gravação e do instrutor que estiverem preenchidos.

Não existe arquivo json separado. O fluxo inteiro viaja **dentro do próprio
PDF**, numa ficha de informações que ninguém vê. É por isso que o *Abrir fluxo
do iCloud* consegue abrir o PDF e devolver tudo preenchido.

- **No computador** (Chrome/Edge): cai direto na pasta que você escolheu. Ele
  só pergunta a pasta na primeira vez.
- **No iPad e no iPhone**: abre a folha de compartilhamento do sistema. Você
  toca em *Salvar em Arquivos* e ele cai no iCloud.

Uma ressalva: se alguém abrir esse PDF em outro programa e **salvar por cima**,
a ficha escondida pode se perder. O PDF continua valendo como folha, mas aí não
abre mais como fluxo. Arquivos `.json` que você salvou antes continuam abrindo
normalmente.

---

## Quando você vai usar cada coisa — a semana típica

**Segunda, no Windows.** Aba TP: sobe o roteiro em PDF, confere as cenas, copia
os nomes, baixa o `.tpp`. Aba Fluxo: escolhe o tipo de fluxo, preenche nome do
vídeo, instrutor, estúdio, data, as câmeras. Aperta **Salvar** e escolhe uma
pasta **dentro do iCloud** — essa escolha é uma vez só, ele lembra depois.

**Terça, no estúdio, no iPad.** Abre o site. Ele está em branco, porque o
preenchimento de ontem mora no navegador do computador e não viaja. Aperta
**Abrir fluxo do iCloud**, escolhe o PDF da aula, e a folha volta inteira —
inclusive se a diária já foi lançada. Durante a gravação marca os takes e as
observações. No fim, **Salvar** → a folha de compartilhamento → *Salvar em
Arquivos*.

**Quinta, de volta no Windows, faltou uma observação.** Se for a mesma máquina
de segunda, o preenchimento ainda está lá e é só continuar. Se for outra
máquina — ou se você tiver limpado a aba —, **Abrir fluxo do iCloud** → escolhe
o PDF → acrescenta → **Salvar** de novo.

**Com os dois aparelhos ligados ao mesmo tempo**, dá pra pular o arquivo:
*Continuar em outro aparelho* mostra um QR que leva o fluxo direto pro iPad.
O *Abrir fluxo* é pro resto das vezes, quando o outro aparelho está desligado —
e continua disponível mesmo depois de você ter entrado pelo QR.

---

## Aba TP

1. **Subir o roteiro** — arrastar o PDF para a área pontilhada, ou tocar e
   escolher. Ctrl+V também funciona. Sem PDF, abrir *Colar ou editar o roteiro
   à mão*.
2. **Nome da aula** — a página monta **Nome pro TP** e **Nome pro Fluxo**, cada
   um com seu **Copiar**.
3. **Conferir as cenas** — LOC, ACORDES, RITMO, DEDIL, TAB, TOCA e TOCA SOLO na
   ordem.
4. **Ajustar à mão** — os botões de tipo trocam o tipo da cena. **Inserir cena**
   põe uma cena onde o cursor está. **Renumerar** arruma a numeração.
   **↶ Desfazer** e **↷ Refazer**.
5. **Baixar .tpp pro Teleprompter**, ou **Salvar na pasta…** pra gravar direto.

### Vários roteiros no mesmo PDF

Um arquivo pode trazer `ROTEIRO DO YOUTUBE`, `ROTEIRO DO SITE`, `ROTEIRO DO
REELS` e `ROTEIRO DO SHORTS`.

- **YouTube e site entram juntos**, cada um com a sua numeração, separados por
  uma divisória.
- **Reels e shorts são ignorados inteiros** *(desde 26/11)*. São outro produto:
  vêm com cabeçalho próprio e a própria numeração — um LOC 01 e um TOCA 01 que
  repetem os do YouTube. Não entram no campo do roteiro, nem na contagem de
  cenas, nem no `.tpp`, nem no fluxo.

O recado depois de ler o PDF diz quantos roteiros entraram, por exemplo:
*"Conferi os 2 roteiros do arquivo e juntei todos: YOUTUBE (3) + SITE (17) =
20 cenas"*.

### O que ele lê do cabeçalho do roteiro

| o que o roteiro diz | para onde vai |
|---|---|
| `Nome: Açaí - Djavan` | nome da aula |
| `Tipo: Simplificada` | a versão — mas quem decide se ela entra no nome é o instrumento |
| `Apresentador: Gustavo Vaz` | instrutor do fluxo (vira "Vaz") |
| `Bpm da música: 120` | BPM toca |
| `BPM: 50` | BPM ensina |

### A versão no nome — quem manda é o instrumento

*(Regra sua, 26/11.)* A versão só existe para separar duas gravações da mesma
música. Onde não há duas, ela só atrapalha o nome.

| instrutor | o que entra no nome |
|---|---|
| **Guitarra** — Vini, Tarsius | **nunca** entra versão: guitarra é sempre única |
| **Violão** — Fofão, Vaz, Caico | entra **sempre**: `(Completa)`, `(Simplificada)`, ou `(Versão Única)` quando o roteiro não disser outra coisa |
| **Noel**, ou instrutor que o site não conhece | só o que estiver **escrito** no roteiro — sem instrumento ele não supõe nada |

**Nada é deduzido.** `Completa` só sai se estiver escrito `Completa` — e
"Completa" só existe quando existe uma Simplificada. Se o roteiro não diz nada,
é versão única.

**Ele lê todas as linhas `Tipo:` do arquivo** e fica com a primeira que seja
mesmo uma versão. Num PDF de três roteiros vêm três — `Reels`, `Youtube` e
`Completa` — e só a última é versão.

> **Exemplo:** no roteiro do Voodoo Child (Vini, guitarra) está escrito
> `Tipo: Completa` no roteiro do site. O nome sai **`Voodoo Child`**, sem
> versão, porque guitarra nunca leva — aquele "Completa" é sobra de modelo.

**Por que isso importa:** a vassoura de brutos trata Completa e Simplificada
como duas aulas diferentes, e só distingue pela palavra escrita. Sem ela, as
duas viram uma só na planilha e uma pode ser apagada no lugar da outra.

**Um limite:** o nome é montado **na hora de ler o PDF**. Se você trocar o
instrutor no fluxo depois, o nome **não** se renomeia sozinho — corrija o campo
do nome à mão.

---

## Aba Fluxo

No topo, acima do nome do vídeo, sai a logo do Cifra Club — ela vai junto no
PDF.

### Tipo de fluxo

- **Padrão** — `D · Cena · Cam · Take(s) · Observações`.
- **Várias diárias** — acrescenta a coluna `Data de gravação`, o bloco
  *Arquivos por diária* e o campo **Quantas diárias**.
- **Desafio, review, editorial e insert** — vêm sem roteiro; as cenas você
  mesma cria (ver abaixo).
- **Microaula** — a leva inteira de um dia. Não usa roteiro: você cola os nomes
  das músicas e ele monta a lista, com **Fundo**, **Recorte**, instrumento e
  diagrama em cada linha, e **Data de gravação** no cabeçalho. Dá pra escolher
  **dois fundos** na mesma aula pelo **+**.

### Acrescentar uma cena que o roteiro esqueceu

*(Novo em 24/11.)* O botão **+ uma cena** fica embaixo da tabela, **no Padrão e
no Várias diárias** — serve para quando o roteiro veio sem uma cena que você
gravou. Escreve o tipo e, **ao sair do campo**, ela se acomoda sozinha.

**O número que você escreve é que manda o lugar:**

| você escreve | o que acontece |
|---|---|
| `LOC` | ganha o próximo número livre e fica embaixo de todas as LOC |
| `loc 3`, numa folha com 7 LOCs | vira **LOC 03** e **toma o lugar do 3**: o LOC 03 antigo vira 04, o 04 vira 05, até o 07 virar 08 |
| `TOCA`, num roteiro sem nenhuma TOCA | vai para o fim, que é onde dá pra achar |

- **Número de cena é sempre de dois algarismos** — 01, 02, 03, nunca 1, 2, 3 —
  e sempre em maiúscula. Você escreve `loc 3`, a folha mostra `LOC 03`.
- **A renumeração empurra só o mesmo tipo.** Entrar uma LOC não mexe nos
  ACORDES nem nos TOCA.
- **O que já estava escrito vai junto.** O CAM, o take e as observações do
  LOC 03 antigo acompanham ele quando ele vira LOC 04.
- **O roteiro da aba TP não é renumerado** — se precisar, você acerta aquela
  parte à mão.

**Para tirar a cena**, o **×** embaixo do nome, com dois toques (o primeiro
vira "tirar?", o segundo apaga). Ele some sozinho assim que você escreve
alguma coisa na linha, para não ficar no caminho; um toque no nome da cena faz
ele voltar.

Um caso que ainda não está resolvido: numa folha com **dois roteiros** (YouTube
e site), os dois começam no LOC 01, e escrever `LOC 2` põe a cena no bloco do
**primeiro**. Para cair no do site, escreva um número que só exista lá.

### Cenas sem roteiro — desafio, review, editorial e insert

Escolhendo um desses tipos aparece também a caixa **"Cenas — escreva quantas de
cada"**. Escreva `3 LOCS e 2 TOCAS` e ele cria as cenas numeradas. Essa caixa
**só aparece nesses quatro tipos** — na vídeo aula fica só o `+ uma cena`, para
não encher a tela de uma folha que já veio pronta.

Essas cenas também alimentam a tabela **Arquivos por diária** — ela lê o TP
quando tem TP, e lê o fluxo quando não tem.

### Preenchimento que se espalha sozinho

- **Cam** — preencher a **primeira linha de um grupo** repete o número no grupo
  todo. Mexer no meio muda só aquela linha; voltar na primeira refaz o grupo.
- **Cam com mais de uma câmera** — escreve com vírgula: `5,6`. No iPhone e no
  iPad o teclado de números abre com a tecla de separador; se o aparelho
  estiver num idioma que põe ponto nela, **o ponto vira vírgula sozinho**.
  *(Corrigido em 24/11 — antes não dava pra pôr duas câmeras no celular.)*
- **Data de gravação** — igual à Cam.
- **Arquivo** — **RITMO, DEDIL, TAB, TOCA e TOCA SOLO dividem o mesmo número**:
  escrever em qualquer uma preenche as outras.
- **Arquivo do ACORDES** — ali você costuma pôr dois, tipo `1234 +12345`. O
  ACORDES guarda os dois e manda **só o segundo** para as cenas acima. Se o
  roteiro não tiver ACORDES, continua como sempre: preenche numa cena e as
  outras seguem. A **LOC** fica de fora dos dois casos.
- Nas várias diárias tudo isso segue a regra das alterações: 1ª vale pra todas,
  2ª daquela em diante, 3ª só naquela.
- **Coluna D** — clicar na célula vira 1ª / 2ª / 3ª diária e pinta a linha.

### Apagar vários campos de uma vez

Vale na tabela de cenas, na tabela *Arquivos por diária* e nos cartões das
diárias. Cada bloco conta sozinho.

- **Computador:** arrastar o mouse e apertar Delete ou Backspace.
- **iPhone/iPad:** **dois toques rápidos no mesmo campo** acendem ele, **um
  toque no último** fecha a faixa, e o **apagar do teclado** limpa tudo. Dá pra
  rolar a tela entre um toque e o outro.
- Começar a digitar desfaz a marcação. Com um campo só, apagar é letra por
  letra.

### Outros atalhos no computador

| O quê | Como |
|---|---|
| Subir e descer de linha | setas ↑ e ↓ |
| Andar no texto e pular de campo na ponta | setas ← e → |
| Desfazer a marcação | Esc, ou clicar fora |

### Botões

- **Salvar** — ver a seção acima.
- **Trocar pasta** — muda a pasta de destino no computador.
- **Abrir fluxo do iCloud** — carrega um fluxo salvo antes. Escolha o **PDF**
  da aula; `.json` e `.fluxo` antigos também abrem. Abre o arquivo de onde ele
  estiver — você pode mover e renomear à vontade, a página nunca vai procurá-lo
  sozinha.
- **Refazer do roteiro** — monta a lista de cenas de novo a partir da aba TP.
- **Continuar em outro aparelho** — QR e link que levam o fluxo preenchido pro
  iPad ou celular. O QR precisa ser gerado **a partir do site**.

O preenchimento também fica guardado no navegador, por aula: fechar e voltar na
mesma máquina não perde nada.

### Como o agrupamento da microaula decide os blocos

O botão de agrupar junta as aulas pela montagem de luz, nesta ordem:

1. Primeiro os fundos que são **só cor**, um bloco por cor, em fila do mais
   quente para o mais frio. Preto fica no fim dessa fila.
2. Depois **tudo que tem Detalhe Fresnel com alguma cor**, num bloco só,
   ordenado pelo Kelvin do Fresnel — porque montar e apontar o Fresnel é o
   trabalho, e trocar a cor do fundo é um toque no painel.
3. Depois o **Fresnel sozinho**, sem cor nenhuma, que é outra montagem.
4. Depois os **grids**, um bloco por código (C007, C009), cada um juntando as
   cores que usaram aquele grid.
5. No fim, as aulas que ainda não têm fundo escolhido.

Ele reconhece a mesma cor escrita de jeitos diferentes: "Laranja H:53 S:90
I:70" e "alaranjado" caem no mesmo bloco; preto, apagado e desligado também.

Os Kelvin disponíveis: **2800K, 3000K, 3500K, 4000K, 5000K, 6000K**.
*(O 5000K entrou em 24/11.)*

---

## Lançar diária nas planilhas

No fim da aba Fluxo. Preenche de uma vez as duas planilhas do Google — a
**Diária Offload** (sua e da Samira) e o **sprint** (da chefia) — sem copiar e
colar.

O site não entra em conta nenhuma: ele manda a diária para um script que mora
dentro da própria planilha, e é o script que escreve, como você.

### Não tem nada pra configurar

O link do script fica **embutido no próprio `index.html`**. Todo aparelho que
abrir o site já está pronto: computador, iPad, iPhone, o aparelho da Samira.
Se um dia o link mudar, é um `index.html` novo e todos passam a usar o novo de
uma vez.

Uma consequência disso: o link está dentro de um arquivo público no GitHub.
Quem achar o repositório consegue acrescentar linhas nessas duas planilhas —
não dá acesso a conta nenhuma, não lê e não apaga nada, mas vale saber.

### Usando

O bloco já vem preenchido a partir do fluxo: data da diária, aba da offload,
status e a lista de aulas. Confere, corrige se quiser, clica em **Lançar
diária**. O recado embaixo diz o que aconteceu.

- **Offload:** uma linha por diária. Se a diária daquele dia já existe, ele
  **soma** as aulas novas na mesma célula, embaixo das que já estavam.
- **Sprint:** uma linha por aula, na aba do mês, com Produto, Canal, Tipo,
  Instrutor, Tarefa e Status (Done por padrão, To do na lista).
- Microaula vai como `Social Media · microaula`; vídeo aula como
  `YouTube · videoaula`; desafio, review e editorial como `editorial`.
- **Insert vai só pra offload** — o sprint não recebe nada.
- Se a aba ou o mês não existirem, ele avisa e não escreve nada.
- Se o envio direto não passar, ele abre uma aba que faz a mesma coisa e mostra
  o resultado. Acontece mais no Safari. Fecha a aba e segue.

### Depois de lançar *(novo em 24/11)*

**O fluxo guarda que foi lançado.** Acima do botão aparece
`✓ Esta diária já foi lançada`, em verde. Sem data, sem hora, sem recado de
planilha — só o fato.

Como isso mora **dentro do fluxo**, e o fluxo viaja dentro do PDF, **abrir o
mesmo fluxo no iPad ou no celular já mostra que foi lançada**. Você não precisa
lembrar de onde lançou.

**O botão trava quando é exatamente a mesma diária:**

| o que está na tela | botão |
|---|---|
| igual ao que foi lançado | travado |
| mesma aula, sem acento ou com outra caixa | travado |
| outra aula, ou outra data | liberado |
| depois de Limpar esta aba | liberado |

### Não duplicar na planilha *(novo em 24/11, versão 5 do script)*

A trava do botão protege o aparelho onde você lançou. Quem protege de verdade é
**o script da planilha**, porque ele vê o que já está escrito lá venha de onde
vier. Ele compara ignorando **acento, maiúscula e pontuação** — antes guardava
a pontuação, e por isso `Açaí - Djavan (Simplificada)` e
`Açaí - Djavan Simplificada` entravam como duas aulas.

**Quando as duas escritas são a mesma aula, fica a mais completa**, e o script
**corrige a planilha** em vez de criar outra linha:

1. ganha quem tem a **versão entre parênteses**
2. empatou: quem tem **mais acentos**
3. empatou de novo: a **mais comprida**

O recado volta dizendo quantos nomes foram corrigidos.

> **Aula sem versão não é a mesma que a versionada.** `Skyfall - Adele` e
> `Skyfall - Adele (Completa)` continuam sendo duas aulas — se virassem uma, a
> trava de versão da vassoura de brutos cairia.

> **De olho no primeiro lançamento de violão depois de 26/11:** aula de violão
> que antes saía sem versão agora sai `(Versão Única)`. Como quem tem
> parênteses ganha, o script vai **corrigir** as linhas antigas dessas aulas
> para a forma nova. É o esperado, mas vale conferir na primeira vez.

### Como o script foi montado (para refazer, se precisar)

Passo a passo completo no arquivo `passo-a-passo-lancar-diaria.md`, entregue
junto com o script `lancar-diaria.gs`. Em resumo:

1. Pegar o **ID** das duas planilhas (o pedaço do link entre `/d/` e `/edit`).
2. Na planilha de offload: *Extensões → Apps Script*, colar o script, trocar os
   dois IDs lá no alto, salvar.
3. *Implantar → Nova implantação → App da Web*, executar como **Eu**, acesso
   para **Qualquer pessoa**. Autorizar. Copiar o URL.

**Para mudar o script depois sem perder o link:** *Implantar → Gerenciar
implantações → lápis → Versão: Nova versão → Implantar*. Fazer por "Nova
implantação" gera um link diferente e quebra o site até o link novo ser
embutido.

---

## Para o iCloud ficar automático

- **Windows** (o caso de hoje): escolher, no Salvar, uma pasta dentro de
  `C:\Users\<você>\iCloudDrive\…`. Tudo que cair lá sobe sozinho.
- **iPad/iPhone:** abrindo pelo **Safari** (não pelo ícone da tela de início)
  com *Ajustes → Safari → Downloads → iCloud Drive*, o download cai no iCloud
  sozinho. Pelo ícone da tela de início, a folha de compartilhamento é o
  caminho.
- **Mac — para quando a equipe migrar:** o Chrome **recusa** a pasta do iCloud
  ("contém arquivos do sistema"), porque ela mora dentro de `~/Library`. Não há
  como contornar pelo site. A volta é apontar os downloads do Chrome pro
  iCloud, em *Chrome → Configurações → Downloads → Alterar*. Fora isso, tudo o
  mais funciona igual ao Windows, desde que seja Chrome ou Edge — o Safari de
  computador não tem a aba Pós Prod. nem o salvar em pasta.

---

## Aba Pós Prod.

Só funciona no Chrome ou Edge **de computador**. O iPad e o iPhone não têm o
recurso de acesso a pastas que ela usa.

1. **Escolher pasta da aula** — depois disso o **Procurar áudio export** fica
   disponível. A pasta fica lembrada entre as sessões, mas o navegador pede
   para liberar o acesso de novo a cada vez; é o aviso âmbar *"Pasta lembrada:
   … Clique em Escolher pasta da aula para liberar"*.
2. **Arrastar os arquivos**:
   - **XML do DaVinci** → converte e salva em `premiere/`
   - **Projeto de áudio** → o conteúdo da pasta vai para `sonar/`, sem a pasta
     de fora
   - **Fluxo (iCloud)** → renomeia o arquivo para `fluxo` e salva na raiz
3. **Procurar áudio export** — este é automático, não se arrasta nada. Procura
   sozinho a pasta de áudio exportado (dentro de `sonar/`, ou da pasta da aula
   se não houver `sonar/`), desce até 6 níveis atrás de uma pasta com "export"
   e "audio" no nome, e **copia os arquivos para `Assets/`**, sem recriar as
   subpastas.

O painel de acompanhamento mostra as quatro etapas de cada aula:

```
○ XML → premiere/      ○ pendente   ⋯ na fila
⋯ Projeto de áudio → sonar/        ◔ andando
◔ Áudio exportado → Assets/        ✓ feito
✓ Fluxo → raiz                     ✕ erro
```

As cópias pesadas entram numa fila, uma de cada vez, e o painel guarda as
últimas 6 aulas.
