# Los Angeles Restaurant Market Analysis

Estudo bilingue sobre o mercado de restaurantes em Los Angeles e a possibilidade de testar uma cafetaria com serviço robotizado. Inclui notebooks Jupyter, resumos em HTML/PDF, dataset de origem e um site estático bilingue.

## Estrutura

- `English/` — notebook e resumo para investidores em inglês.
- `Português de Portugal/` — notebook e resumo em português de Portugal.
- `data/rest_data_us.csv` — conjunto de dados usado nos notebooks.
- `site/` — site estático pronto para publicação no Render; a pasta contém os relatórios, PDFs, notebooks e dataset para descarregar.
- `render.yaml` — definição do site estático no Render.
- `Los_Angeles_Restaurant_Market.code-workspace` — espaço de trabalho para abrir o projecto no VS Code.

## Abrir no VS Code

Abra `Los_Angeles_Restaurant_Market.code-workspace` ou a pasta do projecto. Para trabalhar nos notebooks, instale as extensões Python e Jupyter no VS Code e seleccione um ambiente Python com `pandas`, `numpy`, `matplotlib`, `seaborn` e `plotly`. O caminho do CSV pode ser actualizado na primeira célula de carregamento, caso necessário.

## GitHub

A pasta local está preparada para versionamento. Depois de criar um repositório vazio no GitHub, use o terminal integrado do VS Code:

```powershell
git status
git add .
git commit -m "Add bilingual LA restaurant market analysis"
git remote add origin <URL-do-repositorio-GitHub>
git push -u origin main
```

Não inclua palavras-passe, tokens nem credenciais no repositório.

## Render — site estático

O `render.yaml` publica apenas `site/`; os notebooks e os ficheiros de análise ficam no repositório e os downloads necessários ao site ficam dentro da pasta publicada.

1. Envie primeiro o repositório para o GitHub.
2. No Render, escolha **New → Blueprint** e ligue o repositório; o Render lê `render.yaml`.
3. Se criar o serviço manualmente como **Static Site**, escolha o mesmo repositório, deixe o comando de build vazio e indique `site` como **Publish Directory**.
4. Após o primeiro deploy, verifique a página inicial, as duas versões, os PDFs e os downloads.

A publicação ainda não foi feita: é necessário ligar este repositório à conta GitHub e ao serviço Render da utilizadora. Consulte a [documentação de Static Sites do Render](https://render.com/docs/static-sites) e a [referência de Blueprints](https://render.com/docs/blueprint-spec).
