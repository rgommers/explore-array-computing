Using clipboard copy with highlighting on Linux:

alias pbcopy='xclip -selection clipboard -t text/html'
alias pbpaste='xclip -selection clipboard -o'

pygmentize -l bash -f html -O noclasses=true pydata_ams.md | pbcopy -t text/html

or, from https://gist.github.com/avdi/9038972:

function clipsyn {
  local syntax_type="$1"

  pbpaste | pygmentize -l $syntax_type -f rtf | pbcopy
}
