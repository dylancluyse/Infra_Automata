# Infra_Automata

hello.sh

```
#!/bin/bash
set -o nounset
set -o pipefail

_user="$(id -u -n)"
echo "Hiya $_user !"

_user="$USER"
echo "Hiya $_user !"
```

hey.sh

Eerst moet je de omgevingsvariabele opslaan met ```env person="Dylan"```. Daarna maak je het bash-script aan met daarin de 'nounset'. Daaronder maak je de echo die het omgevingsvariabele oproept.

```
#!/bin/bash
set -o nounset

_user="$(id -u -n)"
```
