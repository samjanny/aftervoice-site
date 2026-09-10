---
layout: page
title: Política de privacidade do Aftervoice
---

Última atualização: 10 de setembro de 2026.

O Aftervoice é um instrumento para sessões de escuta. Esta política diz o que acontece com os
dados que o aplicativo produz. O que ele gera fica no telefone, exceto um relato que você
decida enviar expressamente.

## Em resumo

O Aftervoice não tem contas, publicidade nem estatísticas de uso. Gravações, faixa do microfone,
diário, notas, marcadores e dados dos sensores não são enviados aos nossos servidores. A rede é
usada para os bancos de vozes gerenciados pelo Google Play e, somente a seu pedido, para um
relato de texto.

## O que fica no telefone

- **As configurações**: idioma da interface, idioma da voz, temporizador, busca automática,
  filtro de ruído.
- **O diário das sessões**: data, tempo de escuta, a sintonia usada, o título e as notas que
  você escreve, e os marcadores com o nome que você dá a eles.
- **As gravações**, ao tocar em Gravar. Escuta do ambiente salva apenas o microfone,
  incluindo as vozes próximas, sem emitir áudio. Sintonia salva o áudio do aplicativo e,
  com permissão, o microfone. Ele pode captar também o alto-falante: as faixas não são
  acusticamente isoladas.

São arquivos privados do aplicativo, no armazenamento dele. Nenhum outro aplicativo do telefone
pode lê-los. O aplicativo fica fora tanto do backup na nuvem quanto da transferência para um
telefone novo: se você trocar de aparelho, o diário não vai junto.

## O que fica no telefone

Gravações, microfone, diário, configurações, notas, marcadores e dados dos sensores ficam no
telefone. Não há análise, coleta de falhas, publicidade nem SDKs de rastreamento. O aplicativo
só entra em contato com a Altrove Labs quando você toca em **Enviar relato**.

Os relatórios de falha que o autor recebe vêm do Google Play, agregados e anônimos, e descrevem
como o aplicativo se comportou, nunca o que suas sessões continham.

## Relatos e suporte

Ao tocar em **Relatar** em uma gravação, você escreve o motivo dentro do Aftervoice. Só ao tocar
em **Enviar relato**, o aplicativo envia à Altrove Labs por HTTPS o texto, a versão, o idioma da
interface e identificadores aleatórios da sessão e da gravação. Não envia áudio, faixa do
microfone, notas, marcadores, identificador do aparelho nem endereço de e-mail.

O servidor necessariamente vê o endereço IP da conexão. Ele só o usa na memória para limitar
abusos a cinco relatos por hora, não o registra e o esquece em até uma hora ou ao reiniciar. O
relato é encaminhado por e-mail a `support@altrovelabs.net` e mantido apenas pelo tempo necessário
para avaliá-lo. O provedor do serviço de e-mail só o processa para entregá-lo à Altrove Labs. O
aplicativo mostra uma referência aleatória que você pode usar para pedir a exclusão. Os dados não
são usados para outros fins.

## A permissão de microfone

O Aftervoice pede uma única permissão, **o microfone**, e a usa em dois lugares:

- **Durante uma gravação**, para salvar o ambiente sozinho ou junto da faixa sintética em
  Sintonia. O microfone abre ao tocar em Gravar e fecha ao terminar, inclusive quando o
  aplicativo vai para segundo plano.
- **No sonar**, onde o som captado é filtrado acima de 17 kHz dentro do aplicativo antes de
  qualquer processamento, não é gravado e não é guardado. O microfone fica aberto só enquanto
  aquela tela está aberta.

Se você recusar a permissão, Escuta do ambiente não grava e explica como permitir o acesso.
Não ativa a síntese como alternativa. Sintonia pode gravar só o áudio do aplicativo e indica
isso explicitamente. O sonar precisa de acesso ao microfone.

## Quanto tempo os dados ficam e como apagá-los

Ficam até você apagá-los. Você pode excluir uma gravação específica ou uma sessão inteira pelo
arquivo, com confirmação. Desinstalar o aplicativo apaga tudo: configurações, diário e gravações.

## Menores

O Aftervoice não é dirigido a menores de 13 anos e não coleta deliberadamente dados deles.

## O áudio que o aplicativo gera

Os sons que o Aftervoice faz são gerados por um modelo de voz que roda no telefone. Não são
gravações de pessoas reais e não são prova de coisa alguma.

O áudio produzido pelo aplicativo leva uma marca legível por máquina que o declara sintético,
como exige o artigo 50 do regulamento europeu de inteligência artificial. A marca está no som em
si, não em uma etiqueta do arquivo: sobrevive ao compartilhamento, à recompressão e a um corte, e
continua lá em um arquivo renomeado ou reexportado. Qualquer pessoa pode verificá-la, sem nos
pedir nada, com o detector descrito em [Verificar a marca](../detector.html).

A marca não contém nada sobre você: não há identificador do telefone, nem da sessão, nem da
instalação. Ela diz uma coisa só, sempre a mesma: este áudio foi feito por uma máquina. A trilha
de microfone de uma gravação não é marcada, porque não é áudio gerado — é o cômodo em que você
estava.

## Contato

Para dúvidas sobre esta política: [support@altrovelabs.net](mailto:support@altrovelabs.net).

Responsável pelo tratamento: **Altrove Labs**. Os dados do diário e as gravações permanecem em
seu poder e sob seu controle, no seu telefone. Tratamos apenas os relatos e comunicações que
você decide enviar; você pode exercer seus direitos previstos no GDPR escrevendo para o endereço
acima e informando, para um relato anônimo, a referência.

## Alterações

Se esta política mudar, a data no topo muda com ela, e a versão anterior fica no histórico
público do repositório do site.
