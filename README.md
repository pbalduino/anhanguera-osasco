 **Ideia original**

 - Plínio Balduino: pensei em fazer assim.
 - Plínio Balduino: começo contando muito rapidamente a historia do JS
 - Plínio Balduino: e na sequencia a definição do JS: que é uma linguagem prototipada, orientada a objetos e funcional
 - Igor Hercowitz de França: :)
 - Plínio Balduino: mostro o que é uma linguagem prototipada
 - Plínio Balduino: e um exemplo em self, que é um dialeto de smalltalk
 - Plínio Balduino: mostro um exemplo de orientação a objetos, que a galera está mais do que careca de saber o que é
 - Plínio Balduino: e que um objeto em JS é um mero bag de campos
 - Plínio Balduino: e mostro um exemplo usando prototipos e OO
 - Plínio Balduino: e mostro um exemplo de código funcional em JS
 - Plínio Balduino: com um equivalente em Scheme
 - Igor Hercowitz de França: :D
 - Plínio Balduino: e junto o funcional àquele objeto usado nos exemplos anteriores
 - Igor Hercowitz de França: maneiro :D
 - Igor Hercowitz de França: quero ver essa apresentacao depois :D
 - Plínio Balduino: explico high order functions em JavaScript e como isso é importante para quem usa jQuery
 - Igor Hercowitz de França: boua
 - Plínio Balduino: depois de alguns exemplos, mostro como *tudo* no jQuery usa programação funcional
 - Plínio Balduino: eventos, composites e o cacete
 - Plínio Balduino: será que em meia hora dá ou fica pouco?
 - Igor Hercowitz de França: acho que voce poderia fazer um comparativo do mesmo codigo usando prototype, OO e funcional (just for fun)
 - Plínio Balduino: e como seria isso?
 - Igor Hercowitz de França: sei la
 - Igor Hercowitz de França: fica a ideia ai :)
 - Plínio Balduino: me ajude a pensar nessa parte
 - Plínio Balduino: seria baca
 - Plínio Balduino: bacana
 - Igor Hercowitz de França: estou justamente pensando
 - Igor Hercowitz de França: oque seria bacana tb:
 - Igor Hercowitz de França: nao sei se daria para demonstrar c um codigo bobo
 - Igor Hercowitz de França: mas mostrar a performance entre dos 3 tipos de codigo

### Outro diálogo

- Plínio: foda né?
ó
2 retorna o que?
- Reinaldo: 4
- Plínio: nao
vc tem essa linha de código:
2
essa linha te retorna que valor?
esquece o código lá de cima
todo o seu código agora é isso:
2
retorna 2, certo?
Sent at 3:27 PM on Friday
- Reinaldo: yep
- Plínio: e a linha abaixo:
(2)
retorna quanto?
- Reinaldo: 2
- Plínio: ou seja
(x) retorna o valor de x, ok?
- Reinaldo: ok
- Plínio: isso em lisp ou em js
tanto faz
se vc escrever
(2 + 2)
retorna 4, certo?
beleza
proximo passo
2 é um valor, ok?
nada demais nisso
- Reinaldo: ok
- Plínio: var x = 2;
x retorna 2
x é um valor
tambem nada demais nisso
ok?
- Reinaldo: ok
- Plínio: agora sua cabeça vai doer
- Reinaldo: chalenge acept
- Plínio: function x( ){return 4};
beleza?
se eu executar
x()
retorna quanto?
- Reinaldo: x
- Plínio: ``function x( ){return 4};
x`` retorna quanto? ou o que zzz...
Sent at 3:33 PM on Friday
- Reinaldo: x retorna 4?
- Plínio:
(16:07:47) 
- Plínio Balduino: isso
facil, nao?
- Reinaldo: então, era o que imaginava
- Plínio: e se eu escrever somente
x;
retorna o que?
- Reinaldo: setar o valor de entrada da função internamente nessa função
retorna x
- Plínio: retorna uma função
um objeto do tipo 'function'
Reinaldo: pq ele ta setado ali
Plínio: se vc digitar isso no console, vai aparecer

x;
=> function
x();
=> 4
Sent at 3:41 PM on Friday
-Reinaldo: entendi
x é o nome da função que seta internamente 4 como X
Sent at 3:45 PM on Friday
-Plínio: na verdade
x é a variável que contem uma função
function x(){return 4};

é um atalho para

var x = function(){return 4};
entendeu?
> function é um valor como qualquer outro
como se fosse um numero, um array, um boolean
var y = 3;
- Reinaldo: dentro da var tem uma function?
pqp
pqp
Plínio: hehehe
- Reinaldo: essa foi foda
pqp
- Plínio: lembra do começo da conversa
onde (4) == 4 ?
- Reinaldo: sim
- Plínio: se vc
> (16:07:47) Plínio Balduino: fizer
> var x = function(a){return a * 2};
> sabendo que (blah) retorna blah
> entao
> (x) retorna uma function, certo?
- Reinaldo: sim
- Plínio: então ``(x)(2);``
- retorna 4
- certo?
- Reinaldo: ºoº... vc atribui 2 a função dentro de x
- Plínio: exatamente... vamos de novo ``function x(a){return a * 2};``, ``x(2)`` é 4, certo?
- Reinaldo: ok
- Plínio: function x(a){return a * 2};
é o mesmo que
var x = function(a){return a * 2};
certo?
- Reinaldo: a segunda faz mais sentido mas deve ser sim
- Plínio: beleza
são a mesma coisa
então, de acordo com a segunda forma, se fizermos
x(2) é 4, certo?
Reinaldo: sim
- Plínio: x(2) == 4 do primeiro jeito
x(2) == 4 do segundo jeito
- Reinaldo: nossa
funcção dentro de var e foda
- Plínio: então
se (x) == x
então
> (x)(2) == 4
> certo?
> (x)(2) == x(2)
- Reinaldo: ok
sim
- Plínio: se (x)(2) == 4
e x contem uma função
- Reinaldo: =
diferente
- Plínio: pq nao fazer assim:
> (function(a){return a * 2})(2)
≥ (16:07:47) Plínio Balduino: == 4 ?
Reinaldo: (x)(2) == 4?
Plínio: isso
- Reinaldo: em vez de setar essa função a x
você cria ela ja comparando sem o x
- Plínio: exatamente
crio uma função anonima
função anonima é a que não é atribuida a variavel nenhum
ela nao ganha um nome
Sent at 4:06 PM on Friday
- Plínio: entendeu?
- Reinaldo: sim
- Plínio: louco, nao?
- Reinaldo: eu como um leigo estou me perguntando... o pessoal que programa js no dia a dia, sabe disso?
- Plínio: nao
- Reinaldo: então vc acabou de fazer alguns slides pra amanhã... parabens
- Plínio: hehehe
- Reinaldo: mt foda

**Esqueleto da apresentação**
