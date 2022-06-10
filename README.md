# Домашнее задание Git
1. На локальном репозитории сделать ветки для:
- Postman
- Jmeter
- CheckLists
- Bug Reports
- SQL
- Charles
- Mobile testing

> git branch Postman <br/>
> git branch Jmeter <br/>
> git branch CheckLists <br/>
> git branch Bug Reports <br/>
> git branch SQL <br/>
> git branch Charles <br/>
> git branch Mobile testing

2. Запушить все ветки на внешний репозиторий
> git push --all

3. В ветке Bug Reports сделать текстовый документ со структурой баг репорта
> git checkout Bug_Reports <br/>
> cat >> report.txt <br/>
> Enter

    ID:
    Summary:
    Steps to Reproduce:
    Actual result:
    Expected result:
    Priority:
    Attachments:
    Date:
    Author:

> Enter
> Ctrl+C

4. Запушить структуру баг репорта на внешний репозиторий
> git add . <br/>
> git commit -m 'Create new file' <br/>
> git push -u origin Bug_Reports

5. Вмержить ветку Bug Reports в Main
> git checkout main <br/>
> git merge Bug_reports

6. Запушить main на внешний репозиторий.
> git push

7. В ветке CheckLists набросать структуру чек листа.
> git checkout CheckLists <br/>
> cat >> list.txt <br/>
> Enter

    Номер
    Название проверки
    Результат

> Enter
> Ctrl+C

8. Запушить структуру на внешний репозиторий
> git add . <br/>
> git commit -m 'Create list.txt' <br/>
> git push -u origin CheckLists

9. На внешнем репозитории сделать Pull Request ветки CheckLists в main
> Compare & pull request <br/>
> Create pull request <br/>
> Merge pull request <br/>
> Confirm merge

10. Синхронизировать Внешнюю и Локальную ветки Main
> git checkout main <br/>
> git fetch <br/>
> git pull
