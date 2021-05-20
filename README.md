# Interpretei e buguei

No teste, está descrito e eu não sei se era pra fazer 2 apis, ou 1 com os 2 serviços.
Na confusão, vai as duas.
- 2 APIs diferentes:
[1a API](https://github.com/mtscarneiro/wineTest1/),
[2a API](https://github.com/mtscarneiro/wineTest2/)

- 1 API com os 2 serviços:



### Criação da Primeira API

Está criado a primeira parte do teste, onde já está setado dados das lojas físicas mockados assim como no exemplo dado: 

```java
        Store s1 = new Store(null, "LOJA_PINHEIROS", new ArrayList<>());
        Store s2 = new Store(null, "LOJA_JARDINS", new ArrayList<>());
        Store s3 = new Store(null, "LOJA_MOEMA", new ArrayList<>());
```

e 

```java
        Zip z1 = new Zip(null, 100000, 200000, s1);
        Zip z2 = new Zip(null, 200001, 300000, s1);
        Zip z3 = new Zip(null, 300001, 400000, s2);
        Zip z4 = new Zip(null, 400001, 500000, s2);
        Zip z5 = new Zip(null, 500001, 600000, s3);
        Zip z6 = new Zip(null, 700001, 800000, s3);  
```

Com a possibilidade de inserção de novas Lojas e também de novos CEPs, (caso a loja já existente aumente o seu range de entregas, e ou novas lojas que tenham
novos ranges de entrega).

### Obs:

Para realizar testes e conseguir criar a [Segunda parte do teste](https://github.com/mtscarneiro/wineTest2/), eu fiz um Maven build nesse projeto aqui, e criei um
FatJar para que eu rodasse o server em cmd, e alterei a port da segunda api pra que eu rodasse as duas APIs sem precisar hostea-las.


- [x] Criada a primeira API
- [x] Criada a segunda API
- [x] Uso de dados mockados
- [ ] Consegui o emprego? :shipit: 
