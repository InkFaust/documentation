---
sidebar_position: 1
---

# Обзор

Методология призвана **упростить и стандартизировать декомпозицию логики для больших и долгоживужих проектов.**

Для этого она вводит ряд [концепций][refs-concepts] и [абстракций][refs-splitting], на которых *может базироваться* архитектура от проекта к проекту - отсюда получаем *ряд преимуществ*

:::info

[Модуль][refs-module] - структурная единица проекта (файл / директория)

:::

### Явная бизнес-логика

Модули распределяются согласно [скоупу влияния, бизнес-ответственности и техническому назначению][refs-splitting]

Благодаря этому *архитектура стандартизируется и становится более простой для ознакомления*

### Адаптация к новым условиям

Каждый компонент архитектуры имеет свое назначение и не влияет на другие

Благодаря этому *под новые требования можно независимо модифицировать функциональность приложения без непредвиденных последствий*

### Техдолг и рефакторинг

Каждый модуль является независимым и самодостаточным

Благодаря этому *можно переписать его с нуля без неожиданных сайд-эффектов*

### Масштабирование проекта и команды

Увеличение функциональности ведет к значительно меньшему усложнению проекта, т.к. вся логика распределена детерминированно и изолированно

Благодаря этому *легко добавлять и онбордить новых людей в команду, а также расширять функциональность проекта*

### Контролируемое переиспользование логики

Каждый модуль имеет свои ограничения и рекоммендации на переиспользуемость согласно [своему слою][refs-splitting--layers]

Благодаря этому *сохраняется баланс между соблюдением принципа `DRY` и возможности кастомизировать логику модуля без оверхедных переопределений*

## См. также

- [Причины создания методологии][refs-motivation]
- [(Гайд) Как привести модули к низкой связности][refs-low-coupling]
- [Примеры применения методологии][refs-examples]
- [(Гайд) Миграция с feature-slices (v1)][refs-migration-v1]
  - *Содержит также сравнение двух версий и причины создания v2*

[refs-motivation]: /docs/get-started/motivation

[refs-splitting]: /docs/concepts/app-splitting
[refs-splitting--layers]: /docs/concepts/app-splitting#group-layers
<!-- FIXME: Ссылаться на рут позднее, а не на первый элемент -->
[refs-concepts]: /docs/concepts/architecture

[refs-module]: /docs/reference/glossary#module

[refs-low-coupling]: /docs/guides/low-coupling
[refs-migration-v1]: /docs/guides/migration-from-v1
<!-- FIXME: Ссылаться на рут позднее, а не на первый элемент -->
[refs-examples]: /docs/guides/examples/viewer
