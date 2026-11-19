# Agapornis Life — protótipo 0.1

Protótipo de jogo de manejo e criação de **Agapornis roseicollis**, com interface horizontal e viveiro 3D low-poly.

## O que já funciona
- Viveiro 3D com câmera giratória por arraste e seleção de aves por toque/clique.
- Três aves iniciais, painel de fome, sede, felicidade e saúde.
- Alimentar, fornecer água e fazer carinho.
- Formar casal com validação básica de sexo, idade e exclusividade.
- Construir ninho, iniciar postura, avançar incubação e gerar filhotes após 23 dias de jogo.
- Loja simples, moedas, compra de suprimentos e expansão de viveiros.
- Avanço de dias, envelhecimento, XP e nível.
- Salvamento automático no armazenamento local do navegador.

## Executar
O jogo usa módulos ES e Three.js por CDN. É necessário internet na primeira abertura e servir os arquivos por HTTP (não abrir `index.html` diretamente como `file://`).

Com Node.js instalado:

```bash
npm test
npm run serve
```

Depois abra `http://localhost:8080` no navegador. Também pode publicar a pasta em um host estático, como GitHub Pages, depois de enviar todos os arquivos e pastas mantendo a estrutura.

## Limitações conhecidas desta versão
- A genética ainda não foi implementada: os filhotes recebem uma aparência provisória. Não use esta versão para prever cruzamentos reais.
- Fertilidade e sexo dos filhotes são aleatórios e simplificados para prototipagem.
- A reprodução ainda não possui comportamento autônomo completo, vínculo genético validado, pedigree detalhado, doenças, mercado de aves ou animações de voo/caminhada completas.
- A idade mínima de reprodução é uma regra provisória de jogo, não uma recomendação veterinária.
- O modelo 3D é procedural e simples; a câmera funciona por arraste horizontal.

## Estrutura
- `index.html`: interface e ponto de entrada.
- `style.css`: layout horizontal responsivo.
- `src/main.js`: cena Three.js e ligação da interface.
- `src/game-core.js`: regras e estado do jogo.
- `tests/game-core.test.js`: testes automatizados das regras principais.
