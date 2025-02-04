# Работа с репозитариями

## Основные сведения о Git и GitHub для создания документации
### Обзор
Как участник проекта по созданию документации вы будете использовать ряд инструментов и процессов. Вы будете работать параллельно с другими участниками над одним и тем же проектом, иногда над тем же содержимым и в то же время. Все это возможно благодаря программному обеспечению Git и GitHub.

Git — это система управления версиями с открытым исходным кодом. Она упрощает совместную работу над проектами такого типа с помощью распределенной системы управления версиями файлов, которые хранятся в репозиториях. По сути, Git позволяет интегрировать в определенный репозиторий потоки работы, выполненные несколькими участниками в течение определенного времени.

GitHub — это служба размещения в Интернете репозиториев Git, которые используются для хранения содержимого docs.microsoft.com. В GitHub размещается основной репозиторий всех проектов. Из этого репозитория участники копируют свою работу.

### Git
Если вы знакомы с централизованными системами управления версиями (например, Team Foundation Server, SharePoint или Visual SourceSafe), вы заметите, что Git использует уникальный рабочий процесс и специальную терминологию для поддержки распределенной модели. Например, в Git не блокируются файлы, как это обычно бывает, когда файл берут на редактирование или возвращают после редактирования. На самом деле Git учитывает изменения на более тонком уровне, сравнивая файлы байт за байтом.

_Git также использует многоуровневую структуру для хранения содержимого проекта и управления им._

* Репозиторий — это единица хранения самого высокого уровня. Репозиторий содержит одну или несколько ветвей.
* Ветвь — это единица хранения с текущими файлами и папками, которые формируют содержимое проекта. Ветви используются для разделения потоков работы (обычно они называются версиями). Участники всегда вносят изменения в содержимое в определенной ветви, и эти изменения привязаны к соответствующей ветви. Все репозитории содержат ветвь по умолчанию (обычно она называется главной, "main") и одну или несколько ветвей, предназначенных для объединения с ветвью по умолчанию. Ветвь по умолчанию является текущей версией и "единственным истинно верным источником" для определенного проекта. Из этой родительской ветви создаются все остальные ветви в репозитории.
_Участники взаимодействуют с Git, чтобы обновлять репозитории и управлять ими локально и на уровне GitHub._

* Для локального взаимодействия участники используют такие инструменты, как консоль Git Bash, которая поддерживает команды Git для управления локальными репозиториями и обмена данными с репозиториями GitHub.
* Кроме того, участники используют сайт www.github.com с интегрированной системой Git для управления согласованием изменений, возвращаемых обратно в основной репозиторий.
### GitHub
*_Примечание_*
Хотя управление проекта Docs основано на использовании GitHub, некоторые команды используют Visual Studio Team Services для размещения репозиториев Git. Клиент Visual Studio Team Explorer — это графический интерфейс для взаимодействия с репозиториями Team Services. Этот интерфейс является альтернативой использованию команд Git в командной строке.
Кроме того, многие приведенные ниже руководства разработаны в качестве рекомендаций, которые появились в результате многолетнего размещения содержимого служб Azure в GitHub. Они могут понадобиться для работы с некоторыми репозиториями Docs.
Все рабочие процессы начинаются и заканчиваются на уровне GitHub, где хранится основной репозиторий любого проекта Docs. Копии, создаваемые участниками для собственного использования, распространяются на нескольких компьютерах. В итоге они согласовываются в основном репозитории GitHub проекта.

# Рабочий процесс по внесению значительных или времязатратных изменений на сайте GitHub

==Важно!==

При работе со всеми репозиториями, используемыми для публикации на сайте docs.microsoft.com, необходимо соблюдать правила поведения для управляемых компанией Майкрософт сообществ разработки ПО с открытым кодом и правила поведения от .NET Foundation. Дополнительные сведения см. на странице с часто задаваемыми вопросами о правилах поведения. С любыми вопросами и комментариями можно также обратиться по адресу opencode@microsoft.com или conduct@dotnetfoundation.org.

Порядок внесения незначительных изменений или уточнений в документацию и примеры кода из общедоступных репозиториев см. в условиях использования на сайте docs.microsoft.com. Если новые или значительные изменения вносят не сотрудники корпорации Майкрософт, в комментариях к запросу на вытягивание на сайте GitHub появится предложение принять условия лицензионного соглашения с участником (CLA). Вам нужно заполнить онлайн-форму перед обработкой запроса на вытягивание.

