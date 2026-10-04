# Contas do mês

App pessoal de controle financeiro: lance cada receita e despesa do mês, acompanhe quanto sobra ou falta e veja se você está seguindo a regra 50/30/20 (necessidades / desejos / poupança). Tudo roda em um único arquivo HTML, sem servidor, sem login e sem conta.

## Funcionalidades

- **Lançamentos rápidos** — valor, descrição, categoria e data, com despesa ou receita.
- **Contas fixas e parceladas** — marque um lançamento para repetir todo mês ou dividir em parcelas.
- **Navegação entre meses** — veja, edite e exclua lançamentos de qualquer mês, passado ou atual.
- **Regra 50/30/20** — barras de progresso por grupo (Necessidades, Desejos, Poupança) com alertas ao chegar perto ou passar do limite. Percentuais editáveis.
- **Categorias personalizáveis** — crie, renomeie e defina o grupo de cada categoria.
- **Gráficos** — gastos por categoria no mês e comparativo de entradas/saídas dos últimos 6 meses.
- **Backup e restauração** — exporte um backup em JSON ou uma planilha em CSV, e importe o backup depois (por arquivo, texto colado ou área de transferência).

## Como usar

Abra o arquivo `index.html` em qualquer navegador (celular ou computador). Não precisa de instalação, servidor ou internet depois de aberto.

```bash
# clone o repositório e abra o arquivo
git clone <url-do-repositorio>
cd <repositorio>
open index.html   # macOS
# ou: start index.html (Windows) / xdg-open index.html (Linux)
```

Também pode ser hospedado como uma página estática (GitHub Pages, Netlify, Vercel etc.), já que é um único arquivo autocontido.

## Onde os dados ficam

Todos os lançamentos, categorias e configurações ficam salvos **somente no navegador** em que o app foi aberto (IndexedDB, com fallback para localStorage). Não existe conta, login ou envio de dados para qualquer servidor.

Por isso:

- Limpar os dados de navegação do site apaga tudo. Exporte um backup de vez em quando — o app avisa quando fizer mais de 30 dias desde o último.
- Para usar em mais de um dispositivo ou navegador, exporte o backup em um e importe no outro, em Ajustes.

## Tecnologia

HTML, CSS e JavaScript puro, em um único arquivo, sem dependências externas e sem build. O código fica em `index.html`.

## Roteiro (v2)

- Orçamento por categoria individual, além dos grupos do 50/30/20.
- Múltiplas contas e cartões, com saldo por conta.

## Licença

Projeto de uso pessoal. Adapte livremente para as suas necessidades.
