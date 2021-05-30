# github-alias
- alterar configurações git
  - <code>git config --global core.editor code </code>
  - <code>git config --global --edit</code>
  - <code>
    [user] 
      name = Douglas Poma
      email = email@mail.com
    [core]
      editor = code --wait
    [push]
      followTags = true #envia tags anotadas (-a) automáticamente no push
    [alias]
      s = !git status -s
      c = !git add --all && git commit -am
      l = !git log --pretty-format:'%C(yellow)%h%C(red)%d %C(white)%s - %C(cyan)%cn, %C(green)%cr'
      amend = !git add --all && git commit ---amend --no-edit #emenda alterações com último comando
      count = !git shortlog -s --grep #estatisticas (git count test)
    </code>
