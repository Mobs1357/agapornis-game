# Agapornis Life — protótipo jogável

Protótipo inicial em orientação horizontal, com cenário 3D low-poly feito em Three.js.

## Executar
- Requer Node.js 18+ para os testes.
- Na pasta do projeto: `npm test`
- Para jogar localmente: `npm start` e abrir `http://localhost:8080`.
- O navegador precisa de internet para carregar Three.js pelo CDN.

## Controles
- Arraste a cena para girar a câmera.
- Toque em uma ave para selecioná-la.
- Alimente, faça voar ou transfira a ave.
- Construa novos viveiros por 100 moedas.
- Avance o dia para atualizar idade e necessidades básicas.

## Escopo atual
Inclui núcleo de estado, viveiros, aves, objetos, limites, transferência, salvamento e um visualizador 3D inicial. Ainda não inclui reprodução funcional, genética integrada, filhotes, mercado, persistência automática ao reabrir, nem validação visual em aparelhos Android reais. A animação de voo é demonstrativa e ainda precisa de refinamento.
