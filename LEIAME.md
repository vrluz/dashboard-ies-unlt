# Dashboard IES — UNLT

Arquivos deste repositório: `index.html` (o painel) e a pasta `fonts/` (tipografia Aptos). Não há servidor, build nem workflow.

## Antes de publicar: colocar as chaves do Back4App
Abra `index.html` e, no bloco `1) CONFIGURAÇÃO`, troque os dois `COLE_AQUI`:

    const B4A = {
      appId: "COLE_AQUI",      // Application ID
      jsKey: "COLE_AQUI",      // JavaScript Key
      serverURL: "https://parseapi.back4app.com"
    };

(Back4App > App Settings > Security & Keys.) Use somente Application ID e JavaScript Key. Nunca coloque Master Key, REST Key ou Client Key neste arquivo.

## Publicar no GitHub Pages
Settings > Pages > Source: "Deploy from a branch" > Branch: `main` / `(root)` > Save.

## Segurança
- Os dados ficam no Back4App, protegidos por login e pelas permissões das classes `Analista` e `Medicao` (sem acesso público).
- Este arquivo contém os nomes da equipe e as regras do IES: prefira repositório privado.

Mais detalhes de uso (lançamento, benchmark, níveis) no `LEIAME` do pacote `dashboard-ies-back4app`.
