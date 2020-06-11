# How to make a good commit.  
V1.0
---

## ENG

### Commit structure

Message Structure
A commit messages consists of three distinct parts separated by a blank line: the title, an optional body and an optional footer. The layout looks like this:

```
type: subject

body

footer
```

### Details

The title consists of the type of the message and subject.

The Type
The type is contained within the title and can be one of these types:

feat: a new feature  
fix: a bug fix  
docs: changes to documentation  
style: formatting, missing semi colons, etc; no code change  
refactor: refactoring production code  
test: adding tests, refactoring test; no production code change  
chore: updating build tasks, package manager configs, etc; no production code change  
  
The Subject  
Subjects should be no greater than 50 characters, should begin with a capital letter and do not end with a period.
  
Use an imperative tone to describe what a commit does, rather than what it did. For example, use change; not changed or changes.

The Body  
Not all commits are complex enough to warrant a body, therefore it is optional and only used when a commit requires a bit of explanation and context. Use the body to explain the what and why of a commit, not the how.

When writing a body, the blank line between the title and the body is required and you should limit the length of each line to no more than 72 characters.

The Footer  
The footer is optional and is used to reference issue tracker IDs.

### Commit pattern  

feat: Summarize changes in around 50 characters or less  

More detailed explanatory text, if necessary. Wrap it to about 72  
characters or so. In some contexts, the first line is treated as the  
subject of the commit and the rest of the text as the body. The  
blank line separating the summary from the body is critical (unless  
you omit the body entirely); various tools like `log`, `shortlog`  
and `rebase` can get confused if you run the two together.  
  
Explain the problem that this commit is solving. Focus on why you  
are making this change as opposed to how (the code explains that).  
Are there side effects or other unintuitive consequenses of this  
change? Here's the place to explain them.  
  
Further paragraphs come after blank lines.  
  
 - Bullet points are okay, too  
  
 - Typically a hyphen or asterisk is used for the bullet, preceded  
   by a single space, with blank lines in between, but conventions  
   vary here  
  
If you use an issue tracker, put references to them at the bottom,  
like this:

Resolves: #123  
See also: #456, #789  

## RU

### Шаблон коммита

Сообщение-заголовок. Краткое, до 50 символов. Начинать с заглавной буквы

Более подробный поясняющий текст (если нужен). Должен вмещаться в 72 символа. В некоторых ситуациях первая строка сообщения коммита (заголовок) воспринимается как тема email-а, а остальной текст — как «тело». Пустая строка между темой и телом имеет большое значение (за исключением случаев, когда у вас вообще нет тела сообщения). Если заголовок и тело сообщения будут идти подряд, без разделения пустой строкой, это может сбить с толку такие инструменты как rebase.

Глаголы в сообщении коммита следует писать в повелительном наклонении: "Fix bug" («Исправь баг»), а не "Fixed bug" («Исправлен баг») или "Fixes bug" («Исправляет баг»). Когда сообщения коммитов генерируются командами git merge и git revert, они пишутся именно в повелительном наклонении.

Абзацы отделяются друг от друга пустыми строками.

- Допускаются обозначения пунктов списка.

- Обычно для пунктов списка используются знаки дефиса или звездочки с пробелом после них. Каждый пункт отделяется пустой строкой, но это вариативно.

- Допускается обратный абзацный отступ.

Если вы используете issue tracker, добавьте ссылку(и) внизу, вот так:

Resolves: #123 

### Общие положения

1. Указывайте тип коммита:

feat: новая фича, добавляемая к приложению.  
fix: исправление бага.  
style: функции и обновления, имеющие отношение к стилизации.  
refactor: рефакторинг определенного участка кодовой базы.  
test: все, что касается тестирования.  
docs: все, что касается документации.  
chore: обычная поддержка кода, рутина.  
Для обозначения типов коммитов можно также использовать эмодзи.  

2. Отделяйте заголовок от тела сообщения пустой строкой.

3. Сообщение коммита не должно содержать никаких ошибок пробелов.

4. Убирайте знаки пунктуации, в которых нет необходимости.

5. Не ставьте точку в конце заголовка.

6. Заголовок и каждый отдельный абзац должны начинаться с заглавной буквы.

7. В заголовке сообщения используйте повелительное наклонение.

8. Используйте тело сообщения, чтобы описать вносимые изменения и причины этих изменений.

9. Не предполагайте, что ревьюер знает о проблеме, которую вы решаете: оговаривайте ее.

10. Придерживайтесь соглашения о сообщениях коммитов, принятого в вашей команде.

<hr>

### Sources and additional information:
* [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/ "An article about commits in ENG")
* [Git Styleguide](https://udacity.github.io/git-styleguide/ "An article about commits in ENG")
* [Практическое руководство по написанию хороших сообщений коммитов](https://techrocks.ru/2019/12/02/writing-good-commit-messages/ "Статья на русском про коммиты")