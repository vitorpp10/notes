*sprintf*: para escrever um buffer, array/string na memória.
```
#include<stdio>
char* memory
sprintf(memory, "message");

ou

char buffer[100];
int number = 1;
double height = "6.7";
const char* name = "Vitor";
sprintf(buffer, "%s is %d years old and %.1f feet tall");
```

---

*mmap*: mapeia uma área da memória, escolhe o tipo da pasta, privada/púbica, compartilha/única, tamanho em bytes, offset + fd(arquivo).
*munmap*: para limpar/liberar a área mapeada depois de usada/executada.
```
#include<sys/mman.h>
char* memory = (char*)mmap(NULL, tamanho_bytes, prots, flags, fd, offset);

ou

char* mp = mmap(NULL, tamanho_bytes, prots, flags, fd, offset);
if (mp == MAP_FAILED) { perror("Error in mmap.\n); exit(EXIT_FAILURE); }
munmap(bufffer, tamanho_bytes);
```


+ 1 count beecrowd
