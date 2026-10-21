# Meu Dinheiro no Tempo — Mercado do Tempo

Aplicativo web **funcional**, sem cadastro, baseado no projeto científico *Mercado do Tempo: Estudo dos Impactos da Inflação, da Desigualdade Social e da Educação Financeira na Vida das Famílias Brasileiras*.

## Abrir no VS Code

1. Descompacte o ZIP e abra a pasta `Meu_Dinheiro_no_Tempo_VSCode` no Visual Studio Code.
2. Abra `index.html` no navegador, **ou**, se preferir, instale a extensão **Live Server** e use **Open with Live Server**.
3. Não há bibliotecas, contas, APIs nem instalações necessárias. Funciona inclusive sem internet (os links de fontes externas requerem conexão).

## Telas que funcionam

- **Início:** atalhos e acompanhamento das missões.
- **Simulador de inflação:** taxa anual *hipotética*, cálculo composto, poder de compra e gráfico. Permite salvar.
- **Poder de compra:** preços da cesta editáveis, produtos novos, comparação hoje/futuro, quantidades alcançáveis.
- **Meu orçamento:** renda e oito categorias de despesas editáveis, saldo e proporções, salvamento no histórico.
- **Mercado do Tempo:** três famílias fictícias com rendas e despesas diferentes, eventos econômicos e escolhas. Mostra quem sente mais o efeito relativo.
- **Desafios e quiz:** seis perguntas interativas com explicações e cinco missões desbloqueáveis.
- **Histórico:** registros salvos no navegador, exclusão de itens, CSV e backup/importação em JSON.
- **Aprenda mais:** conceitos fundamentais e links de pesquisa em fontes oficiais.

## Onde ficam os dados?

Todos os registros são armazenados em `localStorage` do navegador atual. **Não há servidor, banco compartilhado ou sincronização entre dispositivos.** Por isso, para transferir dados, utilize **Meu histórico → Salvar backup** e depois **Importar backup** no outro computador.

Em computadores compartilhados, qualquer pessoa que utilize o mesmo perfil do navegador poderá ver ou apagar os dados. Use valores fictícios na feira. No modo anônimo os dados podem desaparecer ao fechar a sessão.

## Hipóteses científicas / limites

- **As taxas de inflação, os preços e os perfis econômicos fornecidos são fictícios**, para ensino. Não representam dados reais atualizados, projeções oficiais nem recomendações financeiras.
- Fórmula da evolução composta: `preço futuro = preço atual × (1 + taxa/100) ** anos`.
- Estimativa do poder de compra: `valor nominal / (1 + taxa/100) ** anos`.
- A cesta considera a **mesma inflação anual hipotética para todos os produtos** para simplificar a comparação; na economia real, os preços variam individualmente.
- As diferenças entre três famílias são ilustrativas e não reproduzem estratos socioeconômicos reais.
- Educação financeira é útil, mas não resolve, sozinha, a desigualdade de renda.

## Estrutura da pasta

```
Meu_Dinheiro_no_Tempo_VSCode/
  index.html  — telas e formulários
  styles.css  — identidade visual e adaptação para celular
  app.js      — todas as interações, cálculos e salvamento
  README.md   — este guia
  TESTES.md   — roteiro de verificação
  assets/     — reservado para imagens futuras
```

## Próximas melhorias possíveis

Versão online com banco de dados seguro, gráficos de IPCA obtidos de fontes oficiais com atribuição da data de consulta, novos desafios baseados em dados reais e pesquisa de usabilidade com estudantes e famílias. Essas melhorias **não fazem parte** desta entrega.
