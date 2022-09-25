<br/>

<p align="left"> 

<img src="img/anhanguera.jpg" width="100px"/> 

</p>

<p align="center"> 

*Palestra na Anhanguera Educacional em 22/05/2013*

</p>

<br/>

# Esqueleto da apresentação 

<details close>

<summary> Ideia original </summary>

<br>

**Plínio Balduino:** pensei em fazer assim.

**Plínio Balduino:** começo contando muito rapidamente a história do JS

**Plínio Balduino:** e na sequência a definição do JS: que é uma linguagem prototipada, orientada a objetos e funcional

**Igor Hercowitz de França:** :)

**Plínio Balduino:** mostro o que é uma linguagem prototipada

**Plínio Balduino:** e um exemplo em self, que é um dialeto de smalltalk

**Plínio Balduino:** mostro um exemplo de orientação a objetos, que a galera está mais do que careca de saber o que é

**Plínio Balduino:** e que um objeto em JS é um mero bag de campos

**Plínio Balduino:** e mostro um exemplo usando prototipos e OO

**Plínio Balduino:** e mostro um exemplo de código funcional em JS

**Plínio Balduino:** com um equivalente em Scheme

**Igor Hercowitz de França:** :)

**Plínio Balduino:** e junto o funcional àquele objeto usado nos exemplos anteriores

**Igor Hercowitz de França:** maneiro :D

**Igor Hercowitz de França:** quero ver essa apresentação depois :D

**Plínio Balduino:** explico high order functions em JavaScript e como isso é importante para quem usa jQuery

**Igor Hercowitz de França:** boua

**Plínio Balduino:** depois de alguns exemplos, mostro como *tudo* no jQuery usa programação funcional

**Plínio Balduino:** eventos, composites e o cacete

**Plínio Balduino:** será que em meia hora dá ou fica pouco?

**Igor Hercowitz de França:** acho que voce poderia fazer um comparativo do mesmo código usando prototype, OO e funcional (just for fun)

**Plínio Balduino:** e como seria isso?

**Igor Hercowitz de França** sei la

**Igor Hercowitz de França:** fica a ideia ai :)

**Plínio Balduino:** me ajude a pensar nessa parte

**Plínio Balduino:** seria baca

**Plínio Balduino:** bacana

**Igor Hercowitz de França:** estou justamente pensando

**Igor Hercowitz de França:** o que seria bacana tb:

**Igor Hercowitz de França:** não sei se daria para demonstrar c um código bobo

**Igor Hercowitz de França:** mas mostrar a performance entre dos 3 tipos de código

<br>

</details>

<details close>
<summary> Outro diálogo  </summary>

<br>

**Plínio Balduino:** foda né? ó 2 retorna o que?

**Reinaldo:** 4

**Plínio Balduino:** não

**Plínio Balduino:** vc tem essa linha de código:

**Plínio Balduino:** 2

**Plínio Balduino:** essa linha te retorna que valor?

**Plínio Balduino:** esquece o código lá de cima

**Plínio Balduino:** todo o seu código agora é isso:

**Plínio Balduino:** 2

**Plínio Balduino:** retorna 2, certo?

**Reinaldo:** yep

**Plínio Balduino:** e a linha abaixo: ```(2)``` retorna quanto?

**Reinaldo:** 2

**Plínio Balduino:** ou seja ```(x)``` retorna o valor de x, ok?

**Reinaldo:** ok

**Plínio Balduino:** isso em lisp ou em js tanto faz se vc escrever ```(2 + 2)```

**Plínio Balduino:** retorna 4, certo?

**Plínio Balduino:** beleza

**Plínio Balduino:** próximo passo

**Plínio Balduino:** 2 é um valor, ok?

**Plínio Balduino:** nada demais nisso  

**Reinaldo:** ok

**Plínio:** ``var x = 2;``

**Plínio Balduino:** x retorna 2

**Plínio Balduino:** x é um valor

**Plínio Balduino:** também nada demais nisso

**Plínio Balduino:** ok?

**Reinaldo:** ok

**Plínio:** agora sua cabeça vai doer

**Reinaldo:** chalenge acept

**Plínio:** ```function x( ){return 4};```

**Plínio Balduino** beleza?

**Plínio Balduino** se eu executar

**Plínio Balduino** ```x()```

**Plínio Balduino** retorna quanto?

**Reinaldo:** ```x```

**Plínio:** ```function x( ){return 4};```

**Plínio Balduino:** ```x``` retorna quanto? ou o que ```zzz...```

**Reinaldo:** ```x retorna 4?```

**Plínio Balduino:** isso

**Plínio Balduino** fácil, não?

**Reinaldo:** então, era o que imaginava

**Plínio:** e se eu escrever somente

**Plínio Balduino** ```x;```

**Plínio Balduino** retorna o que?

**Reinaldo:** setar o valor de entrada da função internamente nessa função

**Plínio Balduino** retorna ```x```

**Plínio:** retorna uma função

**Plínio Balduino** um objeto do tipo 'function'

**Reinaldo:** pq ele ta setado ali

**Plínio:** se vc digitar isso no console, vai aparecer 

```javascript
x; => function
x();
=> 4
```

**Reinaldo:** entendi

**Reinaldo:** ```x``` é o nome da função que seta internamente 4 como ```X```

**Plínio:** na verdade

**Plínio:** x é a variável que contém uma função

**Plínio:** ```function x(){return 4};```

**Plínio:** é um atalho para ```var x = function(){return 4};``` 

**Plínio:** entendeu?

**Plínio:** ```function``` é um valor como qualquer outro como se fosse um número, um array, um boolean

**Plínio:** ```var y = 3;```

**Reinaldo:** dentro da ```var``` tem uma ```function``` ?

**Reinaldo:** pqp

**Reinaldo:** pqp

**Plínio:** hehehe

**Reinaldo:** essa foi foda

**Reinaldo:** pqp

**Plínio:** lembra do começo da conversa onde ```(4) == 4``` ?

**Reinaldo:** sim

**Plínio Balduino:** se vc

**Plínio Balduino:** fizer ```var x = function(a){return a * 2};```

**Plínio Balduino:** sabendo que (blah) retorna blah

**Plínio Balduino:** entao ```(x)``` retorna uma ```function```, certo?

**Reinaldo:** sim

**Plínio Balduino:** então ``(x)(2);``

**Plínio Balduino:** retorna 4 

**Plínio Balduino:** certo?

**Reinaldo:** ºoº... vc atribui 2 a função dentro de ```x```

**Plínio Balduino** exatamente... vamos de novo ```function x(a){return a * 2};```, ```x(2)``` é 4, certo?

**Reinaldo:** ok

**Plínio Balduino** ```function x(a){return a * 2};``` é o mesmo que ```var x = function(a){return a * 2};```

**Plínio Balduino** certo?   

**Reinaldo:** a segunda faz mais sentido mas deve ser sim

**Plínio Balduino** beleza

**Plínio Balduino** são a mesma coisa

**Plínio Balduino** então, de acordo com a segunda forma, se fizermos

**Plínio Balduino** ```x(2)``` é 4, certo?

**Reinaldo:** sim

**Plínio:** ```x(2) == 4``` do primeiro jeito

**Plínio Balduino** ```x(2) == 4``` do segundo jeito

**Reinaldo:** nossa funcção dentro de ```var``` e foda

**Plínio:** então se ```(x) == x``` então ```(x)(2) == 4```

**Plínio Balduino:** certo?

**Plínio Balduino** ```(x)(2) == x(2)```

**Reinaldo:** ok

**Reinaldo:** sim

**Plínio:** se ```(x)(2) == 4``` e ```x``` contém uma função

**Reinaldo:** `=`

**Reinaldo:** diferente

**Plínio:** pq não fazer assim: ```(function(a){return a * 2})(2)```

**Plínio:** ```≥``` 

**Plínio Balduino:** ```== 4``` ?

**Reinaldo:** ```(x)(2) == 4``` ?

**Plínio:** isso

**Reinaldo:** em vez de setar essa função a ```x``` você cria ela ja comparando sem o ```x```

**Plínio:** exatamente

**Plínio Balduino:** crio uma função anônima

**Plínio Balduino:** função anônima é a que não é atribuída a variável nenhuma

**Plínio Balduino:** ela não ganha um nome

**Plínio:** entendeu?

**Reinaldo:** sim

**Plínio:** louco, não?

**Reinaldo:** eu como um leigo estou me perguntando... o pessoal que programa js no dia a dia, sabe disso?

**Plínio:** não

**Reinaldo:** então vc acabou de fazer alguns slides pra amanhã... parabéns

**Plínio:** hehehe

**Reinaldo:** mt foda

<br/>

</details>
