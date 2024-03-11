1. **git rebase**:
    - Эта команда используется для перебазирования (rebase) текущей ветки на другую ветку или на определенный коммит.
    - Пример использования:
      ```bash
      git checkout feature_branch
      git rebase main_branch
      ```

2. **git stash**:
    - Позволяет временно сохранить текущие изменения в стэше (stash), чтобы потом можно было их применить в другом месте.
    - Пример использования:
      ```bash
      git stash
      git checkout another_branch
      git stash apply
      ```

3. **git bisect**:
    - Используется для бинарного поиска по истории коммитов для нахождения того коммита, в котором возникла проблема.
    - Пример использования:
      ```bash
      git bisect start
      git bisect bad
      git bisect good <commit>
      ```

4. **git cherry-pick**:
    - Позволяет выбрать определенный коммит из одной ветки и применить его к другой ветке.
    - Пример использования:
      ```bash
      git checkout another_branch
      git cherry-pick <commit>
      ```

5. **git reflog**:
    - Показывает историю изменений HEAD, что может быть полезно для восстановления случайно удаленных коммитов или переключения между состояниями репозитория.
    - Пример использования:
      ```bash
      git reflog
      git reset --hard HEAD@{1}
      ```

6. **git submodule**:
    - Позволяет включать один репозиторий в другой как подмодуль.
    - Пример использования:
      ```bash
      git submodule add <repository_url>
      git submodule update --init
      ```