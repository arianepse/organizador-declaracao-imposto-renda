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







