### Манифест разработки Дискурса

1. Дискурс — открытый проект. Каждый желающий имеет право стать контрибьютором проекта, внести изменения в любой из сервисов проекта и отправить Pull Request.
1. Дискурс — общий проект. Вы всегда можете пообщаться с другими членами команды в [Gitter чате Дискурса](https://gitter.im/Discours/community). Там Вы можете узнать, что сейчас лучше сделать, а также задать любой вопрос по поводу разработки проекта. 
1. Дискурс — проект для читателя. В первую очередь команда выполняет те таски, за которые проголосовали пользователи на [публичной доске задач проекта]().
1. Дискурс — проект для любого разработчика. Мы принимаем микросервисы для backend на любом языке программирования. Но стоит понимать, что мэйнтейнеры проекта не могут знать всех языков, поэтому Dockerfile для запуска микросервиса, понятная документация и тесты (с настроенным CI для их прогона) обязательны в каждом микросервисе.
1. Дискурс — проект для приятной разработки. Команда следит за качеством кода в проекте для того, чтобы новым контрибьюторам было максимально просто влиться в проект. Качество кода - это не только code style и тесты, но и такие субъективные показатели, как читаемость кода и архитектура. Мэйнтейнеры проекта имеют право попросить автора PR изменить код в целях повышения его качества.
1. Дискурс — проект для удобной разработки новых features. Команда Дискурса стремится создать проект, в котором не надо читать весь код для реализации конкретной функциональности. Мы стремимся создать максимально изолированную среду разработки, используя которую каждая фича разрабатывается отдельно. На frontend проектах мы используем [storybook](https://storybook.js.org/) для разработки компонентов и [react-testing-library](https://testing-library.com/docs/react-testing-library/intro) для интеграционного тестирования функциональности компонентов. На backend проектах — разрабатываем используя тесты.
1. Дискурс — проект с открытым манифестом разработки. Каждый желающий может прислать изменения в данный манифест.
1. Дискурс — проект доступный. Верстка в проекте должна учитывать пользователей с ограниченными возможностями, то есть необходимо использовать [ARIA аттрибуты](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA).
1. Дискурс — проект без гос. цензуры. Но большая часть наших читателей из РФ, где РосКомНадзор частенько бомбит славный город Воронеж и даже иногда [блокирует сам себя](https://lenta.ru/news/2016/12/12/127001/). Инфраструктура проекта должна быть распределенной, но должна поддерживать быструю смену IP адресов всего, до чего необходимо достучаться пользователю (фронтэнд, бэкэнд, rss микросервис, другие микросервисы доступные пользователю). Нельзя создавать vendor lock на решения, которые не позволяют быстро сменить IP (Cloudflare, Netlify).