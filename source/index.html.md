---
title: API Reference

language_tabs: # must be one of https://git.io/vQNgJ
  - shell

toc_footers:
  - <a href='mailto:contato@lab804.com.br'>Obtenha chave de acesso</a>
  - <a href='https://labmet.com.br'>LabMet</a>
  - <a href='https://github.com/lord/slate'>Documentation Powered by Slate</a>

includes:
  - scheme
  - auth
  - errors
  - stations

search: true
---

# Introdução

Cobriremos tudo o que você precisa saber, desde a autenticação até a manipulação dos resultados, até a combinação dos resultados com outros serviços.

As APIs REST fornecem acesso programático para gerar relatórios agrometeorológicos na LabMet. Consulte a Capacidade de água no solo, consulte temperatura, psicometeria, preciptação, radiação e muito mais. A API REST identifica usuários através de uma chave de acesso básica (ApiKey). Todas as respostas estão disponíveis no formato Json.

A API é divida em dois módulos **dados brutos** e **relatórios**, o módulo dados brutos possui dados meteorológicos direto das estações, já os relatórios são dados pré processados e ajustados para cada relatório.
