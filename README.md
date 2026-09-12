# Predictfy — apresentação ao vivo para a Locaweb

Abra `Predictfy_Apresentacao_Locaweb.html` no navegador. Fontes, logos e ícones estão no arquivo; não exige instalação ou servidor. Internet é necessária para abrir o MVP.

Use as setas ou espaço para navegar, F para tela cheia e T para trocar o tema. Home / End levam ao primeiro / último slide. O rodapé contém apenas controles visuais, sem notas.

A apresentação tem 10 slides. O agente está no slide 9, com seu conteúdo preservado. O encerramento está no slide 10 e abre Gestão em outra aba; também há links de Monitoramento, Técnico e Fila operacional. Autentique previamente o MVP no mesmo navegador.

No agente, o botão revela uma síntese editorial de uma resposta real validada. Este HTML não chama o LLM nem simula uma resposta ao vivo; a demonstração real ocorre no MVP.

## Movimentos

- Slide 2: contorno da caixa prioritária varia suavemente em até 2 px.
- Slide 3: ícones flutuam e giram discretamente, com maior amplitude.
- Slide 4: movimento anterior preservado.
- Slide 5: movimento do ícone ampliado.
- Slide 6: linha conecta as etapas de previsão, prioridade e consulta.
- Slide 7: linha fina percorre o espaço atrás das caixas.
- Slide 8: clareamento suave alternado entre as caixas.
- Slide 9: animações do agente preservadas.
- Slide 10: botão de acesso recebe movimento e destaque suaves.

As transições permanecem próximas de 1 segundo. A preferência de movimento reduzido desativa as animações.

## Slide 6

“Da previsão à ação” apresenta funcionalidades verificadas: previsões D+1/D+7, separação de Total/P2/P3 e consultas no dashboard e no agente. Não usa comparação de MAE.

## Escopo

Este repositório contém somente a apresentação ao vivo. Não faz parte do pacote de entrega acadêmica. PPTX, PDFs, dados brutos e código do MVP não estão incluídos.

## Editar e regenerar

Requer Node.js 20 ou superior.

```sh
npm ci
npm run build
npx playwright install chromium
npm test
```

Edite `fontes/gerar_html.cjs`. O build atualiza o HTML na raiz. O teste verifica navegação, conteúdo responsivo e controles em três tamanhos de tela, produzindo capturas em `revisao/`. Fontes, logos e ícones usados estão em `assets/` ou nas dependências fixadas no lockfile.

Para apresentar, basta abrir o HTML; nenhuma dependência ou servidor é necessário.
