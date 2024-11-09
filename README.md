# Contador de Horas de Live

Este projeto cria um contador de horas para exibir o tempo de duração de uma live em uma página HTML. A cada segundo, o contador é atualizado para mostrar o tempo total em horas com a frase "Já foram X horas de live".

## Funcionalidade

A página HTML utiliza JavaScript para incrementar o contador de segundos e exibi-lo em horas (com uma casa decimal) de forma dinâmica. Esse contador pode ser usado diretamente no OBS como uma fonte de navegador, permitindo exibir o tempo de live atualizado em tempo real.

## Onde alterar o valor inicial

Se você quiser que o contador comece com um valor pré-definido em vez de zero, basta editar a variável `segundos` no arquivo HTML.

Por exemplo, se quiser que o contador comece em 1 hora, ajuste o valor inicial para `3600` segundos:

```javascript
const HORAS_INICIAIS = 129 // Começa em 1 hora (3600 segundos)
```
### Como Adicionar o Contador ao OBS

Para exibir o contador no OBS Studio, siga estas etapas:

1. Abra o OBS e selecione a cena onde deseja adicionar o contador.
2. Na seção **Fontes**, clique no botão **+** e selecione **Fonte de Navegador**.
3. Dê um nome à nova fonte (por exemplo, "Contador de Horas de Live") e clique em **OK**.
4. No campo **URL**, insira o link onde o arquivo HTML está hospedado ().
5. Defina a largura e altura da fonte de navegador de acordo com a resolução desejada para o contador (por exemplo, **500x100**).
6. Para garantir que o contador nunca reinicie quando a cena se tornar ativa, granta que a opção **Recarregar quando a cena se tornar ativa** esteja *DESMARCADA*.
7. Clique em **OK** para adicionar a fonte ao OBS e posicione o contador na tela conforme desejado.

Após esses passos, o contador aparecerá em sua live e atualizará o tempo automaticamente a cada segundo, indicando quantas horas já se passaram desde o início. Essa configuração permite que o contador funcione em tempo real sem a necessidade de atualizações manuais.
