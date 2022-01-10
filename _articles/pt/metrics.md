---
lang: pt
title: Métricas do Open Source
description: Tome decisões bem embasadas para ajudar o seu projeto open source a prosperar, medindo e acompanhando seu sucesso.
class: metrics
order: 9
image: /assets/images/cards/metrics.png
related:
  - finding
  - best-practices
---

## Por que medir algo?

Os dados, quando usados com sabedoria, podem ajudá-lo a tomar decisões melhores como um mantenedor open source.

Com mais informações, você pode:

* Entender como usuários respondem a uma nova funcionalidade
* Descubrir de onde os novos usuários vêm
* Identificar e decidir se deve suportar um caso de uso ou uma funcionalidade sugerida.
* Quantificar a popularidade do seu projeto
* Entender como seu projeto é usado
* Arrecadar dinheiro através de patrocínios e doações

Por exemplo, [Homebrew](https://github.com/Homebrew/brew/blob/bbed7246bc5c5b7acb8c1d427d10b43e090dfd39/docs/Analytics.md) descobriu que o Google Analytics os ajuda a priorizar o trabalho:

> Homebrew é fornecido gratuitamente e mantido inteiramente por voluntários em seu tempo livre. Por isso, não temos recursos para fazer estudos detalhados com os usuários do Homebrew para decidir sobre a melhor forma de projetar recursos futuros e priorizar o trabalho atual. Análises agregadas de dados de usuários anônimos nos permitem priorizar correções e recursos com base em como, onde e quando as pessoas usam o Homebrew.

Popularidade não é tudo. As pessoas entram no open source por diferentes razões. Se o seu objetivo como mantenedor open source for mostrar seu trabalho, ser transparente sobre seu código ou apenas se divertir, as métricas podem não ser importantes para você.

Se você _está_ interessado em entender seu projeto em um nível mais profundo, leia as seguintes maneiras de analisar a atividade do seu projeto.

## Descubra

Antes das pessoas poderem contribuir para com seu projeto, elas precisam saber que o projeto existe. Pergunte a si
mesmo: _as pessoas estão encontrando este projeto?_

![Traffic graph](../../assets/images/metrics/repo_traffic_graphs_tooltip.png)

Se seu projeto esta hospedado no
GitHub, [você pode ver](https://help.github.com/articles/about-repository-graphs/#traffic) como as pessoas navegam no
seu projeto e de onde elas vêm. Na página do seu projeto, clique "Insights" e então em "Traffic". Nesta página, você
pode ver:

* **Total de visualizações da página:** Informa quantas vezes seu projeto foi visualizado

* **Total de visitantes únicos:** Informa quantas pessoas visualizaram seu projeto

* **Referência de sites:** Informa de onde vieram os visitantes. Essa métrica pode ajudar você a descobrir como alcançar seu público-alvo e se seus esforços de promoção estão funcionando.

* **Conteudo popular:** Informa a você onde os visitantes vão em seu projeto, a exibição mostra o número de visualizações por página e quantidade de visitantes.

As [GitHub stars](https://help.github.com/articles/about-stars/) também podem ajudar a fornecer uma medida básica de popularidade. Embora as GitHub stars não estejam necessariamente relacionadas a downloads e uso, elas podem dizer quantas pessoas estão percebendo seu trabalho.

Talvez você também queira [rastrear a descoberta apartir de lugares específicos](https://opensource.com/business/16/6/pirate-metrics): por exemplo, Google PageRank, tráfego de referência do site do seu projeto ou referências de outros projetos ou sites open source.

## Uso

As pessoas estão encontrando seu projeto nesta coisa selvagem e louca que chamamos de internet. O ideal é que, quando
elas notarem seu projeto, se sintam compelidos a fazer alguma coisa. A segunda pergunta a se fazer é: _as pessoas estão
utilizando este projeto?_

Se você usa um gerenciador de pacotes, como npm ou RubyGems.org, para distribuir seu projeto, você será capaz de
rastrear os downloads do seu projeto.

Cada gerenciador de pacotes pode usar uma definição ligeiramente diferente de "download". Os downloads não
necessariamente estão relacionados a instalação ou ao uso, mas fornecem uma base para comparação. Tente usar
a [Libraries.io](https://libraries.io/) para rastrear estatísticas de uso em muitos gerenciadores de pacotes populares.

Se o seu projeto está no GitHub, navegue novamento até a página "Traffic". Você pode usar
o [clone graph](https://github.com/blog/1873-clone-graphs) para ver quantas vezes o seu projeto foi clonado em
determinada data, a apresentação mostra o total de clonagem e as clonagens por pessoa.

![Clone graph](../../assets/images/metrics/clone_graph.png)

Se a clonagem é baixa comparada com a quantidade de pessoas que descobrem seu projeto, há duas coisas a se considerar.
São elas:

* Seu projeto não esta obtendo sucesso em converter sua audiência, ou
* Você esta atraindo a audiência errada

Por exemplo, se o seu projeto chegar na primeira página do Hacker News, você provavelmente verá um pico na descoberta (tráfego), mas uma taxa de conversão mais baixa, porque você está alcançando todos no Hacker News. Se o seu projeto Ruby é apresentado em uma conferência Ruby, no entanto, é mais provável que você veja uma alta taxa de conversão de um público-alvo.

Tente descobrir de onde vem seu público e peça a opinião de outras pessoas na página do projeto para descobrir quais desses dois problemas você está enfrentando.

Uma vez que você saiba que as pessoas estão usando o seu projeto, você pode tentar descobrir o que elas estão fazendo com ele. Eles estão construindo nele através e forks ou adicionando novos recursos? Estão usando isso para ciência ou negócios?

## Retenção

As pessoas estão encontrando seu projeto e estão usando. A próxima pergunta a se fazer é: _as pessoas estão contribuindo de volta para este projeto?_

Nunca é cedo demais para pensar nos contribuidores. Sem outras pessoas colaborando, você corre o risco de se colocar em uma situação insustentável onde seu projeto é _popular_ (muitas pessoas o usam), mas não há _suporte_ (não há tempo suficiente para atender a demanda).

A retenção também requer o [ingresso de novos colaboradores](http://blog.abigailcabunoc.com/increasing-developer-engagement-at-mozilla-science-learning-advocacy#contributor-pathways_2), entenda que contribuidores anteriormente ativos acabarão por fazer outras coisas.

Exemplos de métricas da comunidade que você pode acompanhar regularmente incluem:

* **Total de contribuidores e número de commits por contribuidor:** Mostra quantos contribuidores você tem, e quem é mais ou menos ativo. No GitHub, você pode ver isso em "Insights" -> "Contributors." Neste momento, este gráfico conta apenas os contribuidores que se comprometeram com o branch padrão do repositório.

![Contributor graph](../../assets/images/metrics/repo_contributors_specific_graph.png)

* **Primeira vez, casual, e contribuidores recorrentes:** Ajuda você a acompanhar se está recebendo novos contribuidores e se eles retornam. (Contribuidores ocasionais são pessoas com um baixo número de commits. Se é um commit, menos de cinco commits, ou qualquer outra coisa, é com você.) Sem novos contribuidores, a comunidade do seu projeto pode ficar estagnada.

* **Números de issues abertas e pull requests em abertos:** Se esses números ficarem muito altos, talvez você precise de ajuda com a triagem de problemas e as revisões de código.

* **Número de issues _abertas_ e pull requests _abertos_:** Issues abertas, significa que alguém se preocupa o suficiente com o seu projeto para abrir um problema. Se esse número aumenta com o tempo, isso sugere que as pessoas estão interessadas em seu projeto.

* **Tipos de contribuições:** Por exemplo, commits, correções textuais or correções de bugs, ou comentários em uma issue.

> ![](https://avatars.githubusercontent.com/arfon?s=180)
> Open source is more than just code. Successful open source projects include code and documentation contributions together with conversations about these changes.> — @arfon, ["The Shape of Open Source"](https://github.com/blog/2195-the-shape-of-open-source)

## Atividade do mantenedor

Finalmente, você desejará fechar o loop certificando-se de que os mantenedores do seu projeto sejam capazes de lidar com o volume de contribuições recebidas. A última pergunta que você deve se fazer é: _eu estou (ou estamos) respondendo à nossa comunidade?_

Mantenedores não responsivos se tornam um gargalo para projetos open source. Se alguém enviar uma contribuição, mas nunca receber uma resposta de um mantenedor, ela poderá se sentir desencorajada e sair.

[Pesquisa da Mozilla](https://docs.google.com/presentation/d/1hsJLv1ieSqtXBzd5YZusY-mB8e1VJzaeOmh8Q4VeMio/edit#slide=id.g43d857af8_0177) sugere que a capacidade de resposta do mantenedor é um fator crítico para incentivar contribuições recorrentes.

Considere acompanhar quanto tempo leva para você (ou outro mantenedor) responder às contribuições, seja um issue ou um pull request. A resposta não exige ação. Pode ser tão simples como dizer: _"Obrigado pela sua contribuição! E irei revisá-la dentro da próxima semana."_

Você também pode medir o tempo necessário para mover entre as etapas no processo de contribuição, como:

* Tempo médio que um problema permanece em aberto
* Se as questões são fechadas por PRs
* Se as issues obsoletas são fechadas
* Tempo médio para fazer o merge de um pull request

## Use 📊 para aprender sobre pessoas

Entender as métricas ajudará você a construir um projeto open source ativo e crescente. Mesmo que você não acompanhe todas as métricas em um painel, use a estrutura acima para focar sua atenção no tipo de comportamento que ajudará seu projeto a prosperar.
