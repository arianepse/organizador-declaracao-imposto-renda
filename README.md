# Organizador de Declaração de Imposto de Renda em Excel

## 📌 Introdução
Este projeto consiste na criação de um organizador de IR em Excel, estruturado com menu interativo e telas específicas para organização das informações do titular, informes e notas.

## 📂 Estrutura do Projeto
- Aba 1: Titular (dados do contribuinte)
- Aba 2: Informes (rendimentos bancários)
- Aba 3: Notas (fontes de renda ou extratos)

## 🐱‍👤 Habilidades utilizadas
- Criação de Menu
- Itens de navegação
- Formatações personalizadas
- Função soma
- Uniformidade visual
- Ajustes finais de usabilidade

## 🛠 Construção Passo a Passo

### Etapa 1 - Criação do Menu

Abra um arquivo Excel em branco.

Selecione a coluna A e expanda o tamanho dela. Página Inicial -> Fonte -> Cor de preenchimento (balde) -> Mais cores -> Personalizar. *Foi utilizada RGB 14;19;23*.

Pesquise no Google: lion purple icon. Copie a imagem e cole na planilha. Com botão direito do mouse -> Tamanho e Propriedades -> Propriedades -> Marque *Não mover ou dimensionar com células*.

Para adicionar um nome a ferramenta vá em Menu Inserir -> Ilustrações -> Formas -> retângulo. Escreva "LION APP", aumenta a fonte para tamanho 20, em negrito e Arial Black. Diminui o tamanho da caixa, move para a coluna A, sem preenchimento e sem contorno. Seleciona o texto, botão direito, Formatar Efeitos de Texto -> Opções de Texto -> Preenchimento de Texto -> Gradiente. Escolha, pelo menos, 2 cores. Opções de Forma -> *Não mover ou dimensionar com células*.

Selecione o ícone e a forma, irá aparecer Ferramentas de Imagem -> Formatar -> Organizar -> Alinhar -> Centralizar.

**Para criar o botões:** Menu Inserir -> Ilustrações -> Formas -> Retângulo Arredondado. Escreva "TITULAR", fonte Segoe Ui Light, tamanho 18, negrito, centralizado e alinhado ao meio, cor gradiente. Arraste o ponto amarelo que vai arredondar mais a forma. Posicione na coluna A. Copie e cole para "INFORMES e "NOTAS". CTRL para selecionar os três botões, Formatar -> Organizar -> Alinhar -> Centralizar e Distribuir vertical. Sempre verifique o elemento *Não mover ou dimensionar com células*.

**Para adicionar criador:** Menu Inserir -> Ilustrações -> Formas -> Retângulo. Escreva "SYSTEM BY ARI 💜", fonte Segoe Ui Light, tamanho 10. Sem preenchimento e sem contorno. Centraliza. Não mover ou dimensionar com células.

Podemos um detalhe como uma linha, para isso: Menu Inserir -> Ilustrações -> Formas -> Linha. Pressiona SHIFT e arrasta para deixar ela reta. Cor roxa e espessura de 3/4. Centraliza. Não mover ou dimensionar com células.

Renomeie *Planilha1* para "TITULAR". CTRL e arrasta para o lado que duplica, faça isso para "INFORMES" e "NOTAS".

Nos botões da planilha TITULAR deixe sem preenchimento os botões INFORMES e NOTAS. Faça o procedimento análogo nas planilhas Informes e Notas.

**Inserindo Links:** na aba TITULAR, seleciona o botão TITULAR e com botão direito do mouse, Hiperlink -> Colocar neste documento -> célula de referência C1, selecione TITULAR e OK. Faça isso para os outros botões da mesma aba e das demais também. 

Agora temos um Menu navegável!

![Menu](/images/menu.jpg)

### Etapa 2 - Construção da Tela do Titular

Na coluna C vamos colocar todos os campos que pedem para declarar: NOME, CPF, NASCIMENTO, TÍTULO DE ELEITOR, CÔNJUGE, RUA, RUA ABREVIADA, CEP, TELEFONE, CELULAR, E-MAIL, HOUVE ALTERAÇÕES DA ENTREGA ANTERIOR, DEPENDENTE CÔNJUGE, RESIDENTE DO EXTERIOR. 

Começando da C7 fonte Segoe Ui Light, na col D estilos de célula -> neutra. Seleciona colunas C e D e duplo clique para autofit. Bordas horizontais cinza claro. Col C alinhada à direita.

Seleciona C3:E3, Estilos de célula -> Título I. Mais bordas, tom de rosa. Escreva "1. DADOS DO TITULAR" e tom roxo escuro.

Seleciona C4:E4, tom rosa mais claro, aumentar altura, itálico, mesclar, alinhar à esquerda, recuo 3x. Escreva "Preencha os dados da pessoa física abaixo".

Seleciona a tabela e mova uma linha para cima.

Seleciona as três últimas células (D17:D19), Menu Dados -> Validação de Dados -> Permitir -> Lista: SIM;NÃO.

Agora vamos inserir um botão para ir à próxima página: Menu Inserir -> Formas -> Retângulo. Escreva "PRÓXIMO ->", formate como queira, botão direito Não mover ou dimensionar com células. Botão direito, hiperlink, neste documento, C1 e Informes.

### Etapa 2.1 - Formatações personalizadas

Nos campos com CPF, CEP, Telefone e Celular, observa-se que possuem um padrão característico, porém nem sempre formatações específicas essas estão disponíveis. O Excel nos permite personalizar esse tipo de formatação.

Clica na célula do referente ao CPF -> Página Inicial -> Número -> Mais formatos de número -> Personalizado

> Para entradas numéricas é representado por 0 (zero) e entradas de texto são colocadas entre aspas duplas ("").

Em tipo, para o CPF vamos inserir: 000"."000"."000"-"00 e OK.

Quando digitar somente os números do CPF ele já aparecerá no padrão formatado.

De maneira análoga, faça o mesmo para os demais campos necessitam de personalização.

![Formato de CPF](/images/cpf-personalizado.jpg)

E agora temos a aba Titular pronta.

![Tela Titular](/images/titular.jpg)

### Etapa 3 - Tela de Informes

Repare que na primeira aba começamos na célula C3, na segunda aba também manteremos essa célula.

Copia o cabeçalho e deixa a largura das colunas C e D iguais da plan Titular, idem para altura das linhas. Renomeie para "2. INFORMES DE RENDIMENTOS BANCÁRIOS". E na linha debaixo para "Preencha com seus dados atuais de cada banco".

Copia a primeira linha da tabela para pegarmos a formatação. Preencha com BANCO, VALOR ATUAL e ANEXO, em cada linha. Valor formata como moeda e em bancos vamos criar uma listagem de todos os bancos na aba TABELAS para selecioná-los .

Menu Dados -> Validação de Dados -> Lista: seleciona a lista dos bancos. Opcionalmente, pode-se adicionar uma mensagem de entrada que aparece quando passa o mouse por cima da célula, como também criar um alerta de erro.

Você pode, na linha de cima, deixar como "1º Banco" em tamanho menor e fonte cinza clara.

Copia a tabela e saltando uma linha crie mais bancos.

Agora vamos criar um totalizador dos bancos. Adicione algumas linhas acima e escreva "TOTAL" célula debaixo =SOMA e selecione o Valor Atual de cada banco. Formate.

E para finalizar esta tela copiamos o botão de *Próximo* da aba anterior, duplicamos e colocaremos "<- ANTERIOR" que volta ao TITULAR e "PRÓXIMO ->" que vai para notas.

Oculte a aba dos bancos com botão direito do mouse.

![Tela de Informes](/images/informes.jpg)

### Etapa 4 - Tela de Notas

Vamos copiar o estilo, largura da coluna e iniciar na célula C3 como nas abas anteriores. Cabeçalho desta: "3. NOTAS BANCÁRIAS OU EXTRATO DE HOLERITES" e "São todos os valores de entrada mês a mês de receita"

Preenchimento rosa da C7:E7, "ENTRADAS", fonte Segoe Ui Light e cor branca, mesclar e centralizar.

Na linha debaixo, digite DATA, CATEGORIA, VALOR. Redimensione a largura das colunas de forma equilibrada. Formate. Menu Inserir -> Inserir Tabela. No pontinho azul no final da tabela arraste para mais linhas.

Na primeira linha abaixo de Categoria, selecione, Menu Dados -> Validação de Dados -> Lista: HOLERITE; CNPJ; FREELANCE. Copie e cola nas demais linhas da tabela. Centraliza tudo, fonte Segoe Ui.

Copia botão da aba anterior, deixe levemente menor e em cima. Crie o link para Informes.

![Tela de Notas](/images/notas.jpg)

### Etapa 5 - Toques Finais

1. onde tem as abas, clique nos três pontinhos e arraste à esquerda;
2. no Menu Exibir, desmarcar Linhas de grade, Barra de fórmulas, e Títulos;
3. pode deixar em modo tela cheia (caso queira);
4. na aba Titular, parte amarela onde pode mexer, seleciona e com botão direito Formatar célula -> Proteção -> desmarcar a opção *bloqueada*. Botão direito em cima da aba e Proteger planilha -> marca Selecionar células desbloqueadas. Dessa forma, pode digitar apenas onde está liberado o preenchimento dos dados e nos hiperlinks.
5. Faça o passo anterior para as demais abas.

![Tela Final](/images/toquesfinais.jpg)
