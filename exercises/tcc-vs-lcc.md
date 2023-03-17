# TCC *vs* LCC

Explain under which circumstances *Tight Class Cohesion* (TCC) and *Loose Class Cohesion* (LCC) metrics produce the same value for a given Java class. Build an example of such as class and include the code below or find one example in an open-source project from Github and include the link to the class below. Could LCC be lower than TCC for any given class? Explain.

## Answer

Les métriques Tight Class Cohesion (TCC) et Loose Class Cohesion (LCC)  sont deux mesures de la qualité du design orienté objet d'une classe  Java. TCC mesure la proportion de paires de méthodes dans une classe qui partagent au moins un paramètre en commun, tandis que LCC mesure la  proportion de paires de méthodes dans une classe qui n'ont pas de  paramètres en commun.

```java
public class MyClass {
    public void methodA(int x, String s) {
        // implementation
    }
    
    public void methodB(String s, int x) {
        // implementation
    }
    
    public void methodC(int x, double d) {
        // implementation
    }
}
```

Dans cette exemple, chaque paire de méthodes a exactement un paramètre en commun, ce qui signifie que TCC et LCC sont tous deux égaux à 1.

Il est possible que LCC soit inférieur à TCC pour une classe donnée.  Cela se produit lorsqu'une classe a beaucoup de méthodes qui partagent  des paramètres en commun, mais qui ont également des paramètres qui ne  sont pas partagés par d'autres méthodes de la même classe. Dans ce cas,  TCC sera élevé car il y aura de nombreuses paires de méthodes partageant des paramètres en commun, mais LCC sera plus bas car il y aura  également de nombreuses paires de méthodes n'ayant aucun paramètre en  commun.