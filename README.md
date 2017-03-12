# ideology
Для отображения адекватного "git diff", "git log -p", "git show" с odt форматом следует сперва установить odt2txt, затем добавить в конец файла ~/.gitconfig:

[diff "odf"]
      textconv=odt2txt

Затем для каждого нового проекта внести изменение в файл .gitattributes или $GIT_DIR/info/attributes, следующие:


*.ods diff=odf
*.odt diff=odf
*.odp diff=odf

В данном проекте последний шаг уже сделан.
