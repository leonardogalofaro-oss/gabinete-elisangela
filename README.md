# Sistema de Gabinete

Aplicativo web para gestão de gabinete parlamentar municipal — demandas, cidadãos,
agenda, ofícios, metas, comunicação e mais.

- **100% no navegador**, sem servidor. Funciona offline (PWA, "adicionar à tela inicial").
- **Dados criptografados** (AES-256) e guardados no próprio aparelho. Nada sai do dispositivo.
- **Sincronização opcional** entre aparelhos via repositório privado próprio (os dados
  trafegam sempre criptografados — "cofre cego").

## Tecnologia

HTML + JavaScript puro (sem etapa de build), Tailwind, Chart.js, Leaflet, CryptoJS.
Todas as bibliotecas são locais (pasta `vendor/`), então o app funciona sem internet.

## Como rodar localmente

Por ser estático, basta servir a pasta:

```
python3 -m http.server 8080
```

E abrir `http://localhost:8080/index.html`.
