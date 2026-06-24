MESI Protocol: Protocolo da CPU para garantir a coerência de dados das cores e informações que elas lidam no sistema, como cada Core possui dentro de si um L1 e L2 cache, as vezes uma Core pode mudar um valor de forma privada, fazendo com que outras Cores do sistema não vejam essa mudança, então ele fica em um nivel abaixo de `Store Buffer`, `Out-Of-Order`, `Invalide-Queue`, controlando oque cada Core vai receber, cada letra em seu nome significa uma marcação que cada Core vai receber dependendo do que ela fizer:

- `M(Modified)`: Seria quando uma Core modifica um dado recebido dentro da sua L1/L2 cache privada e o MESI dela avisa para as cores que estao com a mesma variavel que ocorreu mudanças, no caso ele descobre quais cores estão com a mesma variavel por causa do L3 cache

- `E(Exclusive)`: Seria quando o dado está apenas em uma Core porem o valor dele está igual RAM

- `S(Shared)`: Quando o 2 ou mais Cores possuem o mesmo dado e está igual na RAM, podendo ler de forma segura

- `I(Invalid)`: Quando o dado está desatualizado em um Core ou não é possivel ler ele, causando Cache Miss
