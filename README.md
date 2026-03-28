*setsid*: faz um processo filho aleatório virar processo principal de um conjunto de processos
```
#include<unistd.h>
if (setsid() < 0)
{
  perror("Error in setsid.\n")
  exit(EXIT_FAILURE);
}
else
{
  // código novo aqui;
}
```

---

*chdir*: mudar destinatário/caminho do seu arquivo/programa
```
#include<unistd.h>
if (chdir(CAMINHO_AQUI))
{
  // código novo aqui;
}
else { perror("Error in chdir.\n"); exit(EXIT_FAILURE); }
```

---

*mkfifo*: serve para criar um pipe nomeado no seu programa/processo
```
#include<sys/stat.h:
int mk = mkfifo(CAMINHO_AQUI, PERMISSÕES_AQUI);
if (mk < 0) { perror("Error in mk.\n"); exit(EXIT_FAILURE); }
```

---

+ 2 count beecrowd
