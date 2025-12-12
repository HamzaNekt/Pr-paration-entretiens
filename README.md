# Guide d'Entretien Technique - Questions et Réponses

Ce document contient une collection structurée de questions fréquemment posées lors d'entretiens techniques, accompagnées de réponses détaillées et d'exemples de code. Il couvre Java, Spring Boot, JavaScript, Angular, React, C#, ASP.NET, HTML, CSS, TypeScript, Docker, DevOps, Git et GitHub.

## 📋 Table des matières

### Java
- [Questions fondamentales sur Java](#questions-fondamentales-sur-java)
- [Questions sur les modificateurs et mots-clés](#questions-sur-les-modificateurs-et-mots-clés)
- [Questions sur la gestion des exceptions](#questions-sur-la-gestion-des-exceptions)
- [Questions sur les Collections et structures de données](#questions-sur-les-collections-et-structures-de-données)
- [Questions sur Java 8+ (nouvelles fonctionnalités)](#questions-sur-java-8-nouvelles-fonctionnalités)
- [Questions comportementales et situationnelles](#questions-comportementales-et-situationnelles)

### Spring Boot
- [Questions fondamentales sur Spring Boot](#questions-fondamentales-sur-spring-boot)
- [Questions sur la configuration](#questions-sur-la-configuration)
- [Questions sur les serveurs embarqués](#questions-sur-les-serveurs-embarqués)
- [Questions sur les REST APIs](#questions-sur-les-rest-apis)
- [Questions sur Spring Data JPA](#questions-sur-spring-data-jpa)
- [Questions sur l'injection de dépendances](#questions-sur-linjection-de-dépendances)
- [Questions sur Spring Boot Actuator](#questions-sur-spring-boot-actuator)
- [Questions sur la sécurité](#questions-sur-la-sécurité)
- [Questions sur les tests](#questions-sur-les-tests-spring-boot)
- [Questions sur les exceptions](#questions-sur-les-exceptions-spring-boot)
- [Questions sur les filtres](#questions-sur-les-filtres)
- [Questions avancées Spring Boot](#questions-avancées-spring-boot)
- [Spring Framework Core - IoC et Injection de Dépendances](#spring-framework-core---ioc-et-injection-de-dépendances)
- [Spring Data JPA et Hibernate](#spring-data-jpa-et-hibernate)
- [Spring MVC](#spring-mvc)
- [Spring Security](#spring-security)
- [Spring AOP (Aspect-Oriented Programming)](#spring-aop-aspect-oriented-programming)
- [Gestion des Transactions](#gestion-des-transactions)
- [Validation](#validation)
- [Gestion des Exceptions](#gestion-des-exceptions)
- [Tests dans Spring Boot](#tests-dans-spring-boot)
- [Configuration et Profils](#configuration-et-profils)
- [REST API et Documentation](#rest-api-et-documentation)
- [Microservices avec Spring Cloud](#microservices-avec-spring-cloud)
- [Sécurité et JWT](#sécurité-et-jwt)
- [Caching](#caching)
- [Messaging avec RabbitMQ/Kafka](#messaging-avec-rabbitmqkafka)
- [Logging](#logging)
- [Schedulé et Tâches Asynchrones](#schedulé-et-tâches-asynchrones)
- [Conseils pour l'Entretien Spring Boot](#conseils-pour-lentretien-spring-boot)

### JavaScript
- [Questions de Base](#questions-de-base-javascript)
- [Questions Intermédiaires](#questions-intermédiaires-javascript)
- [Questions Avancées](#questions-avancées-javascript)

### Angular
- [Questions Fondamentales](#questions-fondamentales-angular)
- [Services et Injection de Dépendances](#services-et-injection-de-dépendances-angular)
- [Cycle de Vie des Composants](#cycle-de-vie-des-composants-angular)
- [RxJS et Observables](#rxjs-et-observables-angular)
- [Routing](#routing-angular)
- [Formulaires](#formulaires-angular)
- [HTTP et Communication](#http-et-communication-angular)
- [Communication entre Composants](#communication-entre-composants-angular)
- [Détection de Changements](#détection-de-changements-angular)
- [Pipes](#pipes-angular)
- [Questions Avancées Angular](#questions-avancées-angular)

### React
- [Questions Fondamentales](#questions-fondamentales-react)
- [Props et State](#props-et-state-react)
- [React Hooks](#react-hooks)
- [Cycle de Vie des Composants](#cycle-de-vie-des-composants-react)
- [Gestion d'État Avancée](#gestion-détat-avancée-react)
- [React Router](#react-router)
- [Performance et Optimisation](#performance-et-optimisation-react)
- [Liste et Clés](#liste-et-clés-react)
- [React et TypeScript](#react-et-typescript)
- [Questions Avancées React](#questions-avancées-react)

### C#
- [Questions Fondamentales](#questions-fondamentales-csharp)
- [Types et Variables](#types-et-variables-csharp)
- [Programmation Orientée Objet](#programmation-orientée-objet-csharp)
- [LINQ et Collections](#linq-et-collections-csharp)
- [Programmation Asynchrone](#programmation-asynchrone-csharp)
- [Gestion des Exceptions](#gestion-des-exceptions-csharp)
- [Questions Avancées C#](#questions-avancées-csharp)

### ASP.NET
- [Questions Fondamentales ASP.NET](#questions-fondamentales-aspnet)
- [ASP.NET Core MVC](#aspnet-core-mvc)
- [Web API](#web-api-aspnet)
- [Entity Framework Core](#entity-framework-core)
- [Middleware et Pipeline](#middleware-et-pipeline)
- [Sécurité et Authentification](#sécurité-et-authentification-aspnet)
- [Déploiement](#déploiement-aspnet)

### HTML
- [Questions Fondamentales HTML](#questions-fondamentales-html)
- [Sémantique HTML5](#sémantique-html5)
- [Formulaires](#formulaires-html)
- [Accessibilité](#accessibilité-html)
- [SEO et Méta-données](#seo-et-méta-données)

### CSS
- [Questions Fondamentales CSS](#questions-fondamentales-css)
- [Sélecteurs et Spécificité](#sélecteurs-et-spécificité)
- [Box Model et Layout](#box-model-et-layout)
- [Flexbox](#flexbox)
- [CSS Grid](#css-grid)
- [Responsive Design](#responsive-design)
- [Animations et Transitions](#animations-et-transitions)
- [Préprocesseurs CSS](#préprocesseurs-css)

### TypeScript
- [Questions Fondamentales TypeScript](#questions-fondamentales-typescript)
- [Types et Interfaces](#types-et-interfaces-typescript)
- [Generics](#generics-typescript)
- [Types Avancés](#types-avancés-typescript)
- [Décorateurs](#décorateurs-typescript)
- [TypeScript avec React](#typescript-avec-react)

### Docker
- [Questions Fondamentales Docker](#questions-fondamentales-docker)
- [Images et Conteneurs](#images-et-conteneurs)
- [Dockerfile](#dockerfile)
- [Docker Compose](#docker-compose)
- [Réseaux et Volumes](#réseaux-et-volumes-docker)
- [Optimisation](#optimisation-docker)

### DevOps
- [Concepts Fondamentaux](#concepts-fondamentaux-devops)
- [CI/CD](#cicd)
- [Infrastructure as Code](#infrastructure-as-code)
- [Monitoring et Logging](#monitoring-et-logging)
- [Cloud Platforms](#cloud-platforms)

### Git
- [Questions Fondamentales Git](#questions-fondamentales-git)
- [Branches et Merge](#branches-et-merge)
- [Rebase et Cherry-pick](#rebase-et-cherry-pick)
- [Résolution de Conflits](#résolution-de-conflits)
- [Bonnes Pratiques](#bonnes-pratiques-git)

### GitHub
- [Questions Fondamentales GitHub](#questions-fondamentales-github)
- [Pull Requests](#pull-requests)
- [GitHub Actions](#github-actions)
- [GitHub Workflows](#github-workflows)
- [Collaboration](#collaboration-github)

---

## Questions fondamentales sur Java

### 1. Qu'est-ce que Java et quelles sont ses principales caractéristiques ?

Java est un langage de programmation orienté objet, développé par Sun Microsystems (maintenant Oracle). Ses principales caractéristiques sont :

- **Indépendance de la plateforme** : "Write Once, Run Anywhere" grâce à la JVM
- **Orienté objet** : tout est organisé en classes et objets
- **Robuste** : gestion automatique de la mémoire avec le garbage collector
- **Sécurisé** : pas de pointeurs explicites, bytecode vérifié
- **Multithread** : support natif de la programmation concurrente
- **Performance** : compilation JIT pour optimiser l'exécution

---

### 2. Quelle est la différence entre JVM, JRE et JDK ?

- **JVM (Java Virtual Machine)** : machine virtuelle qui exécute le bytecode Java et assure l'indépendance de la plateforme
- **JRE (Java Runtime Environment)** : environnement d'exécution qui contient la JVM + bibliothèques standard nécessaires pour exécuter des applications Java
- **JDK (Java Development Kit)** : kit de développement complet qui contient le JRE + outils de développement (compilateur javac, debugger, etc.)

---

### 3. Expliquez les principes de la Programmation Orientée Objet (POO)

Les 4 piliers de la POO :

1. **Encapsulation** : regrouper les données et méthodes dans une classe, cacher les détails d'implémentation avec les modificateurs d'accès
2. **Héritage** : permet à une classe d'hériter des propriétés et méthodes d'une autre classe (relation "est-un")
3. **Polymorphisme** : capacité d'un objet à prendre plusieurs formes (surcharge et redéfinition de méthodes)
4. **Abstraction** : cacher la complexité et ne montrer que les fonctionnalités essentielles (classes abstraites et interfaces)

---

### 4. Qu'est-ce qu'une classe et qu'est-ce qu'un objet en Java ?

- **Classe** : modèle ou blueprint qui définit les propriétés (attributs) et comportements (méthodes) que les objets de ce type auront
- **Objet** : instance concrète d'une classe, créée avec le mot-clé `new`

**Exemple :**

```java
class Voiture { // Classe
    String marque;
    void demarrer() { }
}
Voiture maVoiture = new Voiture(); // Objet
```

---

### 5. Différence entre une classe interne et une sous-classe ?

- **Sous-classe** : classe qui hérite d'une classe parent (`extends`), établit une relation d'héritage, peut accéder aux membres publics et protégés du parent
- **Classe interne** : classe définie à l'intérieur d'une autre classe, a accès à tous les membres (même privés) de la classe englobante, utilisée pour le regroupement logique

---

## Questions sur les modificateurs et mots-clés

### 6. À quoi sert le mot-clé `static` ?

Le mot-clé `static` indique que le membre appartient à la classe plutôt qu'aux instances :

- **Variable static** : partagée par toutes les instances de la classe
- **Méthode static** : peut être appelée sans créer d'instance
- **Bloc static** : exécuté une seule fois au chargement de la classe

**Exemple :**

```java
class Compteur {
    static int count = 0; // Partagé par tous les objets
    static void incrementer() { count++; }
}
Compteur.incrementer(); // Appel sans instance
```

---

### 7. Qu'est-ce que le mot-clé `final` et quand l'utiliser ?

`final` empêche la modification :

- **Variable final** : constante, ne peut pas être réassignée
- **Méthode final** : ne peut pas être redéfinie dans les sous-classes
- **Classe final** : ne peut pas être étendue (pas d'héritage)

**Exemple :**

```java
final int MAX = 100; // Constante
final class String { } // Ne peut pas être étendue
```

---

### 8. Quels sont les spécificateurs d'accès en Java ?

- **`public`** : accessible partout
- **`protected`** : accessible dans le même package et les sous-classes
- **`default`** (pas de mot-clé) : accessible uniquement dans le même package
- **`private`** : accessible uniquement dans la même classe

---

## Questions sur la gestion des exceptions

### 9. Expliquez le fonctionnement des blocs Try, Catch et Finally

```java
try {
    // Code susceptible de lever une exception
    int resultat = 10 / 0;
} catch (ArithmeticException e) {
    // Gestion de l'exception
    System.out.println("Division par zéro");
} finally {
    // Toujours exécuté, même si exception ou return
    System.out.println("Nettoyage des ressources");
}
```

Le bloc `finally` est utilisé pour libérer des ressources (fermer fichiers, connexions DB, etc.)

---

### 10. Quelle est la différence entre une exception checked et unchecked ?

- **Checked (vérifiées)** : héritent de `Exception`, doivent être gérées (`try-catch`) ou déclarées (`throws`) au moment de la compilation. Exemples : `IOException`, `SQLException`
- **Unchecked (non vérifiées)** : héritent de `RuntimeException`, ne nécessitent pas de gestion explicite. Exemples : `NullPointerException`, `ArrayIndexOutOfBoundsException`, `ArithmeticException`

---

## Questions sur les Collections et structures de données

### 11. Quels sont les différents types de collections en Java ?

Les principales interfaces du framework Collections :

- **List** : collection ordonnée, accepte les doublons (`ArrayList`, `LinkedList`, `Vector`)
- **Set** : pas de doublons (`HashSet`, `TreeSet`, `LinkedHashSet`)
- **Queue** : file FIFO (`PriorityQueue`, `LinkedList`)
- **Map** : paires clé-valeur (`HashMap`, `TreeMap`, `LinkedHashMap`)

---

### 12. Différence entre ArrayList et LinkedList ?

- **ArrayList** : tableau dynamique, accès rapide par index O(1), insertion/suppression lente au milieu O(n), meilleur pour la lecture
- **LinkedList** : liste doublement chaînée, accès séquentiel O(n), insertion/suppression rapide O(1), meilleur pour les modifications fréquentes

---

### 13. Qu'est-ce qu'un HashMap et quand l'utiliser ?

HashMap est une structure clé-valeur basée sur le hachage :

- Accès/insertion/suppression en O(1) en moyenne
- N'est pas thread-safe (utiliser `ConcurrentHashMap` pour le multithreading)
- Pas d'ordre garanti (utiliser `LinkedHashMap` pour l'ordre d'insertion)
- Accepte une clé null et plusieurs valeurs null

**Exemple :**

```java
HashMap<String, Integer> ages = new HashMap<>();
ages.put("Alice", 25);
int age = ages.get("Alice");
```

---

### 14. Qu'est-ce qu'une classe Singleton ?

Pattern qui garantit qu'une classe n'a qu'une seule instance dans l'application :

```java
public class Singleton {
    private static Singleton instance;
    
    private Singleton() { } // Constructeur privé
    
    public static Singleton getInstance() {
        if (instance == null) {
            instance = new Singleton();
        }
        return instance;
    }
}
```

Utilisé pour : connexions DB, loggers, gestionnaires de configuration.

---

## Questions sur Java 8+ (nouvelles fonctionnalités)

### 15. Qu'est-ce qu'une expression lambda ?

Syntaxe concise pour représenter une fonction anonyme :

```java
// Avant Java 8
List<String> noms = Arrays.asList("Alice", "Bob", "Charlie");
Collections.sort(noms, new Comparator<String>() {
    public int compare(String a, String b) {
        return a.compareTo(b);
    }
});

// Avec lambda
Collections.sort(noms, (a, b) -> a.compareTo(b));
```

---

### 16. Qu'est-ce qu'une interface fonctionnelle ?

Interface avec une seule méthode abstraite, peut être implémentée avec une lambda :

```java
@FunctionalInterface
interface Calculateur {
    int calculer(int a, int b);
}

Calculateur addition = (a, b) -> a + b;
```

Exemples : `Runnable`, `Callable`, `Comparator`, `Predicate`, `Function`

---

### 17. Qu'est-ce que l'API Stream et comment l'utiliser ?

API pour traiter des collections de manière déclarative et fonctionnelle :

```java
List<Integer> nombres = Arrays.asList(1, 2, 3, 4, 5);
int somme = nombres.stream()
    .filter(n -> n % 2 == 0)  // Filtrer les pairs
    .map(n -> n * 2)          // Doubler chaque nombre
    .reduce(0, Integer::sum); // Sommer
```

- **Opérations intermédiaires (lazy)** : `filter`, `map`, `sorted`
- **Opérations terminales** : `collect`, `forEach`, `reduce`

---

### 18. Expliquez la classe Optional

Container pour gérer les valeurs potentiellement nulles et éviter `NullPointerException` :

```java
Optional<String> nom = Optional.ofNullable(getNom());
String result = nom.orElse("Anonyme"); // Valeur par défaut
nom.ifPresent(n -> System.out.println(n)); // Action si présent
```

---

## Questions comportementales et situationnelles

### 19. Décrivez votre expérience avec Java dans vos projets précédents

Utilisez la méthode **STAR** :

- **Situation** : contexte du projet (stage, projet académique)
- **Tâche** : votre rôle et responsabilités
- **Action** : technologies Java utilisées, défis rencontrés
- **Résultat** : résultats obtenus, apprentissages

---

### 20. Comment gérez-vous les délais serrés dans vos projets ?

- Priorisation des fonctionnalités (MVP)
- Découpage en tâches plus petites
- Communication proactive avec l'équipe
- Gestion du temps efficace
- Demande d'aide si nécessaire

---

### 21. Comment travaillez-vous en équipe ?

- Communication claire et régulière
- Utilisation d'outils collaboratifs (Git, Jira)
- Code reviews et pair programming
- Respect des conventions de code
- Écoute et ouverture aux feedbacks

---

## Questions fondamentales sur Spring Boot

### 1. Qu'est-ce que Spring Boot et pourquoi l'utiliser ?

Spring Boot est un framework Spring basé sur Java utilisé pour le développement accéléré d'applications (pour construire des microservices autonomes) avec un support d'auto-configuration et un serveur d'application embarqué comme Tomcat ou Jetty.

**Avantages principaux :**

- Création d'applications Spring autonomes avec une configuration minimale
- Serveur embarqué (Tomcat/Jetty) - pas besoin de déployer des fichiers WAR
- Auto-configuration intelligente basée sur les dépendances du classpath
- Starter POMs pour simplifier la gestion des dépendances
- Fonctionnalités prêtes pour la production (métriques, health checks, monitoring)
- Absolument aucune exigence de configuration XML

---

### 2. Quelle est la différence entre Spring, Spring MVC et Spring Boot ?

La caractéristique la plus importante de Spring Framework est l'injection de dépendances. Spring MVC Framework fournit un moyen découplé de développement d'applications Web avec des concepts simples comme Dispatcher Servlet, ModelAndView et View Resolver. Le problème avec Spring et Spring MVC est la quantité de configuration nécessaire, que Spring Boot résout grâce à l'auto-configuration et aux projets de démarrage.

**En résumé :**

- **Spring Framework** : conteneur IoC/DI de base
- **Spring MVC** : framework web pour créer des applications web et REST APIs
- **Spring Boot** : couche au-dessus de Spring qui simplifie la configuration et accélère le développement

---

### 3. Qu'est-ce que l'auto-configuration dans Spring Boot ?

Spring Boot configure automatiquement votre application en fonction des dépendances que vous avez ajoutées au projet en utilisant des annotations.

**Comment ça marche :**

```java
@SpringBootApplication // Combine @Configuration, @EnableAutoConfiguration, @ComponentScan
public class MonApplication {
    public static void main(String[] args) {
        SpringApplication.run(MonApplication.class, args);
    }
}
```

**Par exemple :**

- Si `spring-boot-starter-data-jpa` est présent → Spring Boot configure automatiquement un DataSource, EntityManager, etc.
- Si `spring-boot-starter-web` est présent → configure un serveur Tomcat embarqué, DispatcherServlet, etc.

---

### 4. Qu'est-ce que l'annotation @SpringBootApplication ?

C'est une annotation combinée qui équivaut à :

```java
@Configuration        // Définit la classe comme source de beans
@EnableAutoConfiguration  // Active l'auto-configuration
@ComponentScan       // Scanne les composants dans le package actuel et sous-packages
```

---

### 5. Quels sont les Spring Boot Starters principaux ?

Spring Boot fournit un certain nombre de dépendances Starter, dont les plus couramment utilisées sont Data JPA starter, Test Starter, Security starter, Web starter, Mail starter, Thymeleaf starter.

**Liste détaillée :**

- `spring-boot-starter-web` : pour créer des applications web et REST APIs (inclut Tomcat, Spring MVC)
- `spring-boot-starter-data-jpa` : pour JPA avec Hibernate
- `spring-boot-starter-security` : pour Spring Security
- `spring-boot-starter-test` : pour les tests (JUnit, Mockito, AssertJ)
- `spring-boot-starter-thymeleaf` : moteur de templates
- `spring-boot-starter-actuator` : monitoring et métriques
- `spring-boot-starter-validation` : validation des beans

---

## Questions sur la configuration

### 6. Qu'est-ce que application.properties / application.yml ?

Fichiers de configuration pour définir les propriétés de l'application :

**application.properties :**

```properties
server.port=8080
spring.datasource.url=jdbc:mysql://localhost:3306/madb
spring.datasource.username=root
spring.datasource.password=password
spring.jpa.hibernate.ddl-auto=update
```

**Ou en YAML :**

```yaml
server:
  port: 8080
spring:
  datasource:
    url: jdbc:mysql://localhost:3306/madb
    username: root
    password: password
```

---

### 7. Comment gérer différents profils (dev, prod, test) ?

Utilisation de profils Spring pour différents environnements :

```properties
# application-dev.properties
spring.datasource.url=jdbc:h2:mem:testdb

# application-prod.properties
spring.datasource.url=jdbc:mysql://prod-server:3306/proddb
```

**Activation :**

```bash
java -jar app.jar --spring.profiles.active=prod
```

**Ou dans le code :**

```java
@Profile("dev")
@Configuration
public class DevConfig { }
```

---

### 8. Comment externaliser la configuration ?

Spring Boot utilise un système de priorité pour la gestion des configurations qui permet de définir des valeurs par défaut pour les paramètres de configuration, tout en permettant de les surcharger à l'aide de fichiers de propriétés externes ou de variables d'environnement.

**Ordre de priorité (du plus au moins prioritaire) :**

1. Arguments de ligne de commande
2. Variables d'environnement système
3. Fichiers application.properties externes
4. Fichiers application.properties dans le JAR
5. Valeurs par défaut

---

## Questions sur les serveurs embarqués

### 9. Quels serveurs embarqués sont supportés par Spring Boot ?

Spring Boot prend en charge trois principaux conteneurs intégrés : **Tomcat** (par défaut), **Jetty** et **Undertow**.

---

### 10. Comment remplacer Tomcat par Jetty ?

Il est possible de remplacer Embedded Tomcat par n'importe quel autre serveur en utilisant les dépendances de démarrage comme `spring-boot-starter-jetty`.

```xml
<dependency>
    <groupId>org.springframework.boot</groupId>
    <artifactId>spring-boot-starter-web</artifactId>
    <exclusions>
        <exclusion>
            <groupId>org.springframework.boot</groupId>
            <artifactId>spring-boot-starter-tomcat</artifactId>
        </exclusion>
    </exclusions>
</dependency>
<dependency>
    <groupId>org.springframework.boot</groupId>
    <artifactId>spring-boot-starter-jetty</artifactId>
</dependency>
```

---

### 11. Comment désactiver le serveur web embarqué ?

Pour créer une application non-web :

```properties
spring.main.web-application-type=none
```

**Ou :**

```java
SpringApplication app = new SpringApplication(MonApplication.class);
app.setWebApplicationType(WebApplicationType.NONE);
app.run(args);
```

---

## Questions sur les REST APIs

### 12. Comment créer un REST Controller ?

```java
@RestController
@RequestMapping("/api/users")
public class UserController {
    
    @Autowired
    private UserService userService;
    
    @GetMapping
    public List<User> getAllUsers() {
        return userService.findAll();
    }
    
    @GetMapping("/{id}")
    public ResponseEntity<User> getUserById(@PathVariable Long id) {
        return userService.findById(id)
            .map(ResponseEntity::ok)
            .orElse(ResponseEntity.notFound().build());
    }
    
    @PostMapping
    public User createUser(@RequestBody @Valid User user) {
        return userService.save(user);
    }
    
    @PutMapping("/{id}")
    public User updateUser(@PathVariable Long id, @RequestBody User user) {
        return userService.update(id, user);
    }
    
    @DeleteMapping("/{id}")
    public ResponseEntity<Void> deleteUser(@PathVariable Long id) {
        userService.delete(id);
        return ResponseEntity.noContent().build();
    }
}
```

---

### 13. Quelle est la différence entre @Controller et @RestController ?

- **@Controller** : utilisé pour les applications MVC traditionnelles, retourne des vues (HTML)
- **@RestController** : combinaison de `@Controller` + `@ResponseBody`, retourne directement des données JSON/XML

```java
@RestController = @Controller + @ResponseBody
```

---

### 14. Qu'est-ce que @PathVariable ?

L'annotation `@PathVariable` vous aide à extraire directement les informations de l'URI.

```java
@GetMapping("/users/{id}/posts/{postId}")
public Post getPost(@PathVariable Long id, @PathVariable Long postId) {
    return postService.findPost(id, postId);
}

// URL: /users/5/posts/123
// id = 5, postId = 123
```

---

### 15. Différence entre @RequestParam et @PathVariable ?

```java
// @PathVariable - partie de l'URL
@GetMapping("/users/{id}")
public User getUser(@PathVariable Long id) { }
// URL: /users/123

// @RequestParam - paramètre de requête
@GetMapping("/users")
public List<User> searchUsers(@RequestParam String name) { }
// URL: /users?name=John
```

---

## Questions sur Spring Data JPA

### 16. Comment configurer JPA dans Spring Boot ?

**pom.xml :**

```xml
<dependency>
    <groupId>org.springframework.boot</groupId>
    <artifactId>spring-boot-starter-data-jpa</artifactId>
</dependency>
<dependency>
    <groupId>com.mysql</groupId>
    <artifactId>mysql-connector-j</artifactId>
</dependency>
```

**application.properties :**

```properties
spring.datasource.url=jdbc:mysql://localhost:3306/madb
spring.datasource.username=root
spring.datasource.password=password
spring.jpa.hibernate.ddl-auto=update
spring.jpa.show-sql=true
```

---

### 17. Qu'est-ce qu'un Repository dans Spring Data JPA ?

```java
@Entity
public class User {
    @Id
    @GeneratedValue(strategy = GenerationType.IDENTITY)
    private Long id;
    private String name;
    private String email;
    // getters/setters
}

public interface UserRepository extends JpaRepository<User, Long> {
    // Méthodes automatiquement générées :
    // save(), findById(), findAll(), deleteById(), etc.
    
    // Requêtes personnalisées par convention de nommage
    List<User> findByName(String name);
    Optional<User> findByEmail(String email);
    List<User> findByNameContaining(String keyword);
    
    // Requêtes JPQL personnalisées
    @Query("SELECT u FROM User u WHERE u.email LIKE %:domain")
    List<User> findByEmailDomain(@Param("domain") String domain);
}
```

---

### 18. Différence entre JpaRepository, CrudRepository et PagingAndSortingRepository ?

- **CrudRepository** : opérations CRUD de base (save, findById, findAll, delete)
- **PagingAndSortingRepository** : étend CrudRepository + pagination et tri
- **JpaRepository** : étend PagingAndSortingRepository + méthodes spécifiques JPA (flush, saveAndFlush, etc.)

**Hiérarchie :** `JpaRepository` > `PagingAndSortingRepository` > `CrudRepository`

---

## Questions sur l'injection de dépendances

### 19. Quels sont les types d'injection de dépendances dans Spring ?

Vous pouvez le faire de trois façons différentes, mais dans le Spring Framework, les injections de constructeur et de Setter sont les plus utilisées.

**1. Injection par constructeur (recommandée) :**

```java
@Service
public class UserService {
    private final UserRepository userRepository;
    
    @Autowired // Optionnel si un seul constructeur
    public UserService(UserRepository userRepository) {
        this.userRepository = userRepository;
    }
}
```

**2. Injection par setter :**

```java
@Service
public class UserService {
    private UserRepository userRepository;
    
    @Autowired
    public void setUserRepository(UserRepository userRepository) {
        this.userRepository = userRepository;
    }
}
```

**3. Injection par champ (déconseillée) :**

```java
@Service
public class UserService {
    @Autowired
    private UserRepository userRepository;
}
```

**Pourquoi préférer l'injection par constructeur ?**

- Rend les dépendances immutables (final)
- Facilite les tests unitaires
- Rend les dépendances obligatoires explicites
- Évite les NullPointerException

---

### 20. Différence entre @Component, @Service, @Repository et @Controller ?

Tous sont des stéréotypes pour créer des beans Spring, mais avec des sémantiques différentes :

- **@Component** : annotation générique pour tout composant Spring
- **@Service** : couche métier/service
- **@Repository** : couche d'accès aux données (ajoute la traduction des exceptions)
- **@Controller** : couche de présentation MVC
- **@RestController** : contrôleur REST (`@Controller` + `@ResponseBody`)

```java
@Component
class GenericComponent { }

@Service
class UserService { }

@Repository
interface UserRepository extends JpaRepository<User, Long> { }

@RestController
class UserController { }
```

---

## Questions sur Spring Boot Actuator

### 21. Qu'est-ce que Spring Boot Actuator ?

Module qui fournit des endpoints prêts pour la production pour surveiller et gérer l'application :

```xml
<dependency>
    <groupId>org.springframework.boot</groupId>
    <artifactId>spring-boot-starter-actuator</artifactId>
</dependency>
```

**Endpoints principaux :**

- `/actuator/health` : état de santé de l'application
- `/actuator/info` : informations sur l'application
- `/actuator/metrics` : métriques (mémoire, CPU, requêtes HTTP)
- `/actuator/env` : variables d'environnement
- `/actuator/loggers` : configuration des logs
- `/actuator/beans` : tous les beans Spring

```properties
# Activer tous les endpoints
management.endpoints.web.exposure.include=*
# Ou spécifiquement
management.endpoints.web.exposure.include=health,info,metrics
```

---

### 22. Comment créer un custom health indicator ?

```java
@Component
public class CustomHealthIndicator implements HealthIndicator {
    
    @Override
    public Health health() {
        boolean serviceUp = checkExternalService();
        
        if (serviceUp) {
            return Health.up()
                .withDetail("service", "disponible")
                .build();
        }
        return Health.down()
            .withDetail("service", "indisponible")
            .build();
    }
    
    private boolean checkExternalService() {
        // Logique de vérification
        return true;
    }
}
```

---

## Questions sur la sécurité

### 23. Comment sécuriser une application Spring Boot ?

```xml
<dependency>
    <groupId>org.springframework.boot</groupId>
    <artifactId>spring-boot-starter-security</artifactId>
</dependency>
```

**Configuration basique :**

```java
@Configuration
@EnableWebSecurity
public class SecurityConfig {
    
    @Bean
    public SecurityFilterChain filterChain(HttpSecurity http) throws Exception {
        http
            .authorizeHttpRequests(auth -> auth
                .requestMatchers("/public/**").permitAll()
                .requestMatchers("/admin/**").hasRole("ADMIN")
                .anyRequest().authenticated()
            )
            .formLogin(form -> form
                .loginPage("/login")
                .permitAll()
            )
            .logout(logout -> logout.permitAll());
        
        return http.build();
    }
    
    @Bean
    public PasswordEncoder passwordEncoder() {
        return new BCryptPasswordEncoder();
    }
}
```

---

### 24. Comment implémenter JWT avec Spring Boot ?

```java
@Service
public class JwtService {
    
    private static final String SECRET_KEY = "votre-cle-secrete";
    
    public String generateToken(String username) {
        return Jwts.builder()
            .setSubject(username)
            .setIssuedAt(new Date())
            .setExpiration(new Date(System.currentTimeMillis() + 86400000)) // 24h
            .signWith(SignatureAlgorithm.HS256, SECRET_KEY)
            .compact();
    }
    
    public String extractUsername(String token) {
        return Jwts.parser()
            .setSigningKey(SECRET_KEY)
            .parseClaimsJws(token)
            .getBody()
            .getSubject();
    }
}
```

---

## Questions sur les tests Spring Boot

### 25. Comment tester une application Spring Boot ?

```java
@SpringBootTest
@AutoConfigureMockMvc
class UserControllerTest {
    
    @Autowired
    private MockMvc mockMvc;
    
    @MockBean
    private UserService userService;
    
    @Test
    void testGetAllUsers() throws Exception {
        List<User> users = Arrays.asList(
            new User(1L, "Alice", "alice@test.com"),
            new User(2L, "Bob", "bob@test.com")
        );
        
        when(userService.findAll()).thenReturn(users);
        
        mockMvc.perform(get("/api/users"))
            .andExpect(status().isOk())
            .andExpect(jsonPath("$.length()").value(2))
            .andExpect(jsonPath("$[0].name").value("Alice"));
    }
    
    @Test
    void testCreateUser() throws Exception {
        User user = new User(null, "Charlie", "charlie@test.com");
        User savedUser = new User(1L, "Charlie", "charlie@test.com");
        
        when(userService.save(any())).thenReturn(savedUser);
        
        mockMvc.perform(post("/api/users")
                .contentType(MediaType.APPLICATION_JSON)
                .content("{\"name\":\"Charlie\",\"email\":\"charlie@test.com\"}"))
            .andExpect(status().isOk())
            .andExpect(jsonPath("$.id").value(1));
    }
}
```

**Test du repository :**

```java
@DataJpaTest
class UserRepositoryTest {
    
    @Autowired
    private UserRepository userRepository;
    
    @Test
    void testFindByEmail() {
        User user = new User(null, "Test", "test@example.com");
        userRepository.save(user);
        
        Optional<User> found = userRepository.findByEmail("test@example.com");
        
        assertTrue(found.isPresent());
        assertEquals("Test", found.get().getName());
    }
}
```

---

## Questions sur les exceptions Spring Boot

### 26. Comment gérer les exceptions globalement ?

```java
@RestControllerAdvice
public class GlobalExceptionHandler {
    
    @ExceptionHandler(ResourceNotFoundException.class)
    public ResponseEntity<ErrorResponse> handleResourceNotFound(
            ResourceNotFoundException ex) {
        ErrorResponse error = new ErrorResponse(
            HttpStatus.NOT_FOUND.value(),
            ex.getMessage(),
            LocalDateTime.now()
        );
        return new ResponseEntity<>(error, HttpStatus.NOT_FOUND);
    }
    
    @ExceptionHandler(MethodArgumentNotValidException.class)
    public ResponseEntity<ErrorResponse> handleValidationException(
            MethodArgumentNotValidException ex) {
        Map<String, String> errors = new HashMap<>();
        ex.getBindingResult().getFieldErrors().forEach(error ->
            errors.put(error.getField(), error.getDefaultMessage())
        );
        
        ErrorResponse error = new ErrorResponse(
            HttpStatus.BAD_REQUEST.value(),
            "Erreur de validation",
            errors
        );
        return new ResponseEntity<>(error, HttpStatus.BAD_REQUEST);
    }
    
    @ExceptionHandler(Exception.class)
    public ResponseEntity<ErrorResponse> handleGlobalException(Exception ex) {
        ErrorResponse error = new ErrorResponse(
            HttpStatus.INTERNAL_SERVER_ERROR.value(),
            "Erreur interne du serveur",
            LocalDateTime.now()
        );
        return new ResponseEntity<>(error, HttpStatus.INTERNAL_SERVER_ERROR);
    }
}
```

---

## Questions sur les filtres

### 27. Comment ajouter un filtre dans Spring Boot ?

Il existe trois méthodes pour ajouter un filtre à l'application Spring Boot : en implémentant l'interface Filter, utilisation de FilterRegistrationBean, utilisation du contrôleur MVC.

**Méthode 1 : Implémenter Filter**

```java
@Component
public class LoggingFilter implements Filter {
    
    @Override
    public void doFilter(ServletRequest request, ServletResponse response, 
                         FilterChain chain) throws IOException, ServletException {
        HttpServletRequest req = (HttpServletRequest) request;
        System.out.println("Request: " + req.getMethod() + " " + req.getRequestURI());
        
        chain.doFilter(request, response);
        
        System.out.println("Response completed");
    }
}
```

**Méthode 2 : FilterRegistrationBean**

```java
@Configuration
public class FilterConfig {
    
    @Bean
    public FilterRegistrationBean<LoggingFilter> loggingFilter() {
        FilterRegistrationBean<LoggingFilter> registrationBean = 
            new FilterRegistrationBean<>();
        
        registrationBean.setFilter(new LoggingFilter());
        registrationBean.addUrlPatterns("/api/*");
        registrationBean.setOrder(1);
        
        return registrationBean;
    }
}
```

---

## Questions avancées Spring Boot

### 28. Qu'est-ce que Spring Boot DevTools ?

Module qui améliore l'expérience de développement :

```xml
<dependency>
    <groupId>org.springframework.boot</groupId>
    <artifactId>spring-boot-devtools</artifactId>
    <optional>true</optional>
</dependency>
```

**Fonctionnalités :**

- Redémarrage automatique quand le code change
- LiveReload pour rafraîchir le navigateur
- Désactivation du cache des templates en développement
- Configuration par défaut optimisée pour le développement

---

### 29. Comment exécuter du code au démarrage de l'application ?

```java
// Méthode 1 : CommandLineRunner
@Component
public class StartupRunner implements CommandLineRunner {
    @Override
    public void run(String... args) throws Exception {
        System.out.println("Application démarrée !");
    }
}

// Méthode 2 : ApplicationRunner
@Component
public class AppRunner implements ApplicationRunner {
    @Override
    public void run(ApplicationArguments args) throws Exception {
        System.out.println("Initialisation...");
    }
}

// Méthode 3 : @PostConstruct
@Component
public class DataInitializer {
    @PostConstruct
    public void init() {
        System.out.println("Bean initialisé !");
    }
}
```

---

### 30. Comment gérer plusieurs sources de données ?

```java
@Configuration
public class DataSourceConfig {
    
    @Bean
    @Primary
    @ConfigurationProperties(prefix = "spring.datasource.primary")
    public DataSource primaryDataSource() {
        return DataSourceBuilder.create().build();
    }
    
    @Bean
    @ConfigurationProperties(prefix = "spring.datasource.secondary")
    public DataSource secondaryDataSource() {
        return DataSourceBuilder.create().build();
    }
}
```

```properties
# application.properties
spring.datasource.primary.url=jdbc:mysql://localhost:3306/db1
spring.datasource.primary.username=user1

spring.datasource.secondary.url=jdbc:mysql://localhost:3306/db2
spring.datasource.secondary.username=user2
```

---

## Spring Framework Core - IoC et Injection de Dépendances

### 31. Qu'est-ce que l'Inversion de Contrôle (IoC) ?

Le conteneur d'inversion de contrôle de Spring est au cœur du framework Spring. L'inversion de contrôle est une pratique générale du génie logiciel qui permet de transférer le contrôle sur des parties d'un programme ou des objets à un cadre/conteneur. L'inversion de contrôle permet au framework ou au conteneur de prendre le contrôle du programme et d'effectuer des appels à notre code.

---

### 32. Qu'est-ce que l'injection de dépendances ?

L'injection de dépendances est le mécanisme par lequel Spring IoC fournit les dépendances d'un objet au moment de sa création plutôt que de laisser l'objet les créer lui-même.

---

### 33. Quels sont les types d'injection de dépendances ?

Vous pouvez faire une injection de dépendances de trois façons différentes : injection par constructeur, injection par setter, et injection par champ. Dans le Spring Framework, les injections de constructeur et de Setter sont les plus utilisées.

```java
// Injection par constructeur (recommandée)
@Service
public class UserService {
    private final UserRepository userRepository;
    
    @Autowired
    public UserService(UserRepository userRepository) {
        this.userRepository = userRepository;
    }
}

// Injection par setter
@Service
public class UserService {
    private UserRepository userRepository;
    
    @Autowired
    public void setUserRepository(UserRepository userRepository) {
        this.userRepository = userRepository;
    }
}

// Injection par champ (à éviter en production)
@Service
public class UserService {
    @Autowired
    private UserRepository userRepository;
}
```

---

### 34. Qu'est-ce qu'un Bean Spring ?

Un Bean est un objet géré par le conteneur Spring IoC. Les beans sont créés, configurés et gérés par le framework Spring.

```java
@Configuration
public class AppConfig {
    
    @Bean
    public UserService userService() {
        return new UserService();
    }
}
```

---

### 35. Quelles sont les portées (scopes) des beans ?

- **Singleton** (par défaut) : Une seule instance par conteneur Spring
- **Prototype** : Une nouvelle instance à chaque demande
- **Request** : Une instance par requête HTTP (applications web)
- **Session** : Une instance par session HTTP
- **Application** : Une instance par ServletContext
- **WebSocket** : Une instance par session WebSocket

```java
@Component
@Scope("prototype")
public class MonBean {
    // Une nouvelle instance sera créée à chaque injection
}
```

---

## Spring Data JPA et Hibernate

### 36. Qu'est-ce que Spring Data JPA ?

Spring Data JPA est un sous-projet de Spring Data qui simplifie l'implémentation de la couche d'accès aux données en réduisant le code boilerplate nécessaire pour interagir avec les bases de données relationnelles.

---

### 37. Quelle est la différence entre JPA et Hibernate ?

**JPA (Java Persistence API)** est une spécification, tandis que **Hibernate** est une implémentation (provider) de cette spécification. Spring Data JPA utilise Hibernate par défaut comme provider.

---

### 38. Qu'est-ce qu'un Repository dans Spring Data ?

Un Repository est une interface qui fournit des méthodes CRUD (Create, Read, Update, Delete) automatiquement implémentées par Spring Data.

```java
public interface UserRepository extends JpaRepository<User, Long> {
    // Méthodes CRUD héritées : save(), findById(), findAll(), deleteById()
    
    // Requêtes dérivées du nom de la méthode
    List<User> findByLastName(String lastName);
    User findByEmail(String email);
    List<User> findByAgeGreaterThan(int age);
    
    // Requête personnalisée avec @Query
    @Query("SELECT u FROM User u WHERE u.email = ?1")
    User findUserByEmail(String email);
    
    // Requête native SQL
    @Query(value = "SELECT * FROM users WHERE status = ?1", nativeQuery = true)
    List<User> findByStatusNative(String status);
}
```

---

### 39. Qu'est-ce qu'une Entity JPA ?

Une Entity est une classe Java annotée avec `@Entity` qui représente une table dans la base de données.

```java
@Entity
@Table(name = "users")
public class User {
    
    @Id
    @GeneratedValue(strategy = GenerationType.IDENTITY)
    private Long id;
    
    @Column(nullable = false, unique = true)
    private String email;
    
    @Column(nullable = false)
    private String password;
    
    private String firstName;
    private String lastName;
    
    @Temporal(TemporalType.TIMESTAMP)
    private Date createdAt;
    
    @OneToMany(mappedBy = "user", cascade = CascadeType.ALL)
    private List<Order> orders;
    
    // Getters et Setters
}
```

---

### 40. Quelles sont les annotations JPA importantes ?

- **@Entity** : Marque une classe comme entité JPA
- **@Table** : Spécifie le nom de la table
- **@Id** : Définit la clé primaire
- **@GeneratedValue** : Stratégie de génération de la clé
- **@Column** : Propriétés de la colonne
- **@OneToOne, @OneToMany, @ManyToOne, @ManyToMany** : Relations entre entités
- **@JoinColumn** : Spécifie la colonne de jointure
- **@Transient** : Exclut un champ de la persistance

---

### 41. Qu'est-ce que la propriété spring.jpa.hibernate.ddl-auto ?

Cette propriété contrôle le comportement de Hibernate vis-à-vis du schéma de base de données :

- **none** : Aucune action (par défaut en production)
- **validate** : Valide le schéma, ne fait aucun changement
- **update** : Met à jour le schéma si nécessaire
- **create** : Crée le schéma, détruit les données précédentes
- **create-drop** : Crée le schéma au démarrage, le détruit à l'arrêt

---

## Spring MVC

### 42. Qu'est-ce que Spring MVC ?

Spring MVC Framework fournit un moyen découplé de développement d'applications Web. Avec des concepts simples comme Dispatcher Servlet, ModelAndView et View Resolver, il facilite le développement d'applications Web.

---

### 43. Qu'est-ce que le DispatcherServlet ?

Le DispatcherServlet est le contrôleur frontal (Front Controller) dans Spring MVC. Il reçoit toutes les requêtes HTTP entrantes et les dispatche aux contrôleurs appropriés.

---

### 44. Qu'est-ce qu'un Controller dans Spring MVC ?

Un Controller gère les requêtes HTTP et retourne une vue ou des données.

```java
@Controller
public class UserController {
    
    @Autowired
    private UserService userService;
    
    // Retourne une vue
    @GetMapping("/users")
    public String listUsers(Model model) {
        model.addAttribute("users", userService.findAll());
        return "user-list"; // Nom de la vue
    }
    
    // Retourne du JSON (REST)
    @GetMapping("/api/users")
    @ResponseBody
    public List<User> getUsersJson() {
        return userService.findAll();
    }
}

// Ou avec @RestController (combine @Controller et @ResponseBody)
@RestController
@RequestMapping("/api")
public class UserRestController {
    
    @Autowired
    private UserService userService;
    
    @GetMapping("/users")
    public List<User> getUsers() {
        return userService.findAll();
    }
    
    @PostMapping("/users")
    public User createUser(@RequestBody User user) {
        return userService.save(user);
    }
    
    @GetMapping("/users/{id}")
    public User getUser(@PathVariable Long id) {
        return userService.findById(id);
    }
    
    @PutMapping("/users/{id}")
    public User updateUser(@PathVariable Long id, @RequestBody User user) {
        return userService.update(id, user);
    }
    
    @DeleteMapping("/users/{id}")
    public void deleteUser(@PathVariable Long id) {
        userService.deleteById(id);
    }
}
```

---

### 45. Quelles sont les annotations importantes de Spring MVC ?

- **@Controller** : Marque une classe comme contrôleur MVC
- **@RestController** : Combine @Controller et @ResponseBody
- **@RequestMapping** : Mappe une URL à une méthode
- **@GetMapping, @PostMapping, @PutMapping, @DeleteMapping, @PatchMapping** : Raccourcis pour HTTP
- **@PathVariable** : Extrait une variable de l'URL
- **@RequestParam** : Extrait un paramètre de requête
- **@RequestBody** : Convertit le corps de la requête en objet
- **@ResponseBody** : Sérialise la réponse en JSON/XML

---

## Spring Security

### 46. Qu'est-ce que Spring Security ?

Spring Security est un framework puissant et hautement personnalisable pour l'authentification et le contrôle d'accès dans les applications Java. Il protège contre les menaces courantes comme CSRF, XSS, etc.

---

### 47. Comment configurer Spring Security dans Spring Boot ?

```java
@Configuration
@EnableWebSecurity
public class SecurityConfig {
    
    @Bean
    public SecurityFilterChain filterChain(HttpSecurity http) throws Exception {
        http
            .authorizeHttpRequests(auth -> auth
                .requestMatchers("/", "/public/**").permitAll()
                .requestMatchers("/admin/**").hasRole("ADMIN")
                .anyRequest().authenticated()
            )
            .formLogin(form -> form
                .loginPage("/login")
                .defaultSuccessUrl("/dashboard")
                .permitAll()
            )
            .logout(logout -> logout
                .logoutSuccessUrl("/")
                .permitAll()
            );
        
        return http.build();
    }
    
    @Bean
    public PasswordEncoder passwordEncoder() {
        return new BCryptPasswordEncoder();
    }
}
```

---

### 48. Comment implémenter l'authentification avec base de données ?

```java
// Entity User
@Entity
public class User {
    @Id
    @GeneratedValue(strategy = GenerationType.IDENTITY)
    private Long id;
    
    private String username;
    private String password;
    private String role;
    
    // Getters et Setters
}

// UserRepository
public interface UserRepository extends JpaRepository<User, Long> {
    Optional<User> findByUsername(String username);
}

// UserDetailsService personnalisé
@Service
public class CustomUserDetailsService implements UserDetailsService {
    
    @Autowired
    private UserRepository userRepository;
    
    @Override
    public UserDetails loadUserByUsername(String username) 
            throws UsernameNotFoundException {
        User user = userRepository.findByUsername(username)
            .orElseThrow(() -> new UsernameNotFoundException("User not found"));
        
        return org.springframework.security.core.userdetails.User
            .withUsername(user.getUsername())
            .password(user.getPassword())
            .roles(user.getRole())
            .build();
    }
}
```

---

### 49. Qu'est-ce que l'encodage de mot de passe ?

Spring Security utilise des encodeurs de mots de passe pour sécuriser les mots de passe stockés. BCryptPasswordEncoder est le plus recommandé.

```java
@Bean
public PasswordEncoder passwordEncoder() {
    return new BCryptPasswordEncoder();
}

// Utilisation
String encodedPassword = passwordEncoder.encode("motdepasse");
```

---

### 50. Qu'est-ce que CSRF ?

CSRF (Cross-Site Request Forgery) est une attaque où un site malveillant trompe un utilisateur authentifié pour exécuter des actions non désirées. Spring Security active la protection CSRF par défaut.

---

## Spring AOP (Aspect-Oriented Programming)

### 51. Qu'est-ce que la Programmation Orientée Aspect ?

La programmation orientée aspect (POA) est utilisée pour implémenter des fonctionnalités transverses (cross-cutting concerns). Elle permet de rendre l'architecture plus modulaire. Un aspect représente une catégorie d'actions à réaliser dans certaines conditions, par exemple, gérer les transactions, produire des informations de log, mettre en cache des informations.

---

### 52. Quelle est la terminologie AOP ?

La POA introduit un vocabulaire spécifique : Aspect (la problématique spécifique que l'on veut ajouter transversalement), Point de jonction (le point dans le flot d'exécution d'un programme à partir duquel on souhaite ajouter la logique), et Advice (l'action particulière de l'aspect à exécuter quand le programme atteint le point de jonction).

**Vocabulaire AOP complet :**

- **Aspect** : Module qui encapsule une préoccupation transverse
- **Join Point** : Point dans l'exécution du programme (appel de méthode avec Spring AOP)
- **Advice** : Action exécutée à un join point
- **Pointcut** : Expression qui sélectionne les join points
- **Weaving** : Processus d'insertion des aspects dans le code

---

### 53. Quels sont les types d'Advice ?

Spring AOP fournit plusieurs types d'advices : `@Before` (exécuté avant l'appel d'une méthode ciblée), `@After` (exécuté après l'appel, que celui-ci réussisse ou échoue), `@AfterReturning` (exécuté après un retour normal de la méthode), `@AfterThrowing` (exécuté en cas d'exception), et `@Around` (englobe l'exécution de la méthode, permettant un contrôle total).

---

### 54. Comment créer un Aspect dans Spring ?

```java
@Aspect
@Component
public class LoggingAspect {
    
    // Pointcut - définit où l'aspect s'applique
    @Pointcut("execution(* com.example.service.*.*(..))")
    public void serviceMethods() {}
    
    // Before advice - avant l'exécution
    @Before("serviceMethods()")
    public void logBefore(JoinPoint joinPoint) {
        System.out.println("Avant l'exécution de: " + 
            joinPoint.getSignature().getName());
    }
    
    // After returning - après succès
    @AfterReturning(pointcut = "serviceMethods()", returning = "result")
    public void logAfterReturning(JoinPoint joinPoint, Object result) {
        System.out.println("Méthode retournée avec succès: " + result);
    }
    
    // After throwing - en cas d'exception
    @AfterThrowing(pointcut = "serviceMethods()", throwing = "error")
    public void logAfterThrowing(JoinPoint joinPoint, Throwable error) {
        System.out.println("Exception levée: " + error.getMessage());
    }
    
    // Around advice - contrôle total
    @Around("serviceMethods()")
    public Object logAround(ProceedingJoinPoint joinPoint) throws Throwable {
        long start = System.currentTimeMillis();
        
        System.out.println("Début: " + joinPoint.getSignature().getName());
        
        Object result = joinPoint.proceed(); // Exécute la méthode
        
        long duration = System.currentTimeMillis() - start;
        System.out.println("Fin: " + duration + "ms");
        
        return result;
    }
}
```

---

### 55. Comment activer AOP dans Spring Boot ?

La solution la plus simple si vous êtes dans un contexte d'application Spring Boot est de rajouter la dépendance au starter AOP.

```xml
<dependency>
    <groupId>org.springframework.boot</groupId>
    <artifactId>spring-boot-starter-aop</artifactId>
</dependency>
```

---

### 56. Exemples d'expressions Pointcut

```java
// Toutes les méthodes d'une classe spécifique
@Pointcut("execution(* com.example.service.UserService.*(..))")

// Toutes les méthodes publiques
@Pointcut("execution(public * *(..))")

// Toutes les méthodes commençant par "get"
@Pointcut("execution(* get*(..))")

// Toutes les méthodes dans un package et ses sous-packages
@Pointcut("execution(* com.example..*.*(..))")

// Méthodes annotées avec une annotation spécifique
@Pointcut("@annotation(org.springframework.transaction.annotation.Transactional)")

// Combinaison de pointcuts
@Pointcut("serviceMethods() && !execution(* com.example.service.LogService.*(..))")
```

---

## Gestion des Transactions

### 57. Comment gérer les transactions dans Spring ?

Spring gère les transactions de manière déclarative avec l'annotation `@Transactional`.

```java
@Service
public class UserService {
    
    @Autowired
    private UserRepository userRepository;
    
    @Autowired
    private AuditRepository auditRepository;
    
    @Transactional
    public void createUser(User user) {
        // Si une exception est levée, tout est rollback
        userRepository.save(user);
        auditRepository.save(new Audit("User created: " + user.getId()));
    }
    
    @Transactional(readOnly = true)
    public User getUser(Long id) {
        return userRepository.findById(id).orElse(null);
    }
    
    @Transactional(rollbackFor = Exception.class)
    public void updateUser(User user) throws Exception {
        // Rollback même pour les checked exceptions
        userRepository.save(user);
    }
    
    @Transactional(propagation = Propagation.REQUIRES_NEW)
    public void independentTransaction() {
        // Crée une nouvelle transaction indépendante
    }
}
```

---

### 58. Quels sont les niveaux de propagation des transactions ?

- **REQUIRED** (défaut) : Rejoint une transaction existante ou en crée une nouvelle
- **REQUIRES_NEW** : Crée toujours une nouvelle transaction
- **NESTED** : Exécute dans une transaction imbriquée
- **MANDATORY** : Doit être appelé dans une transaction existante
- **SUPPORTS** : Rejoint une transaction si elle existe
- **NOT_SUPPORTED** : Exécute en dehors d'une transaction
- **NEVER** : Lève une exception si appelé dans une transaction

---

## Validation

### 59. Comment valider les données dans Spring Boot ?

```java
// Entity avec validations
@Entity
public class User {
    
    @Id
    @GeneratedValue(strategy = GenerationType.IDENTITY)
    private Long id;
    
    @NotBlank(message = "Le nom d'utilisateur est obligatoire")
    @Size(min = 3, max = 20, message = "Le nom doit contenir entre 3 et 20 caractères")
    private String username;
    
    @NotBlank(message = "L'email est obligatoire")
    @Email(message = "Format d'email invalide")
    private String email;
    
    @NotNull
    @Min(value = 18, message = "L'âge minimum est 18 ans")
    @Max(value = 100, message = "L'âge maximum est 100 ans")
    private Integer age;
    
    @Pattern(regexp = "^\\+?[0-9]{10,}$", message = "Numéro de téléphone invalide")
    private String phone;
}

// Controller avec validation
@RestController
@RequestMapping("/api/users")
public class UserController {
    
    @PostMapping
    public ResponseEntity<?> createUser(@Valid @RequestBody User user, 
                                       BindingResult result) {
        if (result.hasErrors()) {
            Map<String, String> errors = new HashMap<>();
            result.getFieldErrors().forEach(error -> 
                errors.put(error.getField(), error.getDefaultMessage())
            );
            return ResponseEntity.badRequest().body(errors);
        }
        
        return ResponseEntity.ok(userService.save(user));
    }
}
```

**Annotations de validation courantes :**

- **@NotNull** : Ne doit pas être null
- **@NotEmpty** : Ne doit pas être null ou vide
- **@NotBlank** : Ne doit pas être null, vide ou contenir uniquement des espaces
- **@Size(min, max)** : Taille de la chaîne/collection
- **@Min, @Max** : Valeur numérique minimale/maximale
- **@Email** : Format email valide
- **@Pattern** : Correspond à une regex
- **@Past, @Future** : Date dans le passé/futur

---

## Gestion des Exceptions

### 60. Comment gérer les exceptions globalement dans Spring Boot ?

```java
@RestControllerAdvice
public class GlobalExceptionHandler {
    
    @ExceptionHandler(ResourceNotFoundException.class)
    public ResponseEntity<ErrorResponse> handleResourceNotFound(
            ResourceNotFoundException ex) {
        ErrorResponse error = new ErrorResponse(
            HttpStatus.NOT_FOUND.value(),
            ex.getMessage(),
            System.currentTimeMillis()
        );
        return new ResponseEntity<>(error, HttpStatus.NOT_FOUND);
    }
    
    @ExceptionHandler(MethodArgumentNotValidException.class)
    public ResponseEntity<Map<String, String>> handleValidationErrors(
            MethodArgumentNotValidException ex) {
        Map<String, String> errors = new HashMap<>();
        ex.getBindingResult().getFieldErrors().forEach(error ->
            errors.put(error.getField(), error.getDefaultMessage())
        );
        return new ResponseEntity<>(errors, HttpStatus.BAD_REQUEST);
    }
    
    @ExceptionHandler(Exception.class)
    public ResponseEntity<ErrorResponse> handleGlobalException(Exception ex) {
        ErrorResponse error = new ErrorResponse(
            HttpStatus.INTERNAL_SERVER_ERROR.value(),
            "Une erreur est survenue",
            System.currentTimeMillis()
        );
        return new ResponseEntity<>(error, HttpStatus.INTERNAL_SERVER_ERROR);
    }
}

// Classe d'erreur personnalisée
public class ErrorResponse {
    private int status;
    private String message;
    private long timestamp;
    
    // Constructeur, getters, setters
}

// Exception personnalisée
public class ResourceNotFoundException extends RuntimeException {
    public ResourceNotFoundException(String message) {
        super(message);
    }
}
```

---

## Tests dans Spring Boot

### 61. Comment tester une application Spring Boot ?

```java
// Test d'intégration
@SpringBootTest
@AutoConfigureMockMvc
public class UserControllerIntegrationTest {
    
    @Autowired
    private MockMvc mockMvc;
    
    @Autowired
    private UserRepository userRepository;
    
    @Test
    public void testGetUser() throws Exception {
        User user = new User("john", "john@example.com");
        userRepository.save(user);
        
        mockMvc.perform(get("/api/users/" + user.getId()))
            .andExpect(status().isOk())
            .andExpect(jsonPath("$.username").value("john"));
    }
}

// Test unitaire du service
@ExtendWith(MockitoExtension.class)
public class UserServiceTest {
    
    @Mock
    private UserRepository userRepository;
    
    @InjectMocks
    private UserService userService;
    
    @Test
    public void testFindById() {
        User user = new User(1L, "john", "john@example.com");
        when(userRepository.findById(1L)).thenReturn(Optional.of(user));
        
        User found = userService.findById(1L);
        
        assertNotNull(found);
        assertEquals("john", found.getUsername());
        verify(userRepository, times(1)).findById(1L);
    }
}

// Test du repository
@DataJpaTest
public class UserRepositoryTest {
    @Autowired
    private UserRepository userRepository;
    
    @Autowired
    private TestEntityManager entityManager;
    
    @Test
    public void testFindByEmail() {
        User user = new User("john", "john@example.com");
        entityManager.persist(user);
        entityManager.flush();
        
        User found = userRepository.findByEmail("john@example.com");
        
        assertNotNull(found);
        assertEquals(user.getUsername(), found.getUsername());
    }
}

// Test REST avec TestRestTemplate
@SpringBootTest(webEnvironment = SpringBootTest.WebEnvironment.RANDOM_PORT)
public class UserRestTemplateTest {
    @Autowired
    private TestRestTemplate restTemplate;
    
    @Test
    public void testCreateUser() {
        User user = new User("john", "john@example.com");
        
        ResponseEntity<User> response = restTemplate.postForEntity(
            "/api/users", user, User.class);
        
        assertEquals(HttpStatus.CREATED, response.getStatusCode());
        assertNotNull(response.getBody().getId());
    }
}
```

---

## Configuration et Profils

### 62. Comment utiliser plusieurs profils dans Spring Boot ?

```properties
# application.properties (commun)
app.name=Mon Application

# application-dev.properties (développement)
spring.datasource.url=jdbc:h2:mem:testdb
spring.jpa.show-sql=true
logging.level.root=DEBUG

# application-prod.properties (production)
spring.datasource.url=jdbc:mysql://prod-server:3306/proddb
spring.jpa.show-sql=false
logging.level.root=WARN
```

```java
// Activer un profil
@Configuration
@Profile("dev")
public class DevConfiguration {
    @Bean
    public DataSource dataSource() {
        return new H2DataSource();
    }
}

@Configuration
@Profile("prod")
public class ProdConfiguration {
    @Bean
    public DataSource dataSource() {
        return new MySQLDataSource();
    }
}

// Dans le code
@Service
public class EmailService {
    
    @Value("${spring.profiles.active}")
    private String activeProfile;
    
    public void sendEmail() {
        if ("prod".equals(activeProfile)) {
            // Envoyer un vrai email
        } else {
            // Logger l'email
        }
    }
}
```

**Activer un profil :**

```bash
# Via ligne de commande
java -jar app.jar --spring.profiles.active=prod

# Via variable d'environnement
export SPRING_PROFILES_ACTIVE=prod

# Dans application.properties
spring.profiles.active=dev
```

---

## REST API et Documentation

### 63. Comment documenter une API REST avec Swagger/OpenAPI ?

```xml
<!-- Dépendance Springdoc OpenAPI -->
<dependency>
    <groupId>org.springdoc</groupId>
    <artifactId>springdoc-openapi-starter-webmvc-ui</artifactId>
    <version>2.0.0</version>
</dependency>
```

```java
// Configuration OpenAPI
@Configuration
public class OpenApiConfig {
    
    @Bean
    public OpenAPI customOpenAPI() {
        return new OpenAPI()
            .info(new Info()
                .title("Mon API REST")
                .version("1.0")
                .description("Documentation de l'API")
                .contact(new Contact()
                    .name("Support")
                    .email("support@example.com")));
    }
}

// Documentation du controller
@RestController
@RequestMapping("/api/users")
@Tag(name = "Users", description = "API de gestion des utilisateurs")
public class UserController {
    
    @Operation(summary = "Récupérer tous les utilisateurs")
    @ApiResponses(value = {
        @ApiResponse(responseCode = "200", description = "Liste récupérée avec succès"),
        @ApiResponse(responseCode = "500", description = "Erreur serveur")
    })
    @GetMapping
    public List<User> getAllUsers() {
        return userService.findAll();
    }
    
    @Operation(summary = "Créer un nouvel utilisateur")
    @PostMapping
    public ResponseEntity<User> createUser(
            @Parameter(description = "Données de l'utilisateur") 
            @Valid @RequestBody User user) {
        return ResponseEntity.ok(userService.save(user));
    }
}
```

**Accès à la documentation :**

- Swagger UI : `http://localhost:8080/swagger-ui.html`
- JSON API : `http://localhost:8080/v3/api-docs`

---

### 64. Comment implémenter la pagination et le tri ?

```java
@RestController
@RequestMapping("/api/users")
public class UserController {
    
    @GetMapping
    public Page<User> getUsers(
            @RequestParam(defaultValue = "0") int page,
            @RequestParam(defaultValue = "10") int size,
            @RequestParam(defaultValue = "id") String sortBy,
            @RequestParam(defaultValue = "ASC") String direction) {
        
        Sort.Direction sortDirection = Sort.Direction.fromString(direction);
        Pageable pageable = PageRequest.of(page, size, Sort.by(sortDirection, sortBy));
        
        return userService.findAll(pageable);
    }
}

// Service
@Service
public class UserService {
    
    @Autowired
    private UserRepository userRepository;
    
    public Page<User> findAll(Pageable pageable) {
        return userRepository.findAll(pageable);
    }
}

// Repository
public interface UserRepository extends JpaRepository<User, Long> {
    // JpaRepository inclut déjà findAll(Pageable)
    
    // Méthodes personnalisées avec pagination
    Page<User> findByLastName(String lastName, Pageable pageable);
}
```

**Utilisation :** `GET /api/users?page=0&size=20&sortBy=lastName&direction=DESC`

---

## Microservices avec Spring Cloud

### 65. Qu'est-ce que Spring Cloud ?

Spring Cloud est un ensemble d'outils pour construire des architectures de microservices, incluant la découverte de services, la configuration centralisée, les circuit breakers, le routage, etc.

---

### 66. Comment implémenter la découverte de services avec Eureka ?

```xml
<!-- Eureka Server -->
<dependency>
    <groupId>org.springframework.cloud</groupId>
    <artifactId>spring-cloud-starter-netflix-eureka-server</artifactId>
</dependency>
```

```java
// Serveur Eureka
@SpringBootApplication
@EnableEurekaServer
public class EurekaServerApplication {
    public static void main(String[] args) {
        SpringApplication.run(EurekaServerApplication.class, args);
    }
}

// Client Eureka
@SpringBootApplication
@EnableEurekaClient
public class UserServiceApplication {
    public static void main(String[] args) {
        SpringApplication.run(UserServiceApplication.class, args);
    }
}
```

```properties
# Eureka Server (application.properties)
server.port=8761
eureka.client.register-with-eureka=false
eureka.client.fetch-registry=false

# Eureka Client
spring.application.name=user-service
eureka.client.service-url.defaultZone=http://localhost:8761/eureka/
```

---

### 67. Comment implémenter un API Gateway ?

```xml
<dependency>
    <groupId>org.springframework.cloud</groupId>
    <artifactId>spring-cloud-starter-gateway</artifactId>
</dependency>
```

```java
@SpringBootApplication
public class ApiGatewayApplication {
    public static void main(String[] args) {
        SpringApplication.run(ApiGatewayApplication.class, args);
    }
}
```

```yaml
# application.yml
spring:
  cloud:
    gateway:
      routes:
        - id: user-service
          uri: lb://USER-SERVICE
          predicates:
            - Path=/api/users/**
          filters:
            - RewritePath=/api/users/(?<segment>.*), /${segment}
        
        - id: order-service
          uri: lb://ORDER-SERVICE
          predicates:
            - Path=/api/orders/**
```

---

### 68. Qu'est-ce qu'un Circuit Breaker avec Resilience4j ?

```xml
<dependency>
    <groupId>org.springframework.cloud</groupId>
    <artifactId>spring-cloud-starter-circuitbreaker-resilience4j</artifactId>
</dependency>
```

```java
@Service
public class UserService {
    
    @Autowired
    private RestTemplate restTemplate;
    
    @CircuitBreaker(name = "userService", fallbackMethod = "getUserFallback")
    public User getUser(Long id) {
        return restTemplate.getForObject(
            "http://USER-SERVICE/users/" + id, User.class);
    }
    
    // Méthode de fallback en cas d'échec
    public User getUserFallback(Long id, Exception ex) {
        return new User(id, "Default User", "default@example.com");
    }
}
```

```yaml
# Configuration Resilience4j
resilience4j:
  circuitbreaker:
    instances:
      userService:
        sliding-window-size: 10
        failure-rate-threshold: 50
        wait-duration-in-open-state: 10000
        permitted-number-of-calls-in-half-open-state: 3
```

---

### 69. Comment centraliser la configuration avec Config Server ?

```xml
<!-- Config Server -->
<dependency>
    <groupId>org.springframework.cloud</groupId>
    <artifactId>spring-cloud-config-server</artifactId>
</dependency>
```

```java
@SpringBootApplication
@EnableConfigServer
public class ConfigServerApplication {
    public static void main(String[] args) {
        SpringApplication.run(ConfigServerApplication.class, args);
    }
}
```

```properties
# Config Server
server.port=8888
spring.cloud.config.server.git.uri=https://github.com/votre-repo/config-repo

# Config Client
spring.application.name=user-service
spring.cloud.config.uri=http://localhost:8888
```

---

## Sécurité et JWT

### 70. Comment implémenter l'authentification JWT ?

```xml
<dependency>
    <groupId>io.jsonwebtoken</groupId>
    <artifactId>jjwt-api</artifactId>
    <version>0.11.5</version>
</dependency>
<dependency>
    <groupId>io.jsonwebtoken</groupId>
    <artifactId>jjwt-impl</artifactId>
    <version>0.11.5</version>
    <scope>runtime</scope>
</dependency>
```

```java
// Service JWT
@Service
public class JwtService {
    
    @Value("${jwt.secret}")
    private String secret;
    
    @Value("${jwt.expiration}")
    private Long expiration;
    
    public String generateToken(UserDetails userDetails) {
        Map<String, Object> claims = new HashMap<>();
        return createToken(claims, userDetails.getUsername());
    }
    
    private String createToken(Map<String, Object> claims, String subject) {
        return Jwts.builder()
            .setClaims(claims)
            .setSubject(subject)
            .setIssuedAt(new Date(System.currentTimeMillis()))
            .setExpiration(new Date(System.currentTimeMillis() + expiration))
            .signWith(getSigningKey(), SignatureAlgorithm.HS256)
            .compact();
    }
    
    public Boolean validateToken(String token, UserDetails userDetails) {
        final String username = extractUsername(token);
        return (username.equals(userDetails.getUsername()) && !isTokenExpired(token));
    }
    
    public String extractUsername(String token) {
        return extractClaim(token, Claims::getSubject);
    }
    
    private Boolean isTokenExpired(String token) {
        return extractExpiration(token).before(new Date());
    }
    
    private Date extractExpiration(String token) {
        return extractClaim(token, Claims::getExpiration);
    }
    
    public <T> T extractClaim(String token, Function<Claims, T> claimsResolver) {
        final Claims claims = extractAllClaims(token);
        return claimsResolver.apply(claims);
    }
    
    private Claims extractAllClaims(String token) {
        return Jwts.parserBuilder()
            .setSigningKey(getSigningKey())
            .build()
            .parseClaimsJws(token)
            .getBody();
    }
    
    private Key getSigningKey() {
        byte[] keyBytes = Decoders.BASE64.decode(secret);
        return Keys.hmacShaKeyFor(keyBytes);
    }
}

// Filtre JWT
@Component
public class JwtAuthenticationFilter extends OncePerRequestFilter {
    
    @Autowired
    private JwtService jwtService;
    
    @Autowired
    private UserDetailsService userDetailsService;
    
    @Override
    protected void doFilterInternal(
            HttpServletRequest request,
            HttpServletResponse response,
            FilterChain filterChain) throws ServletException, IOException {
        
        final String authHeader = request.getHeader("Authorization");
        final String jwt;
        final String username;
        
        if (authHeader == null || !authHeader.startsWith("Bearer ")) {
            filterChain.doFilter(request, response);
            return;
        }
        
        jwt = authHeader.substring(7);
        username = jwtService.extractUsername(jwt);
        
        if (username != null && SecurityContextHolder.getContext().getAuthentication() == null) {
            UserDetails userDetails = userDetailsService.loadUserByUsername(username);
            
            if (jwtService.validateToken(jwt, userDetails)) {
                UsernamePasswordAuthenticationToken authToken = 
                    new UsernamePasswordAuthenticationToken(
                        userDetails, null, userDetails.getAuthorities());
                
                authToken.setDetails(new WebAuthenticationDetailsSource()
                    .buildDetails(request));
                
                SecurityContextHolder.getContext().setAuthentication(authToken);
            }
        }
        
        filterChain.doFilter(request, response);
    }
}

// Configuration Security avec JWT
@Configuration
@EnableWebSecurity
public class SecurityConfig {
    
    @Autowired
    private JwtAuthenticationFilter jwtAuthFilter;
    
    @Bean
    public SecurityFilterChain securityFilterChain(HttpSecurity http) throws Exception {
        http
            .csrf(csrf -> csrf.disable())
            .authorizeHttpRequests(auth -> auth
                .requestMatchers("/api/auth/**").permitAll()
                .anyRequest().authenticated()
            )
            .sessionManagement(session -> session
                .sessionCreationPolicy(SessionCreationPolicy.STATELESS)
            )
            .addFilterBefore(jwtAuthFilter, UsernamePasswordAuthenticationFilter.class);
        
        return http.build();
    }
}

// Controller d'authentification
@RestController
@RequestMapping("/api/auth")
public class AuthController {
    
    @Autowired
    private AuthenticationManager authenticationManager;
    
    @Autowired
    private JwtService jwtService;
    
    @Autowired
    private UserDetailsService userDetailsService;
    
    @PostMapping("/login")
    public ResponseEntity<AuthResponse> login(@RequestBody AuthRequest request) {
        authenticationManager.authenticate(
            new UsernamePasswordAuthenticationToken(
                request.getUsername(), request.getPassword())
        );
        
        UserDetails user = userDetailsService.loadUserByUsername(request.getUsername());
        String token = jwtService.generateToken(user);
        
        return ResponseEntity.ok(new AuthResponse(token));
    }
}
```

---

## Caching

### 71. Comment implémenter le cache dans Spring Boot ?

```xml
<dependency>
    <groupId>org.springframework.boot</groupId>
    <artifactId>spring-boot-starter-cache</artifactId>
</dependency>
```

```java
// Activer le cache
@SpringBootApplication
@EnableCaching
public class Application {
    public static void main(String[] args) {
        SpringApplication.run(Application.class, args);
    }
}

// Utiliser le cache dans un service
@Service
public class UserService {
    
    @Cacheable(value = "users", key = "#id")
    public User findById(Long id) {
        // Cette méthode ne sera appelée que si l'utilisateur n'est pas en cache
        System.out.println("Récupération depuis la base de données");
        return userRepository.findById(id).orElse(null);
    }
    
    @CachePut(value = "users", key = "#user.id")
    public User update(User user) {
        // Met à jour le cache
        return userRepository.save(user);
    }
    
    @CacheEvict(value = "users", key = "#id")
    public void delete(Long id) {
        // Supprime l'entrée du cache
        userRepository.deleteById(id);
    }
    
    @CacheEvict(value = "users", allEntries = true)
    public void clearCache() {
        // Vide tout le cache
    }
}
```

**Avec Redis :**

```xml
<dependency>
    <groupId>org.springframework.boot</groupId>
    <artifactId>spring-boot-starter-data-redis</artifactId>
</dependency>
```

```properties
spring.cache.type=redis
spring.redis.host=localhost
spring.redis.port=6379
```

---

## Messaging avec RabbitMQ/Kafka

### 72. Comment utiliser RabbitMQ dans Spring Boot ?

```xml
<dependency>
    <groupId>org.springframework.boot</groupId>
    <artifactId>spring-boot-starter-amqp</artifactId>
</dependency>
```

```java
// Configuration RabbitMQ
@Configuration
public class RabbitMQConfig {
    
    @Bean
    public Queue userQueue() {
        return new Queue("user.queue", false);
    }
    
    @Bean
    public DirectExchange exchange() {
        return new DirectExchange("user.exchange");
    }
    
    @Bean
    public Binding binding(Queue queue, DirectExchange exchange) {
        return BindingBuilder.bind(queue).to(exchange).with("user.routing.key");
    }
}

// Producer
@Service
public class MessageProducer {
    
    @Autowired
    private RabbitTemplate rabbitTemplate;
    
    public void sendMessage(String message) {
        rabbitTemplate.convertAndSend(
            "user.exchange", 
            "user.routing.key", 
            message
        );
        System.out.println("Message envoyé: " + message);
    }
}

// Consumer
@Component
public class MessageConsumer {
    
    @RabbitListener(queues = "user.queue")
    public void receiveMessage(String message) {
        System.out.println("Message reçu: " + message);
        // Traiter le message
    }
}
```

---

### 73. Comment utiliser Kafka dans Spring Boot ?

```xml
<dependency>
    <groupId>org.springframework.kafka</groupId>
    <artifactId>spring-kafka</artifactId>
</dependency>
```

```java
// Producer
@Service
public class KafkaProducer {
    
    @Autowired
    private KafkaTemplate<String, String> kafkaTemplate;
    
    public void sendMessage(String topic, String message) {
        kafkaTemplate.send(topic, message);
    }
}

// Consumer
@Component
public class KafkaConsumer {
    
    @KafkaListener(topics = "user-topic", groupId = "user-group")
    public void consume(String message) {
        System.out.println("Message consommé: " + message);
    }
}
```

```properties
# Kafka configuration
spring.kafka.bootstrap-servers=localhost:9092
spring.kafka.consumer.group-id=user-group
spring.kafka.consumer.auto-offset-reset=earliest
```

---

## Logging

### 74. Comment configurer les logs dans Spring Boot ?

```properties
# application.properties
logging.level.root=INFO
logging.level.com.example=DEBUG
logging.level.org.springframework.web=DEBUG
logging.level.org.hibernate.SQL=DEBUG

# Fichier de log
logging.file.name=logs/application.log
logging.file.max-size=10MB
logging.file.max-history=30

# Pattern
logging.pattern.console=%d{yyyy-MM-dd HH:mm:ss} - %msg%n
```

```java
// Utilisation dans le code
@Service
public class UserService {
    
    private static final Logger logger = LoggerFactory.getLogger(UserService.class);
    
    public User createUser(User user) {
        logger.debug("Création de l'utilisateur: {}", user.getUsername());
        
        try {
            User savedUser = userRepository.save(user);
            logger.info("Utilisateur créé avec succès: ID={}", savedUser.getId());
            return savedUser;
        } catch (Exception e) {
            logger.error("Erreur lors de la création de l'utilisateur", e);
            throw e;
        }
    }
}

// Avec Lombok
@Service
@Slf4j
public class UserService {
    
    public User createUser(User user) {
        log.debug("Création de l'utilisateur: {}", user.getUsername());
        return userRepository.save(user);
    }
}
```

---

## Schedulé et Tâches Asynchrones

### 75. Comment planifier des tâches dans Spring Boot ?

```java
@SpringBootApplication
@EnableScheduling
public class Application {
    public static void main(String[] args) {
        SpringApplication.run(Application.class, args);
    }
}

@Component
public class ScheduledTasks {
    
    private static final Logger logger = LoggerFactory.getLogger(ScheduledTasks.class);
    
    // Exécute toutes les 5 secondes
    @Scheduled(fixedRate = 5000)
    public void taskFixedRate() {
        logger.info("Tâche à taux fixe - {}", new Date());
    }
    
    // Exécute 5 secondes après la fin de la précédente exécution
    @Scheduled(fixedDelay = 5000)
    public void taskFixedDelay() {
        logger.info("Tâche à délai fixe - {}", new Date());
    }
    
    // Exécute selon une expression cron (tous les jours à 2h du matin)
    @Scheduled(cron = "0 0 2 * * ?")
    public void taskCron() {
        logger.info("Tâche planifiée - {}", new Date());
    }
    
    // Exemples d'expressions cron
    // "0 0 * * * ?"      - Toutes les heures
    // "0 */15 * * * ?"   - Toutes les 15 minutes
    // "0 0 12 * * MON-FRI" - Tous les jours de semaine à midi
}
```

---

### 76. Comment exécuter des tâches asynchrones ?

```java
@SpringBootApplication
@EnableAsync
public class Application {
    public static void main(String[] args) {
        SpringApplication.run(Application.class, args);
    }
}

@Service
public class AsyncService {
    
    @Async
    public CompletableFuture<String> processData(String data) {
        // Traitement long
        try {
            Thread.sleep(3000);
        } catch (InterruptedException e) {
            Thread.currentThread().interrupt();
        }
        
        return CompletableFuture.completedFuture("Traité: " + data);
    }
    
    @Async
    public void sendEmail(String to, String subject) {
        // Envoi d'email asynchrone
        System.out.println("Email envoyé à: " + to);
    }
}

// Configuration personnalisée de l'exécuteur
@Configuration
@EnableAsync
public class AsyncConfig {
    
    @Bean(name = "taskExecutor")
    public Executor taskExecutor() {
        ThreadPoolTaskExecutor executor = new ThreadPoolTaskExecutor();
        executor.setCorePoolSize(2);
        executor.setMaxPoolSize(5);
        executor.setQueueCapacity(100);
        executor.setThreadNamePrefix("async-");
        executor.initialize();
        return executor;
    }
}
```

---

## Conseils pour l'Entretien Spring Boot

1. **Maîtrisez les fondamentaux** : IoC, DI, AOP sont essentiels
2. **Connaissez l'écosystème** : Spring Data, Security, MVC, Cloud
3. **Pratiquez avec des projets réels** : API REST, microservices
4. **Comprenez les annotations** : Sachez quand utiliser chaque annotation
5. **Soyez à l'aise avec JPA/Hibernate** : Relations, requêtes, transactions
6. **Préparez des exemples concrets** de vos projets Spring Boot
7. **Connaissez les design patterns** utilisés par Spring (Singleton, Factory, Proxy, Template Method)
8. **Comprenez les bonnes pratiques** : Architecture en couches, gestion des exceptions, validation
9. **Soyez prêt à coder en direct** : Controllers, Services, Repositories
10. **Restez à jour** sur les dernières versions de Spring Boot

---

### Questions Bonus Fréquentes

**77. Quelle est la différence entre @Component, @Service, @Repository et @Controller ?**

- **@Component** : Annotation générique pour un bean Spring
- **@Service** : Marque la couche de service (logique métier)
- **@Repository** : Marque la couche d'accès aux données (DAO), ajoute la traduction des exceptions
- **@Controller** : Marque un contrôleur MVC
- **@RestController** : Combine @Controller et @ResponseBody

---

**78. Qu'est-ce que @Autowired vs @Resource vs @Inject ?**

- **@Autowired** : Annotation Spring, injection par type
- **@Resource** : Annotation Java EE (JSR-250), injection par nom
- **@Inject** : Annotation Java EE (JSR-330), injection par type

---

**79. Comment gérer les propriétés de configuration ?**

```java
@Component
@ConfigurationProperties(prefix = "app")
public class AppProperties {
    private String name;
    private String version;
    // Getters et setters
}

// Utilisation
@Service
public class MyService {
    @Value("${app.name}")
    private String appName;
    
    @Autowired
    private AppProperties appProperties;
}
```

---

**80. Qu'est-ce que CommandLineRunner et ApplicationRunner ?**

Interfaces pour exécuter du code au démarrage de l'application.

```java
@Component
public class DataInitializer implements CommandLineRunner {
    
    @Override
    public void run(String... args) throws Exception {
        System.out.println("Application démarrée !");
        // Initialisation de données
    }
}
```

---

## Questions de Base JavaScript

### 1. Qu'est-ce que JavaScript ?

JavaScript est un langage de programmation interprété, principalement utilisé pour le développement web. Contrairement à Java, il est dynamiquement typé et s'exécute dans le navigateur ou sur un serveur avec Node.js.

---

### 2. Quelle est la différence entre var, let et const ?

- **var** : Portée de fonction (function-scoped), hoistée et initialisée avec `undefined`, peut être redéclarée
- **let** : Portée de bloc (block-scoped), hoistée mais non initialisée (temporal dead zone), ne peut pas être redéclarée dans le même scope mais peut être mise à jour
- **const** : Portée de bloc, doit être initialisée à la déclaration, la référence ne peut pas être réassignée (mais les objets peuvent être modifiés)

**Exemple :**

```javascript
// var
function example() {
  if (true) {
    var x = 1;
  }
  console.log(x); // 1 (accessible en dehors du bloc)
}

// let
function example() {
  if (true) {
    let y = 1;
  }
  console.log(y); // ReferenceError (non accessible)
}

// const
const z = 1;
z = 2; // TypeError: Assignment to constant variable

const obj = { a: 1 };
obj.a = 2; // OK, on modifie la propriété, pas la référence
obj = {}; // TypeError
```

---

### 3. Qu'est-ce que le hoisting ?

Le hoisting est le comportement de JavaScript où les déclarations de variables et de fonctions sont déplacées en haut de leur portée avant l'exécution. Les déclarations avec `var` sont hoistées et initialisées avec `undefined`, tandis que `let` et `const` sont hoistées mais non initialisées.

```javascript
console.log(x); // undefined (pas d'erreur)
var x = 5;

console.log(y); // ReferenceError
let y = 10;

// Fonctions
sayHello(); // "Hello" (fonction hoistée)

function sayHello() {
  console.log("Hello");
}
```

---

### 4. Quelle est la différence entre == et === ?

- **==** : Égalité faible (loose equality), effectue une conversion de type si nécessaire
- **===** : Égalité stricte (strict equality), pas de conversion de type, vérifie le type ET la valeur

```javascript
5 == "5"  // true (conversion de type)
5 === "5" // false (types différents)

null == undefined  // true
null === undefined // false

0 == false  // true
0 === false // false
```

**Recommandation :** Utilisez toujours `===` pour éviter les surprises liées à la coercition de type.

---

### 5. Qu'est-ce que null et undefined ?

- **undefined** : Une variable déclarée mais pas initialisée, ou une propriété inexistante
- **null** : Une valeur d'assignation qui représente intentionnellement "aucune valeur"

```javascript
let x;
console.log(x); // undefined

let y = null;
console.log(y); // null

let obj = {};
console.log(obj.prop); // undefined (propriété n'existe pas)

// Vérification
typeof undefined; // "undefined"
typeof null;      // "object" (bug historique de JavaScript)

x === undefined; // true
y === null;      // true
```

---

## Questions Intermédiaires JavaScript

### 6. Qu'est-ce qu'une closure (fermeture) ?

Une closure est une fonction qui a accès à sa portée externe, même après que la fonction externe ait terminé son exécution. C'est utile pour l'encapsulation de données et la création de variables privées.

```javascript
function outerFunction() {
  let count = 0;
  
  function innerFunction() {
    count++;
    console.log(count);
  }
  
  return innerFunction;
}

const counter = outerFunction();
counter(); // 1
counter(); // 2
counter(); // 3

// Exemple pratique : Module pattern
const calculator = (function() {
  let result = 0;
  
  return {
    add: function(x) {
      result += x;
      return this;
    },
    multiply: function(x) {
      result *= x;
      return this;
    },
    getResult: function() {
      return result;
    }
  };
})();

calculator.add(5).multiply(2);
console.log(calculator.getResult()); // 10
```

---

### 7. Expliquez l'Event Loop

L'Event Loop gère les opérations asynchrones en vérifiant continuellement si la pile d'appels (call stack) est vide, puis traite les événements en attente dans la file de messages. Il permet à JavaScript d'effectuer des opérations non bloquantes.

```javascript
console.log("Start");

setTimeout(() => console.log("Async task"), 0);

console.log("End");

// Sortie: Start, End, Async task
// Même avec 0ms, setTimeout s'exécute après à cause de l'Event Loop
```

**Comment ça fonctionne :**

1. Le code synchrone s'exécute d'abord
2. Les fonctions asynchrones (setTimeout, Promises, etc.) sont placées dans la file d'attente
3. Une fois la pile d'appels vide, l'Event Loop prend le premier élément de la file
4. Le processus se répète

```javascript
console.log("1");

setTimeout(() => console.log("2"), 0);

Promise.resolve().then(() => console.log("3"));

console.log("4");

// Sortie: 1, 4, 3, 2
// Les Promises (microtasks) ont priorité sur les callbacks (macrotasks)
```

---

### 8. Qu'est-ce qu'une Promise ?

Une Promise est un objet représentant la complétion ou l'échec éventuel d'une opération asynchrone. Elle a trois états : **pending** (en attente), **fulfilled** (résolue), **rejected** (rejetée).

```javascript
const promise = new Promise((resolve, reject) => {
  setTimeout(() => {
    const success = true;
    if (success) {
      resolve("Succès !");
    } else {
      reject("Erreur !");
    }
  }, 1000);
});

promise
  .then(result => console.log(result))
  .catch(error => console.error(error))
  .finally(() => console.log("Terminé"));

// Promise.all - attendre toutes les promises
const promise1 = Promise.resolve(1);
const promise2 = Promise.resolve(2);
const promise3 = Promise.resolve(3);

Promise.all([promise1, promise2, promise3])
  .then(values => console.log(values)); // [1, 2, 3]

// Promise.race - la première qui se résout
Promise.race([promise1, promise2, promise3])
  .then(value => console.log(value)); // 1
```

---

### 9. Qu'est-ce que async/await ?

`async/await` est du sucre syntaxique construit sur les Promises, rendant le code asynchrone plus lisible et similaire au code synchrone.

```javascript
// Avec Promises
function fetchData() {
  return fetch('https://api.example.com/data')
    .then(response => response.json())
    .then(data => {
      console.log(data);
      return data;
    })
    .catch(error => {
      console.error('Erreur:', error);
    });
}

// Avec async/await
async function fetchData() {
  try {
    const response = await fetch('https://api.example.com/data');
    const data = await response.json();
    console.log(data);
    return data;
  } catch (error) {
    console.error('Erreur:', error);
  }
}

// Fonction async retourne toujours une Promise
async function getData() {
  return "Données";
}

getData().then(data => console.log(data)); // "Données"
```

---

### 10. Qu'est-ce que le mot-clé this ?

`this` fait référence à l'objet qui exécute la fonction actuelle. Sa valeur dépend du contexte d'appel : dans un objet, dans un callback, ou comme constructeur.

```javascript
// Dans un objet
const person = {
  name: "John",
  greet: function() {
    console.log(`Hello, I'm ${this.name}`);
  }
};
person.greet(); // "Hello, I'm John"

// Problème avec les callbacks
const person2 = {
  name: "John",
  greet: function() {
    setTimeout(function() {
      console.log(`Hello, I'm ${this.name}`); // "Hello, I'm undefined"
    }, 100);
  }
};

// Solution 1 : Arrow function
const person3 = {
  name: "John",
  greet: function() {
    setTimeout(() => {
      console.log(`Hello, I'm ${this.name}`); // "Hello, I'm John"
    }, 100);
  }
};

// Solution 2 : bind
const person4 = {
  name: "John",
  greet: function() {
    setTimeout(function() {
      console.log(`Hello, I'm ${this.name}`);
    }.bind(this), 100);
  }
};

// Dans un constructeur
function Person(name) {
  this.name = name;
}
const john = new Person("John");
console.log(john.name); // "John"
```

---

### 11. Qu'est-ce que l'event bubbling et l'event capturing ?

- **Event bubbling** : L'événement se propage de l'élément cible vers ses parents
- **Event capturing** : L'événement se propage du parent vers l'élément cible

```html
<div id="parent">
  <button id="child">Cliquez-moi</button>
</div>
```

```javascript
// Bubbling (par défaut)
document.getElementById('parent').addEventListener('click', () => {
  console.log('Parent cliqué');
});

document.getElementById('child').addEventListener('click', () => {
  console.log('Enfant cliqué');
});

// Clic sur le bouton : "Enfant cliqué", puis "Parent cliqué"

// Capturing
document.getElementById('parent').addEventListener('click', () => {
  console.log('Parent cliqué');
}, true); // true = capturing phase

document.getElementById('child').addEventListener('click', () => {
  console.log('Enfant cliqué');
});

// Clic sur le bouton : "Parent cliqué", puis "Enfant cliqué"

// Arrêter la propagation
document.getElementById('child').addEventListener('click', (e) => {
  e.stopPropagation(); // Empêche la propagation
  console.log('Enfant cliqué');
});
```

---

## Questions Avancées JavaScript

### 12. Qu'est-ce que la délégation d'événements (event delegation) ?

Technique qui consiste à attacher un seul gestionnaire d'événements sur un élément parent plutôt que sur chaque élément enfant. Utile pour les performances et les éléments ajoutés dynamiquement.

```javascript
// ❌ Mauvaise approche
const items = document.querySelectorAll('.item');
items.forEach(item => {
  item.addEventListener('click', handleClick);
});

// ✅ Bonne approche - Event delegation
const list = document.getElementById('list');
list.addEventListener('click', (e) => {
  if (e.target.classList.contains('item')) {
    handleClick(e);
  }
});

// Fonctionne même pour les éléments ajoutés dynamiquement
function addNewItem() {
  const newItem = document.createElement('li');
  newItem.className = 'item';
  newItem.textContent = 'Nouvel élément';
  list.appendChild(newItem);
  // Pas besoin d'ajouter un event listener, ça fonctionne automatiquement !
}
```

---

### 13. Différence entre fonction déclarée et expression de fonction

```javascript
// Déclaration de fonction (hoistée)
function greet() {
  return "Hello";
}

// Peut être appelée avant sa déclaration
sayHello(); // "Hello"

function sayHello() {
  console.log("Hello");
}

// Expression de fonction (non hoistée)
const greet2 = function() {
  return "Hello";
};

// Ne peut pas être appelée avant
sayHello2(); // ReferenceError

const sayHello2 = function() {
  console.log("Hello");
};

// Expression de fonction nommée
const greet3 = function namedFunction() {
  return "Hello";
};
```

---

### 14. Qu'est-ce que les arrow functions (fonctions flèches) ?

Les fonctions flèches offrent une syntaxe plus concise et ne créent pas leur propre contexte `this`, elles héritent du `this` de leur portée englobante.

```javascript
// Fonction traditionnelle
const add = function(a, b) {
  return a + b;
};

// Arrow function
const add = (a, b) => a + b;

// Si un seul paramètre, parenthèses optionnelles
const square = x => x * x;

// Si pas de paramètres
const greet = () => "Hello";

// Si plusieurs lignes, accolades nécessaires
const multiply = (a, b) => {
  const result = a * b;
  return result;
};

// Retour d'objet littéral
const createPerson = (name, age) => ({ name, age });

// Différence avec this
const obj = {
  name: "John",
  regularFunction: function() {
    console.log(this.name); // "John"
  },
  arrowFunction: () => {
    console.log(this.name); // undefined (this = window/global)
  }
};
```

---

### 15. Qu'est-ce que la Temporal Dead Zone (TDZ) ?

La période entre la création d'une liaison de variable `let` ou `const` et son initialisation. Accéder à la variable pendant cette période provoque une `ReferenceError`.

```javascript
// TDZ pour let
console.log(x); // ReferenceError: Cannot access 'x' before initialization
let x = 5;

// TDZ pour const
console.log(y); // ReferenceError
const y = 10;

// Pas de TDZ pour var (mais undefined)
console.log(z); // undefined
var z = 15;

// Exemple plus complexe
function example() {
  console.log(a); // ReferenceError
  let a = 1;
}
```

---

### 16. Qu'est-ce que le currying ?

Technique de transformation d'une fonction avec plusieurs arguments en une séquence de fonctions prenant chacune un seul argument.

```javascript
// Fonction normale
const multiply = (a, b, c) => a * b * c;
console.log(multiply(2, 3, 4)); // 24

// Fonction curryfiée
const multiplyCurried = (a) => (b) => (c) => a * b * c;
console.log(multiplyCurried(2)(3)(4)); // 24

// Utilisation partielle
const multiplyBy2 = multiplyCurried(2);
const multiplyBy2And3 = multiplyBy2(3);
console.log(multiplyBy2And3(4)); // 24

// Fonction de curry générique
function curry(fn) {
  return function curried(...args) {
    if (args.length >= fn.length) {
      return fn.apply(this, args);
    } else {
      return function(...args2) {
        return curried.apply(this, args.concat(args2));
      };
    }
  };
}

const curriedMultiply = curry(multiply);
console.log(curriedMultiply(2)(3)(4)); // 24
```

---

### 17. Différence entre shallow copy et deep copy

- **Shallow copy** : Copie seulement le premier niveau de l'objet
- **Deep copy** : Copie récursive de tous les niveaux

```javascript
const original = { 
  a: 1, 
  b: { 
    c: 2 
  } 
};

// Shallow copy
const shallowCopy = { ...original };
// ou
const shallowCopy2 = Object.assign({}, original);

shallowCopy.b.c = 99;
console.log(original.b.c); // 99 (modifié aussi !)

// Deep copy - Méthode 1: JSON (limitations)
const deepCopy1 = JSON.parse(JSON.stringify(original));
deepCopy1.b.c = 99;
console.log(original.b.c); // 2 (non modifié)

// Limitation: ne fonctionne pas avec fonctions, undefined, Symbol, etc.
const obj = { a: 1, fn: () => {}, undef: undefined };
const copy = JSON.parse(JSON.stringify(obj));
console.log(copy); // { a: 1 } (fn et undef perdus)

// Deep copy - Méthode 2: Structured Clone (moderne)
const deepCopy2 = structuredClone(original);

// Deep copy - Méthode 3: Fonction récursive
function deepCopy(obj) {
  if (obj === null || typeof obj !== 'object') {
    return obj;
  }
  
  if (obj instanceof Date) {
    return new Date(obj.getTime());
  }
  
  if (obj instanceof Array) {
    return obj.map(item => deepCopy(item));
  }
  
  const copy = {};
  for (let key in obj) {
    if (obj.hasOwnProperty(key)) {
      copy[key] = deepCopy(obj[key]);
    }
  }
  return copy;
}
```

---

### 18. Qu'est-ce qu'une IIFE ?

**IIFE** (Immediately Invoked Function Expression) - une fonction qui s'exécute immédiatement après sa définition, utile pour créer une portée privée.

```javascript
// Syntaxe basique
(function() {
  const privateVar = "privée";
  console.log(privateVar);
})();

// Avec paramètres
(function(name) {
  console.log(`Hello, ${name}`);
})("John");

// Avec arrow function
(() => {
  console.log("IIFE avec arrow function");
})();

// Module pattern avec IIFE
const myModule = (function() {
  let privateVar = 0;
  
  return {
    increment: function() {
      privateVar++;
    },
    getValue: function() {
      return privateVar;
    }
  };
})();

myModule.increment();
console.log(myModule.getValue()); // 1
console.log(myModule.privateVar); // undefined (privé)
```

---

### 19. Qu'est-ce qu'une fonction d'ordre supérieur (higher-order function) ?

Une fonction qui prend une ou plusieurs fonctions en paramètres et/ou retourne une fonction.

```javascript
// Fonction qui prend une fonction en paramètre
const numbers = [1, 2, 3, 4];
const doubled = numbers.map(num => num * 2); // map est une higher-order function
console.log(doubled); // [2, 4, 6, 8]

// Fonction qui retourne une fonction
function multiplier(factor) {
  return function(number) {
    return number * factor;
  };
}

const double = multiplier(2);
const triple = multiplier(3);

console.log(double(5)); // 10
console.log(triple(5)); // 15

// Exemples de higher-order functions natives
const numbers2 = [1, 2, 3, 4, 5];

// map - transforme chaque élément
const squared = numbers2.map(n => n * n); // [1, 4, 9, 16, 25]

// filter - filtre les éléments
const evens = numbers2.filter(n => n % 2 === 0); // [2, 4]

// reduce - réduit à une valeur
const sum = numbers2.reduce((acc, n) => acc + n, 0); // 15

// forEach - itère sur chaque élément
numbers2.forEach(n => console.log(n));
```

---

### 20. Qu'est-ce que la coercition de type (type coercion) ?

La conversion automatique de valeurs d'un type de données à un autre. Peut causer des comportements inattendus si on ne fait pas attention.

```javascript
// Coercition implicite
console.log(5 + "5"); // "55" (string)
console.log("5" - 2); // 3 (number)
console.log("5" * 2); // 10 (number)
console.log("5" / 2); // 2.5 (number)

// Coercition avec ==
console.log(5 == "5"); // true
console.log(0 == false); // true
console.log("" == false); // true
console.log(null == undefined); // true

// Coercition avec opérateurs logiques
console.log(0 || "default"); // "default"
console.log("" || "default"); // "default"
console.log(null || "default"); // "default"

// Coercition explicite
const num = "123";
console.log(Number(num)); // 123
console.log(String(123)); // "123"
console.log(Boolean(0)); // false
console.log(Boolean(1)); // true

// Falsy values (coercent vers false)
// false, 0, "", null, undefined, NaN

// Truthy values (coercent vers true)
// Tout le reste, y compris "0", "false", [], {}
```

---

## Questions Fondamentales Angular

### 1. Qu'est-ce qu'Angular ?

Angular est un framework et une plateforme open-source pour créer des applications web côté client en utilisant HTML et TypeScript, développé et maintenu par Google. Il permet de construire des applications web dynamiques à page unique (SPA - Single Page Application) en utilisant une architecture basée sur des composants.

**Caractéristiques principales :**

- Architecture basée sur les composants
- TypeScript comme langage principal
- Injection de dépendances intégrée
- Routing et navigation
- Formulaires réactifs et template-driven
- HTTP client pour les requêtes API
- RxJS pour la programmation réactive

---

### 2. Quelle est la différence entre Angular et AngularJS ?

**AngularJS** (version 1.x) a été le premier framework créé en JavaScript, tandis qu'**Angular** (version 2 et supérieure) a été complètement reconstruit par Google en utilisant TypeScript. Google a cessé la maintenance d'AngularJS en janvier 2022.

**Principales différences :**

| AngularJS (1.x) | Angular (2+) |
|----------------|--------------|
| JavaScript | TypeScript |
| Contrôleurs | Composants |
| $scope | Propriétés de classe |
| Directives complexes | Directives simplifiées |
| Pas de CLI | Angular CLI |
| Pas de lazy loading | Lazy loading intégré |

---

### 3. Qu'est-ce qu'un composant Angular ?

Un composant est la base de l'architecture d'Angular. C'est un élément autonome qui possède sa propre logique, son propre modèle de données et sa propre vue, et peut être réutilisé dans différentes parties de l'application. Un composant est défini par une classe TypeScript décorée avec `@Component`.

```typescript
import { Component } from '@angular/core';

@Component({
  selector: 'app-exemple',
  templateUrl: './exemple.component.html',
  styleUrls: ['./exemple.component.css']
})
export class ExempleComponent {
  titre = 'Mon Composant';
  
  onClick() {
    console.log('Bouton cliqué');
  }
}
```

**Structure d'un composant :**

- **Selector** : Nom de la balise HTML pour utiliser le composant
- **Template** : Vue HTML du composant
- **Styles** : CSS spécifique au composant
- **Classe** : Logique et données du composant

---

### 4. Qu'est-ce qu'un module Angular ?

Un module Angular (NgModule) est un conteneur pour organiser le code de l'application. Chaque application Angular a au moins un module racine (AppModule). Les modules regroupent des composants, des directives, des services et des pipes liés.

```typescript
import { NgModule } from '@angular/core';
import { BrowserModule } from '@angular/platform-browser';
import { HttpClientModule } from '@angular/common/http';

@NgModule({
  declarations: [
    AppComponent, 
    HomeComponent,
    HeaderComponent
  ],
  imports: [
    BrowserModule, 
    HttpClientModule,
    AppRoutingModule
  ],
  providers: [
    MonService,
    DataService
  ],
  bootstrap: [AppComponent]
})
export class AppModule { }
```

**Propriétés d'un NgModule :**

- **declarations** : Composants, directives, pipes de ce module
- **imports** : Autres modules nécessaires
- **providers** : Services disponibles dans ce module
- **bootstrap** : Composant racine de l'application
- **exports** : Éléments à rendre disponibles aux autres modules

---

### 5. Qu'est-ce que le data binding dans Angular ?

Le data binding est la synchronisation automatique des données entre le modèle et les composants de la vue. Il existe quatre types :

1. **Interpolation** : `{{ variable }}`
2. **Property binding** : `[property]="value"`
3. **Event binding** : `(click)="methode()"`
4. **Two-way binding** : `[(ngModel)]="variable"`

```typescript
// Component
export class DataBindingComponent {
  titre = 'Mon Titre';
  isDisabled = false;
  valeur = '';
  
  onClick() {
    console.log('Cliqué');
  }
  
  onInputChange(event: any) {
    this.valeur = event.target.value;
  }
}
```

```html
<!-- Template -->
<!-- 1. Interpolation -->
<h1>{{ titre }}</h1>

<!-- 2. Property binding -->
<button [disabled]="isDisabled">Cliquez-moi</button>
<img [src]="imageUrl" [alt]="imageAlt">

<!-- 3. Event binding -->
<button (click)="onClick()">Cliquez</button>
<input (input)="onInputChange($event)">

<!-- 4. Two-way binding -->
<input [(ngModel)]="valeur">
<!-- Équivalent à -->
<input [ngModel]="valeur" (ngModelChange)="valeur = $event">
```

---

### 6. Qu'est-ce qu'une directive Angular ?

Une directive introduit une nouvelle syntaxe et est comme un attribut sur un élément DOM qui lui associe un comportement spécifique. Il existe trois types :

1. **Directives de composant** : avec un template
2. **Directives structurelles** : modifient le DOM (`*ngIf`, `*ngFor`, `*ngSwitch`)
3. **Directives d'attribut** : modifient l'apparence ou le comportement (`ngClass`, `ngStyle`)

```html
<!-- Directives structurelles -->
<div *ngIf="isVisible">Contenu visible</div>

<div *ngFor="let item of items; let i = index">
  {{ i + 1 }}. {{ item.name }}
</div>

<div [ngSwitch]="status">
  <p *ngSwitchCase="'active'">Actif</p>
  <p *ngSwitchCase="'inactive'">Inactif</p>
  <p *ngSwitchDefault>Inconnu</p>
</div>

<!-- Directives d'attribut -->
<div [ngClass]="{'active': isActive, 'disabled': isDisabled}">
  Contenu
</div>

<div [ngStyle]="{'color': textColor, 'font-size': fontSize + 'px'}">
  Texte stylisé
</div>
```

**Créer une directive personnalisée :**

```typescript
import { Directive, ElementRef, Renderer2, Input } from '@angular/core';

@Directive({
  selector: '[appHighlight]'
})
export class HighlightDirective {
  @Input() appHighlight: string = 'yellow';
  
  constructor(private el: ElementRef, private renderer: Renderer2) {
    this.renderer.setStyle(this.el.nativeElement, 'background-color', this.appHighlight);
  }
}
```

```html
<p appHighlight="lightblue">Texte surligné</p>
```

---

## Services et Injection de Dépendances Angular

### 7. Qu'est-ce qu'un service Angular ?

Les services sont des objets qui fournissent des fonctionnalités spécifiques à l'application, comme l'accès aux données, les calculs, ou les opérations de logique métier, et peuvent être injectés dans les composants.

```typescript
import { Injectable } from '@angular/core';
import { HttpClient } from '@angular/common/http';
import { Observable } from 'rxjs';

@Injectable({
  providedIn: 'root'
})
export class DataService {
  private apiUrl = 'https://api.example.com';
  
  constructor(private http: HttpClient) { }
  
  getData(): Observable<any> {
    return this.http.get(`${this.apiUrl}/data`);
  }
  
  postData(data: any): Observable<any> {
    return this.http.post(`${this.apiUrl}/data`, data);
  }
  
  calculateTotal(items: number[]): number {
    return items.reduce((sum, item) => sum + item, 0);
  }
}
```

**Utilisation dans un composant :**

```typescript
import { Component, OnInit } from '@angular/core';
import { DataService } from './data.service';

@Component({
  selector: 'app-example',
  template: '<div>{{ data }}</div>'
})
export class ExampleComponent implements OnInit {
  data: any;
  
  constructor(private dataService: DataService) { }
  
  ngOnInit() {
    this.dataService.getData().subscribe(result => {
      this.data = result;
    });
  }
}
```

---

### 8. Qu'est-ce que l'injection de dépendances (DI) ?

L'injection de dépendances est un patron de conception où une classe reçoit ses dépendances depuis des sources externes plutôt que de les instancier directement. Angular possède son propre système DI qui gère la création et l'injection des services.

```typescript
// Service
@Injectable({
  providedIn: 'root'
})
export class MonService {
  getData() {
    return 'Données';
  }
}

// Composant avec injection
@Component({
  selector: 'app-example'
})
export class ExampleComponent {
  // Injection via le constructeur (recommandé)
  constructor(private monService: MonService) { }
  
  // Ou injection via @Inject (pour les tokens personnalisés)
  constructor(@Inject(MonService) private monService: MonService) { }
  
  ngOnInit() {
    const data = this.monService.getData();
  }
}
```

**Avantages de l'injection de dépendances :**

- Découplage du code
- Facilité de test (mock des services)
- Réutilisabilité
- Gestion centralisée des dépendances

---

### 9. Quelle est la différence entre providedIn: 'root' et providers dans @Component ?

- **`providedIn: 'root'`** : Crée un singleton au niveau de l'application (recommandé)
- **`providers` dans `@Component`** : Crée une nouvelle instance pour chaque instance du composant

```typescript
// Service avec providedIn: 'root' (singleton)
@Injectable({
  providedIn: 'root'
})
export class SharedService {
  data = 'Partagé';
}

// Service avec providers dans le composant (nouvelle instance)
@Injectable()
export class LocalService {
  data = 'Local';
}

@Component({
  selector: 'app-parent',
  providers: [LocalService] // Nouvelle instance pour ce composant et ses enfants
})
export class ParentComponent {
  constructor(
    private shared: SharedService,  // Même instance partout
    private local: LocalService     // Instance unique à ce composant
  ) { }
}
```

---

## Cycle de Vie des Composants Angular

### 10. Quels sont les lifecycle hooks principaux d'Angular ?

Les hooks de cycle de vie les plus couramment utilisés incluent `ngOnInit` (appelé une fois que le composant est initialisé), `ngOnChanges` (appelé avant `ngOnInit` et chaque fois qu'une propriété d'entrée change), et `ngDoCheck` (appelé lors de chaque exécution de détection de changement).

**Ordre d'exécution des hooks :**

1. **ngOnChanges** : Appelé quand une propriété `@Input()` change
2. **ngOnInit** : Appelé après l'initialisation (idéal pour la logique d'init)
3. **ngDoCheck** : Détection de changements personnalisée
4. **ngAfterContentInit** : Après l'initialisation du contenu projeté
5. **ngAfterContentChecked** : Après chaque vérification du contenu projeté
6. **ngAfterViewInit** : Après l'initialisation de la vue
7. **ngAfterViewChecked** : Après chaque vérification de la vue
8. **ngOnDestroy** : Avant la destruction (nettoyage, unsubscribe)

```typescript
import { 
  Component, 
  OnInit, 
  OnDestroy, 
  OnChanges, 
  SimpleChanges,
  Input,
  AfterViewInit
} from '@angular/core';

@Component({
  selector: 'app-lifecycle',
  template: '<div>{{ message }}</div>'
})
export class LifecycleComponent implements OnInit, OnChanges, AfterViewInit, OnDestroy {
  @Input() data: string = '';
  message: string = '';
  
  constructor() {
    console.log('1. Constructor');
  }
  
  ngOnChanges(changes: SimpleChanges) {
    console.log('2. ngOnChanges', changes);
    if (changes['data']) {
      this.message = `Données reçues: ${changes['data'].currentValue}`;
    }
  }
  
  ngOnInit() {
    console.log('3. ngOnInit');
    // Logique d'initialisation
    // Appels API, initialisation de variables, etc.
  }
  
  ngAfterViewInit() {
    console.log('4. ngAfterViewInit');
    // Accès aux éléments DOM après initialisation
  }
  
  ngOnDestroy() {
    console.log('5. ngOnDestroy');
    // Nettoyage : unsubscribe, arrêt de timers, etc.
  }
}
```

---

## RxJS et Observables Angular

### 11. Qu'est-ce qu'un Observable ?

Un Observable est un objet qui représente un flux de données asynchrone dans le temps. C'est la base de la programmation réactive avec RxJS dans Angular. Les Observables sont "lazy" et ne s'exécutent que lorsqu'on souscrit avec `.subscribe()`.

```typescript
import { Observable } from 'rxjs';

// Création d'un Observable
const observable = new Observable(observer => {
  observer.next('Valeur 1');
  observer.next('Valeur 2');
  setTimeout(() => {
    observer.next('Valeur 3');
    observer.complete();
  }, 1000);
});

// Souscription
const subscription = observable.subscribe({
  next: (value) => console.log(value),      // Valeur 1, Valeur 2, Valeur 3
  error: (err) => console.error(err),
  complete: () => console.log('Terminé')
});

// N'oubliez pas de se désabonner !
subscription.unsubscribe();
```

**Utilisation avec HttpClient :**

```typescript
import { HttpClient } from '@angular/common/http';
import { Observable } from 'rxjs';

@Injectable({
  providedIn: 'root'
})
export class ApiService {
  constructor(private http: HttpClient) { }
  
  getUsers(): Observable<User[]> {
    return this.http.get<User[]>('/api/users');
  }
}

// Dans le composant
this.apiService.getUsers().subscribe(
  users => console.log(users),
  error => console.error(error)
);
```

---

### 12. Quelle est la différence entre Observable et Promise ?

| Observable | Promise |
|------------|---------|
| Peut émettre plusieurs valeurs | Émet une seule valeur |
| Lazy (ne s'exécute que si on subscribe) | Eager (s'exécute immédiatement) |
| Peut être annulé (unsubscribe) | Ne peut pas être annulée |
| Supporte les opérateurs RxJS (map, filter, etc.) | Pas d'opérateurs |
| Multicast possible | Toujours unicast |

```typescript
// Promise
const promise = new Promise((resolve, reject) => {
  resolve('Valeur unique');
});

promise.then(value => console.log(value));

// Observable
const observable = new Observable(observer => {
  observer.next('Valeur 1');
  observer.next('Valeur 2');
  observer.complete();
});

observable.subscribe(value => console.log(value));
```

---

### 13. Qu'est-ce qu'un Subject en RxJS ?

Un Subject est à la fois un Observable et un Observer. Il peut émettre des valeurs à plusieurs subscribers simultanément (multicasting).

```typescript
import { Subject } from 'rxjs';

const subject = new Subject<number>();

// Plusieurs subscribers
subject.subscribe(value => console.log('Observer A:', value));
subject.subscribe(value => console.log('Observer B:', value));

// Émission de valeurs
subject.next(1); // Les deux observers reçoivent 1
subject.next(2); // Les deux observers reçoivent 2

// Types de Subjects
import { BehaviorSubject, ReplaySubject, AsyncSubject } from 'rxjs';

// BehaviorSubject : garde la dernière valeur
const behaviorSubject = new BehaviorSubject<string>('Valeur initiale');
behaviorSubject.subscribe(value => console.log(value)); // Reçoit immédiatement "Valeur initiale"

// ReplaySubject : garde les N dernières valeurs
const replaySubject = new ReplaySubject<number>(2);
replaySubject.next(1);
replaySubject.next(2);
replaySubject.next(3);
replaySubject.subscribe(value => console.log(value)); // Reçoit 2 et 3

// AsyncSubject : émet seulement la dernière valeur à la complétion
const asyncSubject = new AsyncSubject<number>();
asyncSubject.next(1);
asyncSubject.next(2);
asyncSubject.complete(); // Seule la valeur 2 est émise
```

---

### 14. Quels sont les principaux opérateurs RxJS à connaître ?

**Opérateurs de transformation :**

- **map** : Transforme chaque valeur
- **switchMap** : Projette chaque valeur sur un Observable et annule le précédent
- **mergeMap** : Projette et merge les valeurs
- **concatMap** : Projette et concatène les valeurs

**Opérateurs de filtrage :**

- **filter** : Filtre les valeurs selon une condition
- **take** : Prend les N premières valeurs
- **takeUntil** : Prend les valeurs jusqu'à ce qu'un autre Observable émette
- **debounceTime** : Attend un délai avant d'émettre

**Opérateurs utilitaires :**

- **catchError** : Gestion des erreurs
- **tap** : Effets de bord sans modifier le flux
- **finalize** : Exécute du code à la fin (succès ou erreur)

```typescript
import { of, throwError } from 'rxjs';
import { map, filter, catchError, tap, switchMap } from 'rxjs/operators';

this.http.get('/api/data').pipe(
  tap(response => console.log('Réponse reçue:', response)), // Effet de bord
  map(response => response.data),                           // Transformation
  filter(data => data.length > 0),                          // Filtrage
  switchMap(data => this.processData(data)),                // Nouveau Observable
  catchError(error => {                                     // Gestion d'erreur
    console.error('Erreur:', error);
    return of([]); // Valeur par défaut
  })
).subscribe(data => console.log(data));
```

---

## Routing Angular

### 15. Comment fonctionne le routing dans Angular ?

Les routes permettent de gérer la navigation dans l'application en définissant les différentes pages et les URL associées.

```typescript
import { RouterModule, Routes } from '@angular/router';
import { HomeComponent } from './home/home.component';
import { AboutComponent } from './about/about.component';
import { UserComponent } from './user/user.component';
import { NotFoundComponent } from './not-found/not-found.component';

const routes: Routes = [
  { path: '', component: HomeComponent },
  { path: 'about', component: AboutComponent },
  { path: 'user/:id', component: UserComponent },
  { 
    path: 'admin', 
    loadChildren: () => import('./admin/admin.module').then(m => m.AdminModule)
  },
  { path: '**', component: NotFoundComponent } // Route wildcard (doit être en dernier)
];

@NgModule({
  imports: [RouterModule.forRoot(routes)],
  exports: [RouterModule]
})
export class AppRoutingModule { }
```

**Navigation dans les composants :**

```typescript
import { Router, ActivatedRoute } from '@angular/router';

export class UserComponent implements OnInit {
  userId: string = '';
  
  constructor(
    private route: ActivatedRoute,
    private router: Router
  ) { }
  
  ngOnInit() {
    // Récupérer le paramètre de route
    this.userId = this.route.snapshot.paramMap.get('id') || '';
    
    // Ou s'abonner aux changements de paramètres
    this.route.paramMap.subscribe(params => {
      this.userId = params.get('id') || '';
    });
  }
  
  navigateToAbout() {
    this.router.navigate(['/about']);
  }
  
  navigateToUser(id: string) {
    this.router.navigate(['/user', id]);
  }
}
```

**Template avec router-outlet :**

```html
<nav>
  <a routerLink="/" routerLinkActive="active">Accueil</a>
  <a routerLink="/about" routerLinkActive="active">À propos</a>
  <a [routerLink]="['/user', userId]" routerLinkActive="active">Utilisateur</a>
</nav>

<router-outlet></router-outlet>
```

---

### 16. Qu'est-ce qu'un Route Guard ?

Les Route Guards contrôlent l'accès aux routes. Types principaux :

- **CanActivate** : Peut-on activer cette route ?
- **CanDeactivate** : Peut-on quitter cette route ?
- **CanLoad** : Peut-on charger un module lazy-loaded ?
- **Resolve** : Précharger des données avant d'activer la route

```typescript
import { Injectable } from '@angular/core';
import { CanActivate, Router, ActivatedRouteSnapshot } from '@angular/router';
import { AuthService } from './auth.service';

@Injectable({
  providedIn: 'root'
})
export class AuthGuard implements CanActivate {
  constructor(
    private authService: AuthService,
    private router: Router
  ) { }
  
  canActivate(route: ActivatedRouteSnapshot): boolean {
    if (this.authService.isLoggedIn()) {
      return true;
    } else {
      this.router.navigate(['/login']);
      return false;
    }
  }
}

// Utilisation dans les routes
const routes: Routes = [
  {
    path: 'admin',
    component: AdminComponent,
    canActivate: [AuthGuard]
  }
];
```

**CanDeactivate Guard :**

```typescript
@Injectable({
  providedIn: 'root'
})
export class UnsavedChangesGuard implements CanDeactivate<CanComponentDeactivate> {
  canDeactivate(component: CanComponentDeactivate): boolean {
    if (component.hasUnsavedChanges()) {
      return confirm('Vous avez des modifications non sauvegardées. Voulez-vous vraiment quitter ?');
    }
    return true;
  }
}
```

---

## Formulaires Angular

### 17. Quels sont les deux types de formulaires dans Angular ?

Il existe deux types de formulaires dans Angular : les **formulaires basés sur des modèles (Template-driven forms)** et les **formulaires réactifs (Reactive forms)**.

---

### 18. Quelle est la différence entre Template-driven et Reactive forms ?

| Template-driven | Reactive forms |
|----------------|----------------|
| Logique dans le template | Logique dans le component |
| Plus simple pour les cas basiques | Plus puissant et flexible |
| Utilise `ngModel` | Utilise `FormControl`, `FormGroup` |
| Validation dans le template | Validation dans le component |
| Moins de contrôle | Meilleur contrôle et testabilité |

**Template-driven form :**

```typescript
// Component
export class TemplateFormComponent {
  user = {
    name: '',
    email: ''
  };
  
  onSubmit(form: NgForm) {
    if (form.valid) {
      console.log(this.user);
    }
  }
}
```

```html
<!-- Template -->
<form #userForm="ngForm" (ngSubmit)="onSubmit(userForm)">
  <input 
    name="name" 
    [(ngModel)]="user.name" 
    required 
    #name="ngModel">
  <div *ngIf="name.invalid && name.touched">
    Le nom est requis
  </div>
  
  <input 
    name="email" 
    [(ngModel)]="user.email" 
    required 
    email 
    #email="ngModel">
  <div *ngIf="email.invalid && email.touched">
    Email invalide
  </div>
  
  <button type="submit" [disabled]="userForm.invalid">
    Envoyer
  </button>
</form>
```

**Reactive form :**

```typescript
import { FormGroup, FormControl, Validators, FormBuilder } from '@angular/forms';

export class ReactiveFormComponent {
  form: FormGroup;
  
  constructor(private fb: FormBuilder) {
    // Méthode 1 : FormBuilder (recommandé)
    this.form = this.fb.group({
      name: ['', [Validators.required, Validators.minLength(3)]],
      email: ['', [Validators.required, Validators.email]],
      age: [0, [Validators.required, Validators.min(18)]]
    });
    
    // Méthode 2 : FormGroup/FormControl
    // this.form = new FormGroup({
    //   name: new FormControl('', Validators.required),
    //   email: new FormControl('', [Validators.required, Validators.email])
    // });
  }
  
  onSubmit() {
    if (this.form.valid) {
      console.log(this.form.value);
    } else {
      this.markFormGroupTouched(this.form);
    }
  }
  
  get name() {
    return this.form.get('name');
  }
  
  get email() {
    return this.form.get('email');
  }
  
  private markFormGroupTouched(formGroup: FormGroup) {
    Object.keys(formGroup.controls).forEach(key => {
      const control = formGroup.get(key);
      control?.markAsTouched();
    });
  }
}
```

```html
<!-- Template -->
<form [formGroup]="form" (ngSubmit)="onSubmit()">
  <input formControlName="name">
  <div *ngIf="name?.invalid && name?.touched">
    <div *ngIf="name?.errors?.['required']">Le nom est requis</div>
    <div *ngIf="name?.errors?.['minlength']">
      Minimum 3 caractères
    </div>
  </div>
  
  <input formControlName="email" type="email">
  <div *ngIf="email?.invalid && email?.touched">
    Email invalide
  </div>
  
  <input formControlName="age" type="number">
  
  <button type="submit" [disabled]="form.invalid">
    Envoyer
  </button>
</form>
```

---

## HTTP et Communication Angular

### 19. Comment faire des requêtes HTTP dans Angular ?

Angular utilise `HttpClient` du module `@angular/common/http`.

```typescript
import { Injectable } from '@angular/core';
import { HttpClient, HttpHeaders, HttpParams } from '@angular/common/http';
import { Observable } from 'rxjs';

@Injectable({
  providedIn: 'root'
})
export class ApiService {
  private apiUrl = 'https://api.example.com';
  
  constructor(private http: HttpClient) { }
  
  // GET
  getData(): Observable<any> {
    return this.http.get(`${this.apiUrl}/data`);
  }
  
  // GET avec paramètres
  getUsers(params: any): Observable<User[]> {
    let httpParams = new HttpParams();
    if (params.page) {
      httpParams = httpParams.set('page', params.page);
    }
    if (params.limit) {
      httpParams = httpParams.set('limit', params.limit);
    }
    
    return this.http.get<User[]>(`${this.apiUrl}/users`, { params: httpParams });
  }
  
  // POST
  createUser(user: User): Observable<User> {
    return this.http.post<User>(`${this.apiUrl}/users`, user);
  }
  
  // PUT
  updateUser(id: string, user: User): Observable<User> {
    return this.http.put<User>(`${this.apiUrl}/users/${id}`, user);
  }
  
  // DELETE
  deleteUser(id: string): Observable<void> {
    return this.http.delete<void>(`${this.apiUrl}/users/${id}`);
  }
  
  // Avec headers personnalisés
  getDataWithHeaders(): Observable<any> {
    const headers = new HttpHeaders({
      'Authorization': 'Bearer token',
      'Content-Type': 'application/json'
    });
    
    return this.http.get(`${this.apiUrl}/data`, { headers });
  }
}
```

---

### 20. Qu'est-ce qu'un Interceptor HTTP ?

Un interceptor permet d'intercepter et de modifier les requêtes/réponses HTTP, utile pour ajouter des headers, gérer les erreurs, etc.

```typescript
import { Injectable } from '@angular/core';
import { 
  HttpInterceptor, 
  HttpRequest, 
  HttpHandler, 
  HttpEvent,
  HttpErrorResponse
} from '@angular/common/http';
import { Observable, throwError } from 'rxjs';
import { catchError } from 'rxjs/operators';

@Injectable()
export class AuthInterceptor implements HttpInterceptor {
  intercept(req: HttpRequest<any>, next: HttpHandler): Observable<HttpEvent<any>> {
    // Récupérer le token
    const token = localStorage.getItem('token');
    
    // Cloner la requête et ajouter le header
    if (token) {
      const authReq = req.clone({
        headers: req.headers.set('Authorization', `Bearer ${token}`)
      });
      return next.handle(authReq);
    }
    
    return next.handle(req);
  }
}

// Interceptor pour la gestion d'erreurs
@Injectable()
export class ErrorInterceptor implements HttpInterceptor {
  intercept(req: HttpRequest<any>, next: HttpHandler): Observable<HttpEvent<any>> {
    return next.handle(req).pipe(
      catchError((error: HttpErrorResponse) => {
        if (error.status === 401) {
          // Rediriger vers la page de login
          window.location.href = '/login';
        } else if (error.status === 500) {
          console.error('Erreur serveur:', error);
        }
        return throwError(() => error);
      })
    );
  }
}

// Enregistrer les interceptors
@NgModule({
  providers: [
    {
      provide: HTTP_INTERCEPTORS,
      useClass: AuthInterceptor,
      multi: true
    },
    {
      provide: HTTP_INTERCEPTORS,
      useClass: ErrorInterceptor,
      multi: true
    }
  ]
})
export class AppModule { }
```

---

## Communication entre Composants Angular

### 21. Comment partager des données entre composants ?

**1. Parent vers Enfant : `@Input()`**

```typescript
// Parent Component
@Component({
  selector: 'app-parent',
  template: `
    <app-child [data]="parentData" [name]="'John'"></app-child>
  `
})
export class ParentComponent {
  parentData = 'Données du parent';
}

// Enfant Component
@Component({
  selector: 'app-child',
  template: '<div>{{ data }} - {{ name }}</div>'
})
export class ChildComponent {
  @Input() data: string = '';
  @Input() name: string = '';
}
```

**2. Enfant vers Parent : `@Output()` et `EventEmitter`**

```typescript
// Enfant Component
@Component({
  selector: 'app-child',
  template: `
    <button (click)="sendData()">Envoyer</button>
  `
})
export class ChildComponent {
  @Output() dataEvent = new EventEmitter<string>();
  
  sendData() {
    this.dataEvent.emit('Données de l\'enfant');
  }
}

// Parent Component
@Component({
  selector: 'app-parent',
  template: `
    <app-child (dataEvent)="receiveData($event)"></app-child>
    <p>{{ receivedData }}</p>
  `
})
export class ParentComponent {
  receivedData: string = '';
  
  receiveData(data: string) {
    this.receivedData = data;
  }
}
```

**3. Service partagé avec Subject/BehaviorSubject**

```typescript
import { Injectable } from '@angular/core';
import { BehaviorSubject, Observable } from 'rxjs';

@Injectable({ providedIn: 'root' })
export class SharedService {
  private dataSubject = new BehaviorSubject<string>('');
  data$: Observable<string> = this.dataSubject.asObservable();
  
  updateData(data: string) {
    this.dataSubject.next(data);
  }
  
  getCurrentData(): string {
    return this.dataSubject.value;
  }
}

// Component A
export class ComponentA {
  constructor(private sharedService: SharedService) { }
  
  sendData() {
    this.sharedService.updateData('Données de A');
  }
}

// Component B
export class ComponentB implements OnInit, OnDestroy {
  data: string = '';
  private subscription: any;
  
  constructor(private sharedService: SharedService) { }
  
  ngOnInit() {
    this.subscription = this.sharedService.data$.subscribe(data => {
      this.data = data;
    });
  }
  
  ngOnDestroy() {
    this.subscription?.unsubscribe();
  }
}
```

**4. ViewChild pour accéder à un composant enfant**

```typescript
// Parent Component
import { ViewChild, AfterViewInit } from '@angular/core';

@Component({
  selector: 'app-parent',
  template: '<app-child #childRef></app-child>'
})
export class ParentComponent implements AfterViewInit {
  @ViewChild('childRef') childComponent!: ChildComponent;
  
  ngAfterViewInit() {
    // Accéder aux méthodes/propriétés de l'enfant
    this.childComponent.childMethod();
  }
}
```

---

## Détection de Changements Angular

### 22. Comment fonctionne la détection de changements dans Angular ?

Angular utilise Zone.js pour détecter les changements. À chaque événement asynchrone, Angular vérifie si les données du modèle ont changé et met à jour la vue si nécessaire.

**Stratégies de détection de changements :**

1. **Default** : Vérifie tout l'arbre de composants
2. **OnPush** : Vérifie uniquement si les `@Input()` changent ou si un événement est émis

```typescript
import { Component, ChangeDetectionStrategy, ChangeDetectorRef } from '@angular/core';

// Stratégie Default (par défaut)
@Component({
  selector: 'app-default',
  changeDetection: ChangeDetectionStrategy.Default
})
export class DefaultComponent {
  data: string = '';
  
  updateData() {
    this.data = 'Nouvelle valeur'; // Détection automatique
  }
}

// Stratégie OnPush (optimisée)
@Component({
  selector: 'app-onpush',
  changeDetection: ChangeDetectionStrategy.OnPush
})
export class OnPushComponent {
  @Input() data: string = '';
  
  constructor(private cdr: ChangeDetectorRef) { }
  
  updateData() {
    // Avec OnPush, il faut déclencher manuellement la détection
    this.cdr.markForCheck();
    // ou
    this.cdr.detectChanges();
  }
}
```

**Quand utiliser OnPush :**

- Pour améliorer les performances
- Quand les données changent rarement
- Dans les grandes applications

---

## Pipes Angular

### 23. Qu'est-ce qu'un Pipe ?

Un Pipe transforme les données dans le template. Angular fournit des pipes intégrés et permet de créer des pipes personnalisés.

**Pipes intégrés :**

```html
<!-- Date -->
{{ date | date:'dd/MM/yyyy' }}
{{ date | date:'short' }}

<!-- Currency -->
{{ price | currency:'EUR':'symbol':'1.2-2' }}

<!-- Uppercase/Lowercase -->
{{ text | uppercase }}
{{ text | lowercase }}

<!-- Slice -->
{{ array | slice:0:3 }}

<!-- Async (pour les Observables/Promises) -->
{{ data$ | async }}

<!-- JSON (pour le debug) -->
{{ object | json }}
```

**Pipe personnalisé :**

```typescript
import { Pipe, PipeTransform } from '@angular/core';

@Pipe({ 
  name: 'exponential',
  pure: true // Par défaut, true = pipe pur (mieux pour les performances)
})
export class ExponentialPipe implements PipeTransform {
  transform(value: number, exponent: number = 1): number {
    return Math.pow(value, exponent);
  }
}

// Utilisation
// {{ 2 | exponential:3 }} // 8
```

**Pipe impur (exécuté à chaque cycle de détection) :**

```typescript
@Pipe({
  name: 'impurePipe',
  pure: false // Pipe impur
})
export class ImpurePipe implements PipeTransform {
  transform(value: any): any {
    // Exécuté à chaque cycle de détection
    return value;
  }
}
```

---

## Questions Avancées Angular

### 24. Qu'est-ce que le Lazy Loading ?

Le Lazy Loading charge les modules uniquement quand ils sont nécessaires, réduisant le temps de chargement initial.

```typescript
// app-routing.module.ts
const routes: Routes = [
  {
    path: 'admin',
    loadChildren: () => import('./admin/admin.module').then(m => m.AdminModule)
  },
  {
    path: 'dashboard',
    loadChildren: () => import('./dashboard/dashboard.module').then(m => m.DashboardModule)
  }
];

// admin-routing.module.ts (dans le module lazy-loaded)
const routes: Routes = [
  {
    path: '',
    component: AdminComponent
  },
  {
    path: 'users',
    component: UsersComponent
  }
];
```

**Avantages :**

- Réduction de la taille du bundle initial
- Amélioration du temps de chargement
- Meilleure expérience utilisateur

---

### 25. Qu'est-ce que $scope et $rootScope ?

**Note :** Ces concepts sont d'AngularJS (version 1.x), pas d'Angular moderne (2+).

- **$scope** : Peut être considéré comme un modèle, un objet qui lie le contrôleur et la vue
- **$rootScope** : Aide à la communication entre différents contrôleurs d'une application. AngularJS ne peut avoir qu'un seul rootScope pour une application

Dans Angular moderne, ces concepts n'existent plus. On utilise :
- Les propriétés de classe du composant (au lieu de $scope)
- Les services avec RxJS (au lieu de $rootScope)
- `@Input()` et `@Output()` pour la communication parent-enfant

---

## Questions Fondamentales React

### 1. Qu'est-ce que React ?

React est une bibliothèque JavaScript front-end développée par Facebook en 2011 qui suit l'approche basée sur les composants pour créer des composants UI réutilisables. C'est une bibliothèque, pas un framework, qui nous donne toute la puissance de JavaScript avec des fonctionnalités intégrées pour construire des interfaces utilisateur.

**Caractéristiques principales :**

- Architecture basée sur les composants
- Virtual DOM pour des performances optimales
- Unidirectionnel (one-way data binding)
- JSX pour écrire du HTML dans JavaScript
- Écosystème riche et communauté active

---

### 2. Pourquoi utiliser React ?

Les fonctionnalités importantes de React incluent le support complet de Facebook, la stabilité du code avec liaison de données unidirectionnelle. React permet de créer facilement des interfaces utilisateur avec des outils comme JSX, de construire des applications à page unique (SPA), et même des applications mobiles avec React Native.

**Avantages :**

- **Composants réutilisables** : Créer une fois, utiliser partout
- **Virtual DOM** : Mises à jour performantes
- **Écosystème riche** : Nombreuses bibliothèques et outils
- **React Native** : Réutiliser les compétences pour le mobile
- **Grande communauté** : Support et ressources abondants
- **Flexibilité** : Bibliothèque légère, pas un framework imposant

---

### 3. Qu'est-ce que JSX ?

JSX signifie JavaScript XML, c'est un type de fichier utilisé par React qui utilise l'expressivité de JavaScript avec HTML, ce qui rend les applications robustes et augmente leurs performances. Bien que JSX ressemble à du HTML, il s'agit en fait d'appels de fonctions JavaScript : écrire un div en JSX équivaut à appeler `React.createElement()`.

```javascript
// JSX
const element = <h1>Bonjour React!</h1>;

// Équivalent JavaScript
const element = React.createElement('h1', null, 'Bonjour React!');

// JSX avec attributs
const element = <div className="container" id="main">Contenu</div>;

// Équivalent JavaScript
const element = React.createElement(
  'div',
  { className: 'container', id: 'main' },
  'Contenu'
);

// JSX avec expressions
const name = 'John';
const element = <h1>Bonjour, {name}!</h1>;

// JSX avec conditions
const isLoggedIn = true;
const element = (
  <div>
    {isLoggedIn ? <p>Bienvenue!</p> : <p>Veuillez vous connecter</p>}
  </div>
);
```

**Règles JSX :**

- Un seul élément racine (ou utiliser Fragment)
- Utiliser `className` au lieu de `class`
- Utiliser `htmlFor` au lieu de `for`
- Les attributs en camelCase (`onClick`, `onChange`)

---

### 4. Qu'est-ce qu'un composant React ?

Un composant est un bloc de construction réutilisable de l'interface utilisateur. Il existe deux types de composants :

**1. Composant fonctionnel (recommandé) :**

```javascript
// Composant fonctionnel simple
function Welcome(props) {
  return <h1>Bonjour, {props.name}!</h1>;
}

// Composant fonctionnel avec arrow function
const Welcome = (props) => {
  return <h1>Bonjour, {props.name}!</h1>;
};

// Composant fonctionnel avec destructuring
const Welcome = ({ name, age }) => {
  return (
    <div>
      <h1>Bonjour, {name}!</h1>
      <p>Vous avez {age} ans</p>
    </div>
  );
};
```

**2. Composant classe (legacy) :**

```javascript
class Welcome extends React.Component {
  render() {
    return <h1>Bonjour, {this.props.name}!</h1>;
  }
}
```

**Utilisation :**

```javascript
function App() {
  return (
    <div>
      <Welcome name="Alice" age={25} />
      <Welcome name="Bob" age={30} />
    </div>
  );
}
```

---

### 5. Qu'est-ce qu'un élément React vs un composant React ?

- **Un élément React** : Un objet simple et immuable créé pour représenter un nœud DOM, qui ne peut pas être modifié une fois créé
- **Un composant React** : Modifiable et produit une sortie JSX une fois rendu

```javascript
// Élément React (objet immuable)
const element = <h1>Hello, world</h1>;

// Composant React (fonction/classe qui retourne des éléments)
function Welcome({ name }) {
  return <h1>Hello, {name}</h1>;
}

// Un composant peut retourner plusieurs éléments
function App() {
  return (
    <>
      <Welcome name="Alice" />
      <Welcome name="Bob" />
    </>
  );
}
```

---

### 6. Qu'est-ce que le Virtual DOM ?

Le DOM virtuel est un objet JavaScript léger qui est à l'origine une copie du vrai DOM. C'est une arborescence de nœuds qui répertorie les éléments, leurs attributs et leur contenu en tant qu'objets et leurs propriétés. React utilise le Virtual DOM pour optimiser les mises à jour en comparant les changements avant de les appliquer au DOM réel.

**Comment ça fonctionne :**

1. React crée une représentation virtuelle du DOM en mémoire
2. Quand l'état change, React crée un nouveau Virtual DOM
3. React compare (diff) l'ancien et le nouveau Virtual DOM
4. React met à jour uniquement les parties qui ont changé dans le vrai DOM (reconciliation)

**Avantages :**

- Performance améliorée (moins de manipulations DOM)
- Mises à jour efficaces (seulement ce qui change)
- Code plus simple (React gère les optimisations)

```javascript
// Exemple de représentation Virtual DOM
const virtualElement = {
  type: 'div',
  props: {
    className: 'container',
    children: [
      {
        type: 'h1',
        props: {
          children: 'Hello React'
        }
      }
    ]
  }
};
```

---

## Props et State React

### 7. Quelle est la différence entre Props et State ?

La principale différence est que l'État est mutable et les Props sont immuables.

**Props :**

- Ce sont des composants en lecture seule qui doivent être maintenus purs, c'est-à-dire immuables
- Ils sont toujours transmis du composant parent aux composants enfants
- Un composant enfant ne peut jamais renvoyer un Props au composant parent
- Les props ne peuvent pas être modifiées par le composant qui les reçoit

**State :**

- C'est un objet qui décide du rendu d'un composant spécifique et de son comportement
- L'état stocke les informations qui peuvent être modifiées au cours de la durée de vie d'un composant React
- Le state est local au composant et peut être modifié avec `setState` (classes) ou les setters de hooks (fonctions)

```javascript
// Props (immuables, passées du parent)
function Blog({ post }) {
  return (
    <div>
      <h1>{post.title}</h1>
      <p>{post.content}</p>
    </div>
  );
}

function App() {
  const post = { title: "Mon Article!", content: "Contenu..." };
  return <Blog post={post} />;
}

// State (mutable, local au composant)
import { useState } from 'react';

function Counter() {
  const [count, setCount] = useState(0);
  
  return (
    <div>
      <p>Compteur: {count}</p>
      <button onClick={() => setCount(count + 1)}>+</button>
      <button onClick={() => setCount(count - 1)}>-</button>
    </div>
  );
}
```

**Quand utiliser Props vs State :**

- **Props** : Données qui viennent du parent, configuration, valeurs initiales
- **State** : Données qui changent dans le composant, interactions utilisateur, données calculées localement

---

### 8. Comment passer des données entre composants ?

Il y a 2 façons principales de passer des données aux composants React : les props sont des données transmises par le parent immédiat d'un composant, et le contexte est une donnée transmise par un fournisseur de contexte à tout composant qui consomme le contexte.

**1. Props (Parent → Enfant) :**

```javascript
// Parent
function App() {
  const data = "Données du parent";
  return <ChildComponent data={data} />;
}

// Enfant
function ChildComponent({ data }) {
  return <p>{data}</p>;
}
```

**2. Callbacks (Enfant → Parent) :**

```javascript
// Parent
function App() {
  const [message, setMessage] = useState('');
  
  const handleChildMessage = (msg) => {
    setMessage(msg);
  };
  
  return (
    <div>
      <p>Message reçu: {message}</p>
      <ChildComponent onSendMessage={handleChildMessage} />
    </div>
  );
}

// Enfant
function ChildComponent({ onSendMessage }) {
  const handleClick = () => {
    onSendMessage("Message de l'enfant");
  };
  
  return <button onClick={handleClick}>Envoyer</button>;
}
```

**3. Context API (Partage global) :**

```javascript
import { createContext, useContext, useState } from 'react';

const DataContext = createContext();

function App() {
  const [sharedData, setSharedData] = useState('Données partagées');
  
  return (
    <DataContext.Provider value={{ sharedData, setSharedData }}>
      <ComponentA />
      <ComponentB />
    </DataContext.Provider>
  );
}

function ComponentA() {
  const { sharedData } = useContext(DataContext);
  return <p>{sharedData}</p>;
}

function ComponentB() {
  const { setSharedData } = useContext(DataContext);
  return (
    <button onClick={() => setSharedData('Nouvelle valeur')}>
      Modifier
    </button>
  );
}
```

---

## React Hooks

### 9. Qu'est-ce qu'un Hook React ?

Les hooks React permettent d'utiliser le State et d'autres fonctionnalités sans écrire de classe. Avec les React Hooks, les class components sont remplaçables par des function components dans la majorité des cas.

**Règles des Hooks :**

1. Appeler les Hooks uniquement au niveau supérieur (pas dans des boucles, conditions ou fonctions imbriquées)
2. Appeler les Hooks uniquement depuis des fonctions React (composants fonctionnels ou custom hooks)

**Hooks intégrés principaux :**

- `useState` : Gérer l'état local
- `useEffect` : Effets de bord
- `useContext` : Accéder au contexte
- `useRef` : Références
- `useReducer` : État complexe
- `useMemo` : Mémorisation de valeurs
- `useCallback` : Mémorisation de fonctions

---

### 10. Qu'est-ce que useState ?

`useState` permet d'ajouter un état local à un composant fonctionnel. Il retourne une paire : la valeur actuelle de l'état et une fonction pour la mettre à jour.

```javascript
import { useState } from 'react';

function Counter() {
  const [count, setCount] = useState(0);
  
  return (
    <div>
      <p>Vous avez cliqué {count} fois</p>
      <button onClick={() => setCount(count + 1)}>
        Cliquez-moi
      </button>
    </div>
  );
}

// useState avec fonction d'initialisation (lazy initial state)
function ExpensiveComponent() {
  const [data, setData] = useState(() => {
    // Cette fonction ne s'exécute qu'une fois
    return computeExpensiveValue();
  });
}

// useState avec objet
function Form() {
  const [formData, setFormData] = useState({
    name: '',
    email: ''
  });
  
  const handleChange = (field, value) => {
    setFormData(prev => ({
      ...prev,
      [field]: value
    }));
  };
  
  return (
    <form>
      <input 
        value={formData.name}
        onChange={(e) => handleChange('name', e.target.value)}
      />
      <input 
        value={formData.email}
        onChange={(e) => handleChange('email', e.target.value)}
      />
    </form>
  );
}
```

---

### 11. Qu'est-ce que useEffect ?

`useEffect` permet d'effectuer des effets de bord dans les composants fonctionnels (appels API, souscriptions, timers, etc.). Il s'exécute après le rendu du composant.

```javascript
import { useState, useEffect } from 'react';

function DataFetcher() {
  const [data, setData] = useState(null);
  const [loading, setLoading] = useState(true);
  
  useEffect(() => {
    // Effet : récupération des données
    fetch('https://api.example.com/data')
      .then(response => response.json())
      .then(data => {
        setData(data);
        setLoading(false);
      });
    
    // Fonction de nettoyage (optionnelle)
    return () => {
      console.log('Nettoyage');
    };
  }, []); // [] = exécuté une seule fois au montage
  
  if (loading) return <div>Chargement...</div>;
  
  return <div>{data ? <p>{data}</p> : <p>Aucune donnée</p>}</div>;
}
```

---

### 12. Quand useEffect s'exécute-t-il ?

**Sans dépendances :** `useEffect(() => {})` → S'exécute après chaque rendu

```javascript
useEffect(() => {
  console.log('Exécuté à chaque rendu');
});
```

**Tableau vide :** `useEffect(() => {}, [])` → S'exécute une seule fois au montage

```javascript
useEffect(() => {
  console.log('Exécuté une seule fois au montage');
}, []);
```

**Avec dépendances :** `useEffect(() => {}, [count])` → S'exécute quand `count` change

```javascript
const [count, setCount] = useState(0);
const [name, setName] = useState('');

useEffect(() => {
  console.log('Exécuté quand count change');
}, [count]); // Seulement quand count change

useEffect(() => {
  console.log('Exécuté quand count OU name change');
}, [count, name]); // Quand count ou name change
```

---

### 13. Qu'est-ce que la fonction de nettoyage dans useEffect ?

La fonction de nettoyage est retournée par `useEffect` et s'exécute avant que le composant ne soit démonté ou avant la prochaine exécution de l'effet. Utile pour nettoyer les abonnements, timers, etc.

```javascript
useEffect(() => {
  const timer = setInterval(() => {
    console.log('Tick');
  }, 1000);
  
  // Nettoyage : s'exécute avant le démontage ou avant la prochaine exécution
  return () => {
    clearInterval(timer);
    console.log('Timer nettoyé');
  };
}, []);

// Exemple avec souscription
useEffect(() => {
  const subscription = someObservable.subscribe(data => {
    console.log(data);
  });
  
  return () => {
    subscription.unsubscribe();
  };
}, []);

// Exemple avec event listener
useEffect(() => {
  const handleResize = () => {
    console.log('Window resized');
  };
  
  window.addEventListener('resize', handleResize);
  
  return () => {
    window.removeEventListener('resize', handleResize);
  };
}, []);
```

---

### 14. Qu'est-ce que useContext ?

`useContext` permet d'accéder aux valeurs d'un contexte sans avoir à imbriquer des composants Consumer.

```javascript
import { createContext, useContext, useState } from 'react';

const ThemeContext = createContext('light');

function ThemedButton() {
  const theme = useContext(ThemeContext);
  return (
    <button style={{ 
      background: theme === 'dark' ? '#333' : '#fff',
      color: theme === 'dark' ? '#fff' : '#333'
    }}>
      Bouton
    </button>
  );
}

function App() {
  const [theme, setTheme] = useState('light');
  
  return (
    <ThemeContext.Provider value={theme}>
      <ThemedButton />
      <button onClick={() => setTheme(theme === 'light' ? 'dark' : 'light')}>
        Changer le thème
      </button>
    </ThemeContext.Provider>
  );
}
```

---

### 15. Qu'est-ce que useRef ?

Un ref est une référence à un élément DOM dans React. Les ref sont créés à l'aide du hook `useRef` et peuvent être immédiatement placés dans une variable, puis passés à un élément React pour obtenir une référence à l'élément DOM sous-jacent.

```javascript
import { useRef } from 'react';

function TextInput() {
  const inputRef = useRef(null);
  
  const handleClick = () => {
    inputRef.current.focus();
  };
  
  return (
    <div>
      <input ref={inputRef} type="text" />
      <button onClick={handleClick}>Focus</button>
    </div>
  );
}

// useRef pour stocker des valeurs qui ne déclenchent pas de re-render
function Timer() {
  const [count, setCount] = useState(0);
  const intervalRef = useRef(null);
  
  const startTimer = () => {
    intervalRef.current = setInterval(() => {
      setCount(prev => prev + 1);
    }, 1000);
  };
  
  const stopTimer = () => {
    clearInterval(intervalRef.current);
  };
  
  return (
    <div>
      <p>{count}</p>
      <button onClick={startTimer}>Démarrer</button>
      <button onClick={stopTimer}>Arrêter</button>
    </div>
  );
}
```

---

### 16. Qu'est-ce que useReducer ?

`useReducer` est une alternative à `useState` pour gérer des états complexes. Il fonctionne comme Redux avec des actions et un reducer.

```javascript
import { useReducer } from 'react';

function reducer(state, action) {
  switch (action.type) {
    case 'increment':
      return { count: state.count + 1 };
    case 'decrement':
      return { count: state.count - 1 };
    case 'reset':
      return { count: 0 };
    case 'set':
      return { count: action.payload };
    default:
      return state;
  }
}

function Counter() {
  const [state, dispatch] = useReducer(reducer, { count: 0 });
  
  return (
    <div>
      <p>Count: {state.count}</p>
      <button onClick={() => dispatch({ type: 'increment' })}>+</button>
      <button onClick={() => dispatch({ type: 'decrement' })}>-</button>
      <button onClick={() => dispatch({ type: 'reset' })}>Reset</button>
      <button onClick={() => dispatch({ type: 'set', payload: 10 })}>
        Set to 10
      </button>
    </div>
  );
}
```

---

### 17. Quelles sont les règles des Hooks ?

**1. Appeler les Hooks uniquement au niveau supérieur :**

Ne pas appeler dans des boucles, conditions ou fonctions imbriquées.

```javascript
// ❌ Incorrect
function Component() {
  if (condition) {
    const [state, setState] = useState(0); // Erreur !
  }
}

// ✅ Correct
function Component() {
  const [state, setState] = useState(0);
  if (condition) {
    // Utiliser state ici
  }
}
```

**2. Appeler les Hooks uniquement depuis des fonctions React :**

Composants fonctionnels ou custom hooks.

```javascript
// ✅ Correct
function Component() {
  const [state, setState] = useState(0);
}

// ✅ Correct (custom hook)
function useCustomHook() {
  const [state, setState] = useState(0);
  return state;
}

// ❌ Incorrect
function regularFunction() {
  const [state, setState] = useState(0); // Erreur !
}
```

---

## Cycle de Vie des Composants React

### 18. Quelles sont les phases du cycle de vie d'un composant ?

Les étapes importantes du cycle de vie de React incluent plusieurs phases. Pour les composants classe :

**Montage :**

- `constructor()` : Initialisation
- `render()` : Rendu du composant
- `componentDidMount()` : Après le montage dans le DOM

**Mise à jour :**

- `render()` : Re-rendu
- `componentDidUpdate()` : Après la mise à jour

**Démontage :**

- `componentWillUnmount()` : Avant le démontage (nettoyage)

```javascript
class LifecycleComponent extends React.Component {
  constructor(props) {
    super(props);
    this.state = { count: 0 };
    console.log('1. Constructor');
  }
  
  componentDidMount() {
    console.log('3. Component Did Mount');
    // Appels API, souscriptions, etc.
  }
  
  componentDidUpdate(prevProps, prevState) {
    console.log('4. Component Did Update');
    if (prevState.count !== this.state.count) {
      console.log('Count a changé');
    }
  }
  
  componentWillUnmount() {
    console.log('5. Component Will Unmount');
    // Nettoyage : unsubscribe, clearInterval, etc.
  }
  
  render() {
    console.log('2. Render');
    return (
      <div>
        <p>{this.state.count}</p>
        <button onClick={() => this.setState({ count: this.state.count + 1 })}>
          +
        </button>
      </div>
    );
  }
}
```

---

### 19. Comment répliquer le cycle de vie avec les Hooks ?

```javascript
import { useEffect, useState } from 'react';

function LifecycleComponent() {
  const [count, setCount] = useState(0);
  
  // componentDidMount
  useEffect(() => {
    console.log('Composant monté');
    // Logique d'initialisation
  }, []); // Tableau vide = une seule fois
  
  // componentDidUpdate
  useEffect(() => {
    console.log('État mis à jour');
    // Logique après chaque mise à jour
  }); // Pas de tableau de dépendances = à chaque rendu
  
  // componentDidUpdate (seulement quand count change)
  useEffect(() => {
    console.log('Count a changé:', count);
  }, [count]); // Dépendance spécifique
  
  // componentWillUnmount
  useEffect(() => {
    return () => {
      console.log('Composant démonté');
      // Nettoyage
    };
  }, []);
  
  return (
    <div>
      <p>{count}</p>
      <button onClick={() => setCount(count + 1)}>+</button>
    </div>
  );
}
```

---

## Gestion d'État Avancée React

### 20. Qu'est-ce qu'un composant contrôlé vs non contrôlé ?

**Composant contrôlé :** Contrôle la valeur d'un champ, prend la valeur courante par le biais de props et notifie les changements par le biais de callbacks comme `onChange`.

**Composant non contrôlé :** Stocke et gère son propre état en interne.

```javascript
// Composant contrôlé
function ControlledInput() {
  const [value, setValue] = useState('');
  
  const handleChange = (e) => {
    setValue(e.target.value);
  };
  
  return (
    <div>
      <input 
        value={value} 
        onChange={handleChange}
        placeholder="Tapez quelque chose"
      />
      <p>Valeur: {value}</p>
    </div>
  );
}

// Composant non contrôlé
function UncontrolledInput() {
  const inputRef = useRef();
  
  const handleSubmit = () => {
    console.log('Valeur:', inputRef.current.value);
  };
  
  return (
    <div>
      <input ref={inputRef} type="text" />
      <button onClick={handleSubmit}>Soumettre</button>
    </div>
  );
}

// Formulaire non contrôlé avec defaultValue
function UncontrolledForm() {
  const handleSubmit = (e) => {
    e.preventDefault();
    const formData = new FormData(e.target);
    console.log('Nom:', formData.get('name'));
    console.log('Email:', formData.get('email'));
  };
  
  return (
    <form onSubmit={handleSubmit}>
      <input name="name" defaultValue="John" />
      <input name="email" type="email" defaultValue="john@example.com" />
      <button type="submit">Soumettre</button>
    </form>
  );
}
```

**Quand utiliser :**

- **Contrôlé** : Besoin de validation en temps réel, synchronisation avec d'autres composants
- **Non contrôlé** : Formulaires simples, intégration avec du code non-React

---

### 21. Qu'est-ce qu'un Higher-Order Component (HOC) ?

Les High Order Components permettent de réutiliser la logique des composants. Ce sont des composants personnalisés qui enveloppent un autre composant en leur sein.

```javascript
// HOC pour l'authentification
function withAuth(Component) {
  return function AuthComponent(props) {
    const [isAuthenticated, setIsAuthenticated] = useState(false);
    
    useEffect(() => {
      // Vérifier l'authentification
      const checkAuth = async () => {
        const auth = await checkAuthentication();
        setIsAuthenticated(auth);
      };
      checkAuth();
    }, []);
    
    if (!isAuthenticated) {
      return <div>Accès refusé. Veuillez vous connecter.</div>;
    }
    
    return <Component {...props} />;
  };
}

// Utilisation
const Dashboard = () => <div>Tableau de bord</div>;
const ProtectedDashboard = withAuth(Dashboard);

// HOC pour le logging
function withLogging(Component) {
  return function LoggedComponent(props) {
    useEffect(() => {
      console.log(`Component ${Component.name} monté`);
      return () => {
        console.log(`Component ${Component.name} démonté`);
      };
    }, []);
    
    return <Component {...props} />;
  };
}

// Composition de HOCs
const EnhancedDashboard = withLogging(withAuth(Dashboard));
```

---

### 22. Qu'est-ce que le Context API ?

Context permet de partager des données à travers l'arbre de composants sans passer manuellement les props à chaque niveau.

```javascript
import { createContext, useContext, useState } from 'react';

const UserContext = createContext(null);

function App() {
  const [user, setUser] = useState({ name: 'John', email: 'john@example.com' });
  
  return (
    <UserContext.Provider value={{ user, setUser }}>
      <Profile />
      <Settings />
    </UserContext.Provider>
  );
}

function Profile() {
  const { user } = useContext(UserContext);
  return (
    <div>
      <h1>Profil</h1>
      <p>Nom: {user.name}</p>
      <p>Email: {user.email}</p>
    </div>
  );
}

function Settings() {
  const { user, setUser } = useContext(UserContext);
  
  const updateName = (newName) => {
    setUser({ ...user, name: newName });
  };
  
  return (
    <div>
      <h1>Paramètres</h1>
      <input 
        value={user.name}
        onChange={(e) => updateName(e.target.value)}
      />
    </div>
  );
}
```

---

## React Router

### 23. Qu'est-ce que React Router ?

React Router est une bibliothèque qui fournit des fonctionnalités de routage dans une application React. Il facilite l'inclusion et l'utilisation de composants de navigation riches, ce qui peut être très utile pour les projets volumineux ou complexes.

```javascript
import { BrowserRouter, Routes, Route, Link, Navigate } from 'react-router-dom';

function App() {
  return (
    <BrowserRouter>
      <nav>
        <Link to="/">Accueil</Link>
        <Link to="/about">À propos</Link>
        <Link to="/users">Utilisateurs</Link>
      </nav>
      
      <Routes>
        <Route path="/" element={<Home />} />
        <Route path="/about" element={<About />} />
        <Route path="/users" element={<Users />} />
        <Route path="/user/:id" element={<User />} />
        <Route path="/redirect" element={<Navigate to="/" />} />
        <Route path="*" element={<NotFound />} />
      </Routes>
    </BrowserRouter>
  );
}

function Home() {
  return <h1>Page d'accueil</h1>;
}

function About() {
  return <h1>À propos</h1>;
}

function Users() {
  return <h1>Liste des utilisateurs</h1>;
}

function User() {
  const { id } = useParams();
  return <h1>Utilisateur ID: {id}</h1>;
}

function NotFound() {
  return <h1>404 - Page non trouvée</h1>;
}
```

---

### 24. Comment accéder aux paramètres d'URL ?

```javascript
import { useParams, useNavigate, useLocation, useSearchParams } from 'react-router-dom';

function User() {
  const { id } = useParams(); // Paramètre de route : /user/:id
  const navigate = useNavigate();
  const location = useLocation();
  const [searchParams, setSearchParams] = useSearchParams();
  
  const name = searchParams.get('name'); // Query param : ?name=John
  
  return (
    <div>
      <h1>User ID: {id}</h1>
      <p>Nom: {name}</p>
      <p>Pathname: {location.pathname}</p>
      <button onClick={() => navigate('/home')}>Retour</button>
      <button onClick={() => setSearchParams({ name: 'Alice' })}>
        Changer le nom
      </button>
    </div>
  );
}
```

---

## Performance et Optimisation React

### 25. Qu'est-ce qu'un Pure Component ?

Les composants purs sont les composants les plus rapides qui peuvent remplacer n'importe quel composant avec seulement un render(). Ils améliorent la simplicité du code et les performances de l'application.

```javascript
// Pure Component (classe)
class PureCounter extends React.PureComponent {
  render() {
    return <div>{this.props.count}</div>;
  }
}

// Équivalent fonctionnel avec React.memo
const PureCounter = React.memo(({ count }) => {
  return <div>{count}</div>;
});

// React.memo avec comparaison personnalisée
const ExpensiveComponent = React.memo(
  ({ data }) => {
    return <div>{data}</div>;
  },
  (prevProps, nextProps) => {
    // Retourne true si les props sont égales (pas de re-render)
    return prevProps.data.id === nextProps.data.id;
  }
);
```

---

### 26. Comment optimiser les performances dans React ?

**1. Utiliser React.memo() pour mémoriser les composants**

```javascript
const ExpensiveComponent = React.memo(({ data }) => {
  return <div>{data}</div>;
});
```

**2. Utiliser useMemo() pour mémoriser des valeurs calculées**

```javascript
function ExpensiveCalculation({ items }) {
  const expensiveValue = useMemo(() => {
    return items.reduce((sum, item) => sum + item.value, 0);
  }, [items]); // Recalcule seulement si items change
  
  return <div>{expensiveValue}</div>;
}
```

**3. Utiliser useCallback() pour mémoriser des fonctions**

```javascript
function Parent({ items }) {
  const [count, setCount] = useState(0);
  
  const handleClick = useCallback(() => {
    console.log('Clicked');
  }, []); // Fonction stable
  
  return (
    <div>
      <ExpensiveChild onClick={handleClick} />
    </div>
  );
}

const ExpensiveChild = React.memo(({ onClick }) => {
  return <button onClick={onClick}>Cliquez</button>;
});
```

**4. Lazy loading avec React.lazy() et Suspense**

```javascript
import { lazy, Suspense } from 'react';

const HeavyComponent = lazy(() => import('./HeavyComponent'));

function App() {
  return (
    <Suspense fallback={<div>Chargement...</div>}>
      <HeavyComponent />
    </Suspense>
  );
}
```

**5. Virtualisation des listes longues**

```javascript
import { FixedSizeList } from 'react-window';

function LongList({ items }) {
  return (
    <FixedSizeList
      height={600}
      itemCount={items.length}
      itemSize={50}
      width="100%"
    >
      {({ index, style }) => (
        <div style={style}>
          {items[index].name}
        </div>
      )}
    </FixedSizeList>
  );
}
```

---

## Liste et Clés React

### 27. Pourquoi les clés sont-elles importantes dans les listes ?

Les clés indiquent à React quel élément ou composant est dans une liste. Sinon, si nous devions modifier les éléments de cette liste, React ne saurait pas dans quel ordre les mettre. React se charge de mettre à jour le DOM à notre place en utilisant un DOM virtuel, mais les clés sont nécessaires pour que React puisse le mettre à jour correctement.

```javascript
function TodoList({ todos }) {
  return (
    <ul>
      {todos.map(todo => (
        <li key={todo.id}>{todo.text}</li>
      ))}
    </ul>
  );
}

// ❌ Mauvaise pratique : utiliser l'index comme clé
function BadList({ items }) {
  return (
    <ul>
      {items.map((item, index) => (
        <li key={index}>{item.name}</li> // Problème si l'ordre change
      ))}
    </ul>
  );
}

// ✅ Bonne pratique : utiliser un identifiant unique
function GoodList({ items }) {
  return (
    <ul>
      {items.map(item => (
        <li key={item.id}>{item.name}</li>
      ))}
    </ul>
  );
}
```

**Pourquoi les clés sont importantes :**

- Aident React à identifier quels éléments ont changé
- Améliorent les performances (moins de re-renders)
- Évitent les bugs lors de la réorganisation des éléments

---

## React et TypeScript

### 28. Comment typer des composants React avec TypeScript ?

```typescript
import React, { useState } from 'react';

// Props typées
interface ButtonProps {
  text: string;
  onClick: () => void;
  disabled?: boolean;
  variant?: 'primary' | 'secondary';
}

const Button: React.FC<ButtonProps> = ({ 
  text, 
  onClick, 
  disabled = false,
  variant = 'primary'
}) => {
  return (
    <button 
      onClick={onClick} 
      disabled={disabled}
      className={variant}
    >
      {text}
    </button>
  );
};

// Hook typé
function Counter() {
  const [count, setCount] = useState<number>(0);
  const [name, setName] = useState<string>('');
  
  return (
    <div>
      <p>{count}</p>
      <input 
        value={name}
        onChange={(e) => setName(e.target.value)}
      />
    </div>
  );
}

// Props avec enfants
interface CardProps {
  title: string;
  children: React.ReactNode;
}

const Card: React.FC<CardProps> = ({ title, children }) => {
  return (
    <div className="card">
      <h2>{title}</h2>
      {children}
    </div>
  );
};

// Event handlers typés
interface FormProps {
  onSubmit: (data: { name: string; email: string }) => void;
}

const Form: React.FC<FormProps> = ({ onSubmit }) => {
  const handleSubmit = (e: React.FormEvent<HTMLFormElement>) => {
    e.preventDefault();
    onSubmit({ name: 'John', email: 'john@example.com' });
  };
  
  return <form onSubmit={handleSubmit}>...</form>;
};
```

---

## Questions Avancées React

### 29. Quelle est la différence entre React et React Native ?

**React JS** est une bibliothèque JavaScript open source frontale utilisée pour créer des interfaces utilisateur, tandis que **React Native** est un framework mobile open source qui permet aux développeurs d'utiliser React sur des plates-formes comme Android et iOS.

| React | React Native |
|-------|--------------|
| Pour le web | Pour mobile (iOS/Android) |
| Utilise le DOM | Utilise des composants natifs |
| HTML/CSS | StyleSheet API |
| `<div>`, `<span>` | `<View>`, `<Text>` |
| `onClick` | `onPress` |

```javascript
// React (Web)
function WebComponent() {
  return (
    <div onClick={() => console.log('clicked')}>
      <h1>Hello Web</h1>
    </div>
  );
}

// React Native (Mobile)
import { View, Text, TouchableOpacity } from 'react-native';

function MobileComponent() {
  return (
    <TouchableOpacity onPress={() => console.log('pressed')}>
      <View>
        <Text>Hello Mobile</Text>
      </View>
    </TouchableOpacity>
  );
}
```

---

### 30. Qu'est-ce que le rendu côté serveur (SSR) ?

Le rendu côté serveur est utile car il améliore l'expérience utilisateur et le référencement. Vous aurez besoin d'un environnement Node.js, d'un bundler comme Webpack et d'un framework comme Next.js et Remix pour rendre les applications React au moment de l'exécution.

**Avantages du SSR :**

- Meilleur SEO (moteurs de recherche)
- Temps de chargement initial plus rapide
- Meilleure expérience utilisateur

**Frameworks SSR pour React :**

- **Next.js** : Framework React avec SSR intégré
- **Remix** : Framework React moderne
- **Gatsby** : Pour les sites statiques

---

### 31. Qu'est-ce que le Lazy Loading ?

```javascript
import { lazy, Suspense } from 'react';

// Lazy loading d'un composant
const HeavyComponent = lazy(() => import('./HeavyComponent'));
const AdminPanel = lazy(() => import('./AdminPanel'));

function App() {
  return (
    <div>
      <Suspense fallback={<div>Chargement...</div>}>
        <HeavyComponent />
      </Suspense>
      
      <Suspense fallback={<div>Chargement du panneau admin...</div>}>
        <AdminPanel />
      </Suspense>
    </div>
  );
}

// Lazy loading avec React Router
import { lazy } from 'react';
import { Routes, Route } from 'react-router-dom';

const Home = lazy(() => import('./pages/Home'));
const About = lazy(() => import('./pages/About'));

function App() {
  return (
    <Suspense fallback={<div>Chargement...</div>}>
      <Routes>
        <Route path="/" element={<Home />} />
        <Route path="/about" element={<About />} />
      </Routes>
    </Suspense>
  );
}
```

---

### 32. Qu'est-ce qu'une fonction fléchée (arrow function) ?

Une fonction fléchée est simplement une manière plus courte de définir des fonctions. Il s'agit d'un raccourci ES6.

```javascript
// Fonction traditionnelle
const add = function(a, b) {
  return a + b;
};

// Arrow function
const add = (a, b) => a + b;

// Arrow function avec un seul paramètre
const square = x => x * x;

// Arrow function sans paramètres
const greet = () => 'Hello';

// Arrow function avec plusieurs lignes
const multiply = (a, b) => {
  const result = a * b;
  return result;
};

// Arrow function dans React
function Component() {
  const handleClick = () => {
    console.log('Clicked');
  };
  
  return <button onClick={handleClick}>Cliquez</button>;
}
```

---

### 33. Qu'est-ce qu'un Custom Hook ?

Un custom hook est une fonction JavaScript dont le nom commence par "use" et qui peut appeler d'autres Hooks.

```javascript
// Custom hook pour localStorage
function useLocalStorage(key, initialValue) {
  const [value, setValue] = useState(() => {
    const stored = localStorage.getItem(key);
    return stored ? JSON.parse(stored) : initialValue;
  });
  
  useEffect(() => {
    localStorage.setItem(key, JSON.stringify(value));
  }, [key, value]);
  
  return [value, setValue];
}

// Utilisation
function App() {
  const [name, setName] = useLocalStorage('name', 'John');
  
  return (
    <div>
      <input 
        value={name}
        onChange={(e) => setName(e.target.value)}
      />
    </div>
  );
}

// Custom hook pour les appels API
function useFetch(url) {
  const [data, setData] = useState(null);
  const [loading, setLoading] = useState(true);
  const [error, setError] = useState(null);
  
  useEffect(() => {
    fetch(url)
      .then(response => response.json())
      .then(data => {
        setData(data);
        setLoading(false);
      })
      .catch(error => {
        setError(error);
        setLoading(false);
      });
  }, [url]);
  
  return { data, loading, error };
}

// Utilisation
function DataComponent() {
  const { data, loading, error } = useFetch('https://api.example.com/data');
  
  if (loading) return <div>Chargement...</div>;
  if (error) return <div>Erreur: {error.message}</div>;
  
  return <div>{JSON.stringify(data)}</div>;
}
```

---

### 34. Comment créer une application React ?

La commande `create-react-app` est utilisée dans l'interface CLI (interface en ligne de commande) permettant à React de créer des applications sans configuration de build.

```bash
# Créer une nouvelle application React
npx create-react-app mon-app

# Naviguer dans le dossier
cd mon-app

# Démarrer le serveur de développement
npm start

# Build pour la production
npm run build

# Lancer les tests
npm test
```

**Alternatives modernes :**

```bash
# Vite (plus rapide)
npm create vite@latest mon-app -- --template react

# Next.js (avec SSR)
npx create-next-app mon-app
```

---

### 35. Qu'est-ce que la méthode render() ?

Chaque composant React doit obligatoirement avoir la méthode `render()`. Elle renvoie un seul élément React qui est la représentation du composant DOM natif. Si plusieurs éléments HTML doivent être rendus, ils doivent être regroupés dans une balise englobante.

```javascript
// Composant classe avec render()
class Welcome extends React.Component {
  render() {
    return <h1>Hello, {this.props.name}</h1>;
  }
}

// Composant fonctionnel (équivalent, pas besoin de render explicite)
function Welcome({ name }) {
  return <h1>Hello, {name}</h1>;
}

// Plusieurs éléments avec Fragment
function MultipleElements() {
  return (
    <>
      <h1>Titre</h1>
      <p>Paragraphe</p>
      <button>Bouton</button>
    </>
  );
}

// Ou avec div
function MultipleElementsDiv() {
  return (
    <div>
      <h1>Titre</h1>
      <p>Paragraphe</p>
    </div>
  );
}
```

---

## Questions Fondamentales C# {#questions-fondamentales-csharp}

### 1. Qu'est-ce que C# et quelles sont ses principales caractéristiques ?

C# (C Sharp) est un langage de programmation moderne, orienté objet et fortement typé développé par Microsoft. Il fait partie de la plateforme .NET.

**Principales caractéristiques :**

- **Langage orienté objet** : supporte l'encapsulation, l'héritage et le polymorphisme
- **Fortement typé** : vérification des types à la compilation
- **Gestion automatique de la mémoire** : garbage collector intégré
- **Sécurité des types** : évite les erreurs courantes de manipulation de mémoire
- **Moderne** : supporte la programmation asynchrone, LINQ, lambdas, etc.
- **Multiplateforme** : avec .NET Core/.NET 5+, fonctionne sur Windows, Linux et macOS
- **Intégré à l'écosystème .NET** : accès à une vaste bibliothèque de classes

---

### 2. Quelle est la différence entre .NET Framework, .NET Core et .NET 5+ ?

- **.NET Framework** : version originale, uniquement Windows, dernière version 4.8, en mode maintenance
- **.NET Core** : version cross-platform (1.0-3.1), modulaire, performante, open-source
- **.NET 5/6/7/8+** : unification de .NET Framework et .NET Core, une seule plateforme pour tous les types d'applications, cross-platform, moderne

**En résumé :**
```
.NET Framework (Windows only) + .NET Core (cross-platform) = .NET 5+ (unified)
```

---

### 3. Qu'est-ce que le CLR (Common Language Runtime) ?

Le CLR est le moteur d'exécution de .NET qui :

- **Compile le code** : convertit le code IL (Intermediate Language) en code machine via le compilateur JIT (Just-In-Time)
- **Gère la mémoire** : garbage collection automatique
- **Assure la sécurité** : vérification des types, gestion des exceptions
- **Fournit des services** : threading, gestion des exceptions, sécurité

**Flux d'exécution :**
```
Code C# → Compilateur C# → IL (MSIL) → CLR/JIT → Code machine natif
```

---

## Types et Variables C# {#types-et-variables-csharp}

### 4. Quelle est la différence entre les types valeur et les types référence ?

**Types valeur (Value Types) :**
- Stockés sur la stack
- Contiennent directement la valeur
- Exemples : `int`, `double`, `bool`, `struct`, `enum`
- Copie par valeur

```csharp
int a = 10;
int b = a;  // b est une copie de a
b = 20;     // a reste 10
```

**Types référence (Reference Types) :**
- Stockés sur le heap
- La variable contient une référence (adresse mémoire)
- Exemples : `class`, `interface`, `delegate`, `string`, `array`
- Copie par référence

```csharp
List<int> list1 = new List<int> { 1, 2, 3 };
List<int> list2 = list1;  // list2 référence le même objet
list2.Add(4);             // list1 contient aussi 4
```

---

### 5. Qu'est-ce que le boxing et unboxing ?

- **Boxing** : conversion d'un type valeur en type référence (object)
- **Unboxing** : conversion inverse, d'un object vers un type valeur

```csharp
// Boxing
int valeur = 123;
object obj = valeur;  // Boxing automatique

// Unboxing
int nombre = (int)obj;  // Unboxing explicite avec cast

// Impact performance : éviter le boxing/unboxing excessif
// Utiliser des génériques à la place
List<int> nombres = new List<int>();  // Pas de boxing
```

---

### 6. Quelle est la différence entre `var`, `dynamic` et `object` ?

```csharp
// var : typage implicite à la compilation
var nom = "Alice";  // Le compilateur infère string
// nom = 123;  // ERREUR : nom est de type string

// dynamic : typage dynamique à l'exécution
dynamic valeur = "Alice";
valeur = 123;  // OK, vérification à l'exécution
valeur.UneMethodeInexistante();  // Compile mais erreur à l'exécution

// object : type de base de tous les types
object obj = "Alice";
// obj.ToUpper();  // ERREUR : nécessite un cast
string s = ((string)obj).ToUpper();  // OK
```

---

## Programmation Orientée Objet C# {#programmation-orientée-objet-csharp}

### 7. Expliquez les modificateurs d'accès en C#

```csharp
public class Exemple
{
    public int Public;           // Accessible partout
    private int Private;         // Accessible uniquement dans cette classe
    protected int Protected;     // Accessible dans cette classe et ses dérivées
    internal int Internal;       // Accessible dans le même assembly
    protected internal int ProtectedInternal;  // Protected OU Internal
    private protected int PrivateProtected;    // Protected ET Internal
}
```

---

### 8. Qu'est-ce qu'une propriété (Property) et pourquoi l'utiliser ?

Les propriétés encapsulent les champs avec des accesseurs get/set :

```csharp
public class Personne
{
    // Auto-property (recommandé)
    public string Nom { get; set; }

    // Property avec backing field
    private int _age;
    public int Age
    {
        get { return _age; }
        set
        {
            if (value >= 0)
                _age = value;
            else
                throw new ArgumentException("L'âge doit être positif");
        }
    }

    // Read-only property
    public string NomComplet { get; }

    // Init-only property (C# 9+)
    public string Email { get; init; }

    // Expression-bodied property
    public string Description => $"{Nom} a {Age} ans";
}

// Utilisation
var p = new Personne
{
    Nom = "Alice",
    Age = 25,
    Email = "alice@example.com"  // Seulement lors de l'initialisation
};
// p.Email = "nouveau@example.com";  // ERREUR avec init
```

---

### 9. Qu'est-ce qu'une classe abstraite et une interface ? Différences ?

**Classe abstraite :**
```csharp
public abstract class Animal
{
    // Peut avoir des champs
    protected string nom;

    // Méthode concrète
    public void Dormir()
    {
        Console.WriteLine("Zzz...");
    }

    // Méthode abstraite (doit être implémentée)
    public abstract void FaireDuBruit();
}

public class Chien : Animal
{
    public override void FaireDuBruit()
    {
        Console.WriteLine("Woof!");
    }
}
```

**Interface :**
```csharp
public interface IVolant
{
    void Voler();
    int Altitude { get; set; }

    // C# 8+ : méthodes par défaut
    void Atterrir()
    {
        Altitude = 0;
    }
}

public class Oiseau : Animal, IVolant
{
    public int Altitude { get; set; }

    public void Voler()
    {
        Console.WriteLine("Je vole!");
    }

    public override void FaireDuBruit()
    {
        Console.WriteLine("Cui cui!");
    }
}
```

**Différences clés :**
- Une classe peut hériter d'une seule classe abstraite mais implémenter plusieurs interfaces
- Classe abstraite peut avoir des champs, constructeurs, membres concrets
- Interface définit un contrat (que faire), classe abstraite peut définir un comportement (comment faire)

---

### 10. Qu'est-ce que le polymorphisme en C# ?

Le polymorphisme permet à un objet de prendre plusieurs formes :

```csharp
// Polymorphisme par héritage
public class Forme
{
    public virtual double CalculerAire()
    {
        return 0;
    }
}

public class Cercle : Forme
{
    public double Rayon { get; set; }

    public override double CalculerAire()
    {
        return Math.PI * Rayon * Rayon;
    }
}

public class Rectangle : Forme
{
    public double Largeur { get; set; }
    public double Hauteur { get; set; }

    public override double CalculerAire()
    {
        return Largeur * Hauteur;
    }
}

// Utilisation polymorphe
List<Forme> formes = new List<Forme>
{
    new Cercle { Rayon = 5 },
    new Rectangle { Largeur = 10, Hauteur = 20 }
};

foreach (var forme in formes)
{
    Console.WriteLine($"Aire : {forme.CalculerAire()}");
}
```

---

## LINQ et Collections C# {#linq-et-collections-csharp}

### 11. Qu'est-ce que LINQ et comment l'utiliser ?

LINQ (Language Integrated Query) permet d'interroger des collections de manière déclarative :

```csharp
List<int> nombres = new List<int> { 1, 2, 3, 4, 5, 6, 7, 8, 9, 10 };

// Syntaxe méthode (recommandée)
var pairs = nombres
    .Where(n => n % 2 == 0)
    .Select(n => n * 2)
    .OrderByDescending(n => n)
    .ToList();

// Syntaxe requête
var pairsQuery = (from n in nombres
                  where n % 2 == 0
                  orderby n descending
                  select n * 2).ToList();

// Opérations courantes
var premier = nombres.First();
var premierOuDefaut = nombres.FirstOrDefault(n => n > 100);
var existe = nombres.Any(n => n > 5);
var tousPositifs = nombres.All(n => n > 0);
var somme = nombres.Sum();
var moyenne = nombres.Average();
var max = nombres.Max();
```

---

### 12. Quelles sont les principales collections en C# ?

```csharp
// List<T> : liste dynamique (tableau redimensionnable)
List<string> liste = new List<string> { "a", "b", "c" };
liste.Add("d");

// Dictionary<TKey, TValue> : paires clé-valeur
Dictionary<string, int> ages = new Dictionary<string, int>
{
    ["Alice"] = 25,
    ["Bob"] = 30
};

// HashSet<T> : ensemble sans doublons
HashSet<int> ensemble = new HashSet<int> { 1, 2, 3, 2 };  // {1, 2, 3}

// Queue<T> : file FIFO
Queue<string> file = new Queue<string>();
file.Enqueue("premier");
string item = file.Dequeue();

// Stack<T> : pile LIFO
Stack<string> pile = new Stack<string>();
pile.Push("premier");
string top = pile.Pop();

// IEnumerable<T> : interface de base pour l'itération
IEnumerable<int> sequence = Enumerable.Range(1, 10);
```

---

## Programmation Asynchrone C# {#programmation-asynchrone-csharp}

### 13. Qu'est-ce que async/await et comment l'utiliser ?

`async`/`await` permet d'écrire du code asynchrone de manière synchrone :

```csharp
// Méthode asynchrone
public async Task<string> TelechargerDonneesAsync(string url)
{
    using (var client = new HttpClient())
    {
        // await libère le thread pendant l'attente
        string resultat = await client.GetStringAsync(url);
        return resultat;
    }
}

// Utilisation
public async Task TraiterDonneesAsync()
{
    try
    {
        string donnees = await TelechargerDonneesAsync("https://api.example.com");
        Console.WriteLine($"Reçu : {donnees.Length} caractères");
    }
    catch (HttpRequestException ex)
    {
        Console.WriteLine($"Erreur : {ex.Message}");
    }
}

// Multiples opérations asynchrones en parallèle
public async Task<(string, string)> TelechargerPlusieursFichiersAsync()
{
    var tache1 = TelechargerDonneesAsync("https://api1.com");
    var tache2 = TelechargerDonneesAsync("https://api2.com");

    await Task.WhenAll(tache1, tache2);

    return (tache1.Result, tache2.Result);
}
```

---

### 14. Quelle est la différence entre Task et Thread ?

```csharp
// Thread : niveau bas, contrôle manuel
Thread thread = new Thread(() =>
{
    Console.WriteLine("Sur un nouveau thread");
});
thread.Start();
thread.Join();  // Attendre la fin

// Task : abstraction de haut niveau, utilise le thread pool
Task task = Task.Run(() =>
{
    Console.WriteLine("Sur un thread du pool");
});
await task;  // Attendre de manière asynchrone

// Task avec retour de valeur
Task<int> taskAvecResultat = Task.Run(() =>
{
    return 42;
});
int resultat = await taskAvecResultat;
```

**Différences :**
- **Thread** : ressource lourde, contrôle fin, pas de retour de valeur facile
- **Task** : abstraction légère, intégrée avec async/await, retourne des valeurs, meilleure gestion des exceptions

---

## Gestion des Exceptions C# {#gestion-des-exceptions-csharp}

### 15. Comment gérer les exceptions en C# ?

```csharp
// try-catch-finally
try
{
    int resultat = 10 / 0;
}
catch (DivideByZeroException ex)
{
    Console.WriteLine($"Erreur spécifique : {ex.Message}");
}
catch (Exception ex)
{
    Console.WriteLine($"Erreur générale : {ex.Message}");
}
finally
{
    // Toujours exécuté
    Console.WriteLine("Nettoyage");
}

// Exception filters (C# 6+)
try
{
    // code
}
catch (HttpRequestException ex) when (ex.StatusCode == HttpStatusCode.NotFound)
{
    Console.WriteLine("Resource not found");
}

// Créer une exception personnalisée
public class BusinessException : Exception
{
    public BusinessException(string message) : base(message) { }
    public BusinessException(string message, Exception inner) : base(message, inner) { }
}

// Lancer une exception
throw new BusinessException("Règle métier violée");
```

---

## Questions Avancées C# {#questions-avancées-csharp}

### 16. Qu'est-ce qu'un delegate et un event ?

```csharp
// Delegate : pointeur de fonction typé
public delegate void NotificationHandler(string message);

public class Notificateur
{
    // Event basé sur le delegate
    public event NotificationHandler OnNotification;

    public void EnvoyerNotification(string message)
    {
        // Déclencher l'event
        OnNotification?.Invoke(message);
    }
}

// Utilisation
var notif = new Notificateur();
notif.OnNotification += (msg) => Console.WriteLine($"Reçu : {msg}");
notif.OnNotification += (msg) => Console.WriteLine($"Log : {msg}");
notif.EnvoyerNotification("Hello!");

// Delegates prédéfinis
Action<string> action = (s) => Console.WriteLine(s);
Func<int, int, int> addition = (a, b) => a + b;
Predicate<int> estPair = (n) => n % 2 == 0;
```

---

### 17. Qu'est-ce que la réflexion (Reflection) ?

La réflexion permet d'inspecter et manipuler les types à l'exécution :

```csharp
// Obtenir le type
Type type = typeof(string);
Type type2 = "Hello".GetType();

// Inspecter les membres
PropertyInfo[] proprietes = type.GetProperties();
MethodInfo[] methodes = type.GetMethods();

// Créer une instance dynamiquement
Type personneType = typeof(Personne);
object instance = Activator.CreateInstance(personneType);

// Appeler une méthode
MethodInfo methode = personneType.GetMethod("DireBonjour");
methode.Invoke(instance, null);

// Lire/écrire une propriété
PropertyInfo prop = personneType.GetProperty("Nom");
prop.SetValue(instance, "Alice");
string nom = (string)prop.GetValue(instance);
```

---

### 18. Qu'est-ce qu'un record en C# 9+ ?

Les records sont des types immuables pour les données :

```csharp
// Record simple
public record Personne(string Nom, int Age);

// Utilisation
var p1 = new Personne("Alice", 25);
var p2 = new Personne("Alice", 25);
Console.WriteLine(p1 == p2);  // true (égalité par valeur)

// Clonage avec modification
var p3 = p1 with { Age = 26 };

// Record avec corps
public record Employe(string Nom, int Age)
{
    public string Poste { get; init; }

    public void AfficherInfo()
    {
        Console.WriteLine($"{Nom}, {Age} ans, {Poste}");
    }
}
```

---

### 19. Qu'est-ce que le pattern matching ?

```csharp
// Switch expression (C# 8+)
public static string ObtenirType(object obj) => obj switch
{
    int i => $"Entier : {i}",
    string s => $"Chaîne : {s}",
    Personne { Age: >= 18 } => "Adulte",
    Personne p => $"Mineur : {p.Nom}",
    null => "Null",
    _ => "Type inconnu"
};

// Property pattern
public static decimal CalculerTarif(Personne p) => p switch
{
    { Age: < 12 } => 5.0m,
    { Age: >= 12 and < 65 } => 10.0m,
    { Age: >= 65 } => 7.0m,
    _ => 0
};

// Pattern avec when
public static string Categorie(int age) => age switch
{
    var a when a < 0 => "Invalide",
    < 13 => "Enfant",
    >= 13 and < 20 => "Adolescent",
    >= 20 => "Adulte"
};
```

---

### 20. Qu'est-ce que IDisposable et using ?

```csharp
// IDisposable pour libérer les ressources
public class Connexion : IDisposable
{
    private bool disposed = false;

    public void Dispose()
    {
        Dispose(true);
        GC.SuppressFinalize(this);
    }

    protected virtual void Dispose(bool disposing)
    {
        if (!disposed)
        {
            if (disposing)
            {
                // Libérer les ressources managées
            }
            // Libérer les ressources non-managées
            disposed = true;
        }
    }
}

// Using statement (appelle Dispose automatiquement)
using (var conn = new Connexion())
{
    // Utiliser la connexion
}  // Dispose appelé automatiquement

// Using declaration (C# 8+)
using var conn2 = new Connexion();
// Dispose appelé à la fin du scope
```

---
## Questions Fondamentales ASP.NET {#questions-fondamentales-aspnet}

### 1. Qu'est-ce que ASP.NET Core et quelles sont ses différences avec ASP.NET Framework ?

**ASP.NET Core** est un framework web cross-platform, open-source et performant pour construire des applications web modernes.

**Différences clés :**

| ASP.NET Framework | ASP.NET Core |
|-------------------|--------------|
| Windows uniquement | Cross-platform (Windows, Linux, macOS) |
| Monolithique | Modulaire |
| System.Web dépendant d'IIS | Indépendant du serveur web |
| .NET Framework | .NET Core/.NET 5+ |
| Configuration XML | Configuration code-first |

---

### 2. Qu'est-ce que le pipeline de requête ASP.NET Core ?

Le pipeline traite les requêtes HTTP via une séquence de middleware :

```csharp
public class Startup
{
    public void Configure(IApplicationBuilder app)
    {
        // Ordre important!
        app.UseHttpsRedirection();
        app.UseStaticFiles();
        app.UseRouting();
        app.UseAuthentication();
        app.UseAuthorization();
        app.UseEndpoints(endpoints =>
        {
            endpoints.MapControllers();
        });
    }
}
```

**Chaque middleware peut :**
- Traiter la requête
- Modifier la requête/réponse
- Passer au middleware suivant
- Court-circuiter le pipeline

---

## ASP.NET Core MVC {#aspnet-core-mvc}

### 3. Expliquez le pattern MVC dans ASP.NET Core

**MVC** : Model-View-Controller, sépare l'application en trois composants :

```csharp
// Model : données et logique métier
public class Produit
{
    public int Id { get; set; }
    public string Nom { get; set; }
    public decimal Prix { get; set; }
}

// Controller : traite les requêtes
public class ProduitController : Controller
{
    private readonly IProduitService _service;

    public ProduitController(IProduitService service)
    {
        _service = service;
    }

    // Action qui retourne une vue
    public IActionResult Index()
    {
        var produits = _service.ObtenirTous();
        return View(produits);
    }

    // Action POST
    [HttpPost]
    public IActionResult Creer(Produit produit)
    {
        if (ModelState.IsValid)
        {
            _service.Ajouter(produit);
            return RedirectToAction(nameof(Index));
        }
        return View(produit);
    }
}
```

**View (Razor) :**
```html
@model IEnumerable<Produit>

<h2>Liste des Produits</h2>
<table>
    @foreach (var produit in Model)
    {
        <tr>
            <td>@produit.Nom</td>
            <td>@produit.Prix €</td>
        </tr>
    }
</table>
```

---

### 4. Qu'est-ce que Razor Pages ?

Alternative à MVC pour les pages simples, combine controller et vue :

```csharp
// Pages/Produits/Index.cshtml.cs
public class IndexModel : PageModel
{
    private readonly IProduitService _service;

    public List<Produit> Produits { get; set; }

    public IndexModel(IProduitService service)
    {
        _service = service;
    }

    public void OnGet()
    {
        Produits = _service.ObtenirTous();
    }

    public IActionResult OnPost(Produit produit)
    {
        _service.Ajouter(produit);
        return RedirectToPage();
    }
}
```

---

## Web API ASP.NET {#web-api-aspnet}

### 5. Comment créer une Web API REST avec ASP.NET Core ?

```csharp
[ApiController]
[Route("api/[controller]")]
public class ProduitsController : ControllerBase
{
    private readonly IProduitService _service;

    public ProduitsController(IProduitService service)
    {
        _service = service;
    }

    // GET: api/produits
    [HttpGet]
    public ActionResult<IEnumerable<Produit>> Get()
    {
        return Ok(_service.ObtenirTous());
    }

    // GET: api/produits/5
    [HttpGet("{id}")]
    public ActionResult<Produit> Get(int id)
    {
        var produit = _service.ObtenirParId(id);
        if (produit == null)
            return NotFound();
        return Ok(produit);
    }

    // POST: api/produits
    [HttpPost]
    public ActionResult<Produit> Post([FromBody] Produit produit)
    {
        if (!ModelState.IsValid)
            return BadRequest(ModelState);

        _service.Ajouter(produit);
        return CreatedAtAction(nameof(Get), new { id = produit.Id }, produit);
    }

    // PUT: api/produits/5
    [HttpPut("{id}")]
    public IActionResult Put(int id, [FromBody] Produit produit)
    {
        if (id != produit.Id)
            return BadRequest();

        _service.Modifier(produit);
        return NoContent();
    }

    // DELETE: api/produits/5
    [HttpDelete("{id}")]
    public IActionResult Delete(int id)
    {
        _service.Supprimer(id);
        return NoContent();
    }
}
```

---

### 6. Comment gérer les erreurs dans une API ?

```csharp
// Middleware d'exception global
public class ExceptionMiddleware
{
    private readonly RequestDelegate _next;

    public ExceptionMiddleware(RequestDelegate next)
    {
        _next = next;
    }

    public async Task InvokeAsync(HttpContext context)
    {
        try
        {
            await _next(context);
        }
        catch (Exception ex)
        {
            await HandleExceptionAsync(context, ex);
        }
    }

    private static Task HandleExceptionAsync(HttpContext context, Exception ex)
    {
        context.Response.ContentType = "application/json";
        context.Response.StatusCode = ex switch
        {
            NotFoundException => StatusCodes.Status404NotFound,
            ValidationException => StatusCodes.Status400BadRequest,
            _ => StatusCodes.Status500InternalServerError
        };

        return context.Response.WriteAsJsonAsync(new
        {
            error = ex.Message,
            statusCode = context.Response.StatusCode
        });
    }
}

// Enregistrement dans Program.cs
app.UseMiddleware<ExceptionMiddleware>();
```

---

## Entity Framework Core {#entity-framework-core}

### 7. Qu'est-ce qu'Entity Framework Core ?

ORM (Object-Relational Mapper) pour .NET qui permet de travailler avec des bases de données via des objets C# :

```csharp
// DbContext
public class ApplicationDbContext : DbContext
{
    public DbSet<Produit> Produits { get; set; }
    public DbSet<Categorie> Categories { get; set; }

    public ApplicationDbContext(DbContextOptions<ApplicationDbContext> options)
        : base(options)
    {
    }

    protected override void OnModelCreating(ModelBuilder modelBuilder)
    {
        // Configuration fluente
        modelBuilder.Entity<Produit>()
            .HasOne(p => p.Categorie)
            .WithMany(c => c.Produits)
            .HasForeignKey(p => p.CategorieId);

        modelBuilder.Entity<Produit>()
            .Property(p => p.Prix)
            .HasPrecision(18, 2);
    }
}

// Entités
public class Produit
{
    public int Id { get; set; }
    [Required]
    [MaxLength(100)]
    public string Nom { get; set; }
    public decimal Prix { get; set; }
    public int CategorieId { get; set; }
    public Categorie Categorie { get; set; }
}
```

---

### 8. Comment utiliser EF Core (CRUD) ?

```csharp
public class ProduitService
{
    private readonly ApplicationDbContext _context;

    public ProduitService(ApplicationDbContext context)
    {
        _context = context;
    }

    // Create
    public async Task<Produit> AjouterAsync(Produit produit)
    {
        _context.Produits.Add(produit);
        await _context.SaveChangesAsync();
        return produit;
    }

    // Read
    public async Task<List<Produit>> ObtenirTousAsync()
    {
        return await _context.Produits
            .Include(p => p.Categorie)  // Eager loading
            .ToListAsync();
    }

    public async Task<Produit> ObtenirParIdAsync(int id)
    {
        return await _context.Produits
            .FirstOrDefaultAsync(p => p.Id == id);
    }

    // Update
    public async Task ModifierAsync(Produit produit)
    {
        _context.Entry(produit).State = EntityState.Modified;
        await _context.SaveChangesAsync();
    }

    // Delete
    public async Task SupprimerAsync(int id)
    {
        var produit = await _context.Produits.FindAsync(id);
        if (produit != null)
        {
            _context.Produits.Remove(produit);
            await _context.SaveChangesAsync();
        }
    }
}
```

---

## Middleware et Pipeline {#middleware-et-pipeline}

### 9. Comment créer un middleware personnalisé ?

```csharp
// Middleware de logging personnalisé
public class RequestLoggingMiddleware
{
    private readonly RequestDelegate _next;
    private readonly ILogger<RequestLoggingMiddleware> _logger;

    public RequestLoggingMiddleware(
        RequestDelegate next,
        ILogger<RequestLoggingMiddleware> logger)
    {
        _next = next;
        _logger = logger;
    }

    public async Task InvokeAsync(HttpContext context)
    {
        _logger.LogInformation($"Request: {context.Request.Method} {context.Request.Path}");

        await _next(context);

        _logger.LogInformation($"Response: {context.Response.StatusCode}");
    }
}

// Extension method
public static class MiddlewareExtensions
{
    public static IApplicationBuilder UseRequestLogging(this IApplicationBuilder builder)
    {
        return builder.UseMiddleware<RequestLoggingMiddleware>();
    }
}

// Utilisation dans Program.cs
app.UseRequestLogging();
```

---

## Sécurité et Authentification ASP.NET {#sécurité-et-authentification-aspnet}

### 10. Comment implémenter l'authentification JWT ?

```csharp
// Configuration dans Program.cs
builder.Services.AddAuthentication(JwtBearerDefaults.AuthenticationScheme)
    .AddJwtBearer(options =>
    {
        options.TokenValidationParameters = new TokenValidationParameters
        {
            ValidateIssuer = true,
            ValidateAudience = true,
            ValidateLifetime = true,
            ValidateIssuerSigningKey = true,
            ValidIssuer = builder.Configuration["Jwt:Issuer"],
            ValidAudience = builder.Configuration["Jwt:Audience"],
            IssuerSigningKey = new SymmetricSecurityKey(
                Encoding.UTF8.GetBytes(builder.Configuration["Jwt:Key"]))
        };
    });

// Service d'authentification
public class AuthService
{
    private readonly IConfiguration _config;

    public string GenerateToken(User user)
    {
        var securityKey = new SymmetricSecurityKey(
            Encoding.UTF8.GetBytes(_config["Jwt:Key"]));
        var credentials = new SigningCredentials(
            securityKey, SecurityAlgorithms.HmacSha256);

        var claims = new[]
        {
            new Claim(ClaimTypes.NameIdentifier, user.Id.ToString()),
            new Claim(ClaimTypes.Name, user.Email),
            new Claim(ClaimTypes.Role, user.Role)
        };

        var token = new JwtSecurityToken(
            issuer: _config["Jwt:Issuer"],
            audience: _config["Jwt:Audience"],
            claims: claims,
            expires: DateTime.Now.AddHours(3),
            signingCredentials: credentials);

        return new JwtSecurityTokenHandler().WriteToken(token);
    }
}

// Controller protégé
[Authorize]
[ApiController]
[Route("api/[controller]")]
public class SecureController : ControllerBase
{
    [HttpGet]
    [Authorize(Roles = "Admin")]
    public IActionResult GetSecureData()
    {
        return Ok("Données sécurisées");
    }
}
```

---

## Déploiement ASP.NET {#déploiement-aspnet}

### 11. Comment déployer une application ASP.NET Core ?

```bash
# Publication de l'application
dotnet publish -c Release -o ./publish

# Avec Docker
# Dockerfile
FROM mcr.microsoft.com/dotnet/aspnet:8.0 AS base
WORKDIR /app
EXPOSE 80

FROM mcr.microsoft.com/dotnet/sdk:8.0 AS build
WORKDIR /src
COPY ["MonApp.csproj", "./"]
RUN dotnet restore
COPY . .
RUN dotnet build -c Release -o /app/build

FROM build AS publish
RUN dotnet publish -c Release -o /app/publish

FROM base AS final
WORKDIR /app
COPY --from=publish /app/publish .
ENTRYPOINT ["dotnet", "MonApp.dll"]
```

---

## Questions Fondamentales HTML {#questions-fondamentales-html}

### 1. Qu'est-ce que HTML et HTML5 ?

**HTML** (HyperText Markup Language) est le langage de balisage standard pour créer des pages web.

**HTML5** est la dernière version majeure, introduisant :
- Nouvelles balises sémantiques (`<header>`, `<nav>`, `<article>`, `<section>`, `<footer>`)
- APIs modernes (Canvas, SVG, Geolocation, Web Storage)
- Support multimédia natif (`<video>`, `<audio>`)
- Formulaires améliorés (nouveaux types d'input)
- Suppression des éléments obsolètes (`<font>`, `<center>`)

---

### 2. Quelle est la structure de base d'un document HTML ?

```html
<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Description de la page">
    <title>Titre de la page</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <header>
        <h1>En-tête principal</h1>
        <nav>
            <ul>
                <li><a href="#section1">Section 1</a></li>
                <li><a href="#section2">Section 2</a></li>
            </ul>
        </nav>
    </header>

    <main>
        <article>
            <h2>Contenu principal</h2>
            <p>Paragraphe de texte.</p>
        </article>
    </main>

    <footer>
        <p>&copy; 2024 Mon Site</p>
    </footer>

    <script src="script.js"></script>
</body>
</html>
```

---

## Sémantique HTML5 {#sémantique-html5}

### 3. Quelles sont les principales balises sémantiques HTML5 ?

```html
<!-- Structure de page -->
<header>En-tête de la page ou d'une section</header>
<nav>Navigation principale</nav>
<main>Contenu principal unique de la page</main>
<article>Contenu autonome et réutilisable</article>
<section>Section thématique</section>
<aside>Contenu complémentaire</aside>
<footer>Pied de page</footer>

<!-- Contenu -->
<figure>
    <img src="image.jpg" alt="Description">
    <figcaption>Légende de l'image</figcaption>
</figure>

<time datetime="2024-01-15">15 janvier 2024</time>
<mark>Texte surligné</mark>
<details>
    <summary>Titre cliquable</summary>
    <p>Contenu dépliable</p>
</details>
```

**Avantages :**
- Meilleur SEO
- Accessibilité améliorée
- Code plus lisible et maintenable
- Structure logique claire

---

### 4. Différence entre `<div>` et `<span>` ?

```html
<!-- div : élément bloc -->
<div class="container">
    <p>Un div crée un nouveau bloc</p>
</div>

<!-- span : élément inline -->
<p>Un <span class="highlight">span</span> reste dans le flux du texte</p>
```

- `<div>` : conteneur générique de niveau bloc, prend toute la largeur
- `<span>` : conteneur générique inline, prend seulement l'espace nécessaire

---

## Formulaires HTML {#formulaires-html}

### 5. Comment créer des formulaires HTML5 avec validation ?

```html
<form action="/submit" method="POST">
    <!-- Input text avec validation -->
    <label for="nom">Nom :</label>
    <input type="text" id="nom" name="nom" 
           required minlength="2" maxlength="50"
           placeholder="Votre nom">

    <!-- Email avec validation -->
    <label for="email">Email :</label>
    <input type="email" id="email" name="email" required>

    <!-- Nombre avec min/max -->
    <label for="age">Âge :</label>
    <input type="number" id="age" name="age" 
           min="18" max="100" required>

    <!-- Date -->
    <input type="date" name="dateNaissance">

    <!-- Téléphone -->
    <input type="tel" pattern="[0-9]{10}" placeholder="0612345678">

    <!-- URL -->
    <input type="url" placeholder="https://example.com">

    <!-- Mot de passe -->
    <input type="password" minlength="8" required>

    <!-- Select -->
    <select name="pays" required>
        <option value="">Choisissez un pays</option>
        <option value="fr">France</option>
        <option value="be">Belgique</option>
    </select>

    <!-- Textarea -->
    <textarea name="message" rows="4" maxlength="500"></textarea>

    <!-- Checkbox -->
    <input type="checkbox" id="conditions" required>
    <label for="conditions">J'accepte les conditions</label>

    <!-- Radio -->
    <input type="radio" id="homme" name="genre" value="H">
    <label for="homme">Homme</label>
    <input type="radio" id="femme" name="genre" value="F">
    <label for="femme">Femme</label>

    <!-- Submit -->
    <button type="submit">Envoyer</button>
</form>
```

---

## Accessibilité HTML {#accessibilité-html}

### 6. Comment rendre un site accessible ?

```html
<!-- Alt text pour les images -->
<img src="logo.png" alt="Logo de l'entreprise XYZ">

<!-- Labels pour les formulaires -->
<label for="email">Email :</label>
<input type="email" id="email" name="email">

<!-- ARIA (Accessible Rich Internet Applications) -->
<button aria-label="Fermer" aria-expanded="false">
    <span aria-hidden="true">×</span>
</button>

<nav aria-label="Navigation principale">
    <ul role="menubar">
        <li role="menuitem"><a href="/accueil">Accueil</a></li>
    </ul>
</nav>

<!-- Structure de titres logique -->
<h1>Titre principal (un seul par page)</h1>
    <h2>Sous-titre</h2>
        <h3>Sous-sous-titre</h3>

<!-- Skip links pour la navigation au clavier -->
<a href="#main-content" class="skip-link">Aller au contenu principal</a>

<!-- Lang attribute -->
<html lang="fr">
<p lang="en">This paragraph is in English</p>
```

**Principes WCAG :**
- **Perceptible** : contenu visible et audible
- **Utilisable** : navigable au clavier
- **Compréhensible** : texte lisible, comportement prévisible
- **Robuste** : compatible avec les technologies d'assistance

---

## SEO et Méta-données {#seo-et-méta-données}

### 7. Comment optimiser le SEO avec HTML ?

```html
<head>
    <!-- Title : 50-60 caractères -->
    <title>Guide HTML - Apprendre le développement web</title>

    <!-- Meta description : 150-160 caractères -->
    <meta name="description" content="Guide complet pour apprendre HTML5 avec des exemples pratiques et des bonnes pratiques SEO.">

    <!-- Meta keywords (moins important aujourd'hui) -->
    <meta name="keywords" content="HTML, HTML5, développement web, tutoriel">

    <!-- Viewport pour responsive -->
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <!-- Charset -->
    <meta charset="UTF-8">

    <!-- Open Graph (réseaux sociaux) -->
    <meta property="og:title" content="Guide HTML">
    <meta property="og:description" content="Guide complet HTML5">
    <meta property="og:image" content="https://example.com/image.jpg">
    <meta property="og:url" content="https://example.com/guide-html">
    <meta property="og:type" content="article">

    <!-- Twitter Card -->
    <meta name="twitter:card" content="summary_large_image">
    <meta name="twitter:title" content="Guide HTML">

    <!-- Canonical URL -->
    <link rel="canonical" href="https://example.com/guide-html">

    <!-- Favicon -->
    <link rel="icon" type="image/png" href="/favicon.png">
</head>

<body>
    <!-- Hiérarchie de titres -->
    <h1>Titre H1 unique avec mots-clés principaux</h1>
    <h2>Sous-titres H2 pour structurer le contenu</h2>

    <!-- Liens internes -->
    <a href="/autre-page">Texte d'ancre descriptif</a>

    <!-- Images avec alt -->
    <img src="image.jpg" alt="Description pertinente avec mots-clés">

    <!-- Schema.org / Structured Data -->
    <script type="application/ld+json">
    {
        "@context": "https://schema.org",
        "@type": "Article",
        "headline": "Guide HTML",
        "author": {
            "@type": "Person",
            "name": "John Doe"
        },
        "datePublished": "2024-01-15"
    }
    </script>
</body>
```

---

## Questions Fondamentales CSS {#questions-fondamentales-css}

### 1. Qu'est-ce que CSS et comment l'inclure dans HTML ?

**CSS** (Cascading Style Sheets) est le langage de style pour le web.

```html
<!-- 1. CSS Inline (éviter) -->
<p style="color: red; font-size: 16px;">Texte rouge</p>

<!-- 2. CSS Interne -->
<head>
    <style>
        p {
            color: blue;
            font-size: 14px;
        }
    </style>
</head>

<!-- 3. CSS Externe (recommandé) -->
<head>
    <link rel="stylesheet" href="styles.css">
</head>
```

---

### 2. Quelle est la différence entre class et id ?

```html
<!-- ID : unique, haute spécificité -->
<div id="header">En-tête unique</div>

<!-- Class : réutilisable, spécificité moyenne -->
<div class="card">Carte 1</div>
<div class="card">Carte 2</div>
<div class="card featured">Carte mise en avant</div>
```

```css
/* ID : #nom */
#header {
    background: blue;
}

/* Class : .nom */
.card {
    padding: 20px;
    border: 1px solid #ccc;
}

/* Multiple classes */
.card.featured {
    border-color: gold;
}
```

**Règles :**
- Un ID doit être unique dans la page
- Une classe peut être réutilisée
- Préférer les classes pour le styling

---

## Sélecteurs et Spécificité {#sélecteurs-et-spécificité}

### 3. Quels sont les différents types de sélecteurs CSS ?

```css
/* Sélecteur universel */
* {
    margin: 0;
    padding: 0;
}

/* Sélecteur de type */
p {
    color: black;
}

/* Sélecteur de classe */
.container {
    width: 100%;
}

/* Sélecteur d'ID */
#main {
    background: white;
}

/* Sélecteur d'attribut */
input[type="text"] {
    border: 1px solid #ccc;
}

a[href^="https"] {  /* commence par */
    color: green;
}

/* Sélecteurs combinés */
div p {  /* Descendant */
    color: red;
}

div > p {  /* Enfant direct */
    color: blue;
}

h2 + p {  /* Sibling adjacent */
    margin-top: 0;
}

h2 ~ p {  /* Tous les siblings suivants */
    color: gray;
}

/* Pseudo-classes */
a:hover {
    color: red;
}

li:first-child {
    font-weight: bold;
}

li:nth-child(odd) {
    background: #f0f0f0;
}

input:focus {
    outline: 2px solid blue;
}

/* Pseudo-éléments */
p::first-line {
    font-weight: bold;
}

p::before {
    content: "→ ";
}
```

---

### 4. Comment fonctionne la spécificité CSS ?

**Ordre de priorité (du plus au moins spécifique) :**

1. `!important` (à éviter sauf exception)
2. Styles inline
3. ID
4. Classes, attributs, pseudo-classes
5. Éléments, pseudo-éléments

```css
/* Spécificité : 0,0,0,1 */
p {
    color: black;
}

/* Spécificité : 0,0,1,1 */
p.intro {
    color: blue;
}

/* Spécificité : 0,1,0,1 */
#main p {
    color: red;
}

/* Spécificité : 0,1,1,1 */
#main p.intro {
    color: green;  /* Celui-ci gagne */
}

/* !important surcharge tout (à éviter) */
p {
    color: purple !important;
}
```

---

## Box Model et Layout {#box-model-et-layout}

### 5. Qu'est-ce que le Box Model CSS ?

Chaque élément HTML est une boîte composée de :

```css
.box {
    /* Contenu */
    width: 200px;
    height: 100px;

    /* Padding : espace intérieur */
    padding: 20px;

    /* Border : bordure */
    border: 2px solid black;

    /* Margin : espace extérieur */
    margin: 10px;
}

/* Box-sizing */
* {
    box-sizing: border-box;  /* width inclut padding et border */
}
```

**Calcul de la largeur totale :**
- `box-sizing: content-box` (défaut) : `width + padding + border + margin`
- `box-sizing: border-box` : `width` (inclut padding et border) + margin

---

### 6. Quelle est la différence entre display: block, inline et inline-block ?

```css
/* block : prend toute la largeur, nouvelle ligne */
div, p, h1 {
    display: block;
    width: 100%;
}

/* inline : dans le flux du texte, width/height ignorés */
span, a, strong {
    display: inline;
}

/* inline-block : hybride, dans le flux mais accepte width/height */
.button {
    display: inline-block;
    width: 150px;
    height: 40px;
    padding: 10px;
}

/* none : élément caché et retiré du flux */
.hidden {
    display: none;
}
```

---

## Flexbox {#flexbox}

### 7. Comment utiliser Flexbox pour le layout ?

```css
/* Conteneur flex */
.container {
    display: flex;

    /* Direction */
    flex-direction: row;  /* row | row-reverse | column | column-reverse */

    /* Alignement horizontal (axe principal) */
    justify-content: center;  /* flex-start | flex-end | center | space-between | space-around | space-evenly */

    /* Alignement vertical (axe secondaire) */
    align-items: center;  /* flex-start | flex-end | center | baseline | stretch */

    /* Retour à la ligne */
    flex-wrap: wrap;  /* nowrap | wrap | wrap-reverse */

    /* Espacement entre les éléments */
    gap: 20px;
}

/* Items flex */
.item {
    /* Facteur de croissance */
    flex-grow: 1;

    /* Facteur de rétrécissement */
    flex-shrink: 1;

    /* Taille de base */
    flex-basis: 200px;

    /* Raccourci : flex: grow shrink basis */
    flex: 1 1 200px;

    /* Alignement individuel */
    align-self: flex-end;
}
```

**Exemple pratique :**
```css
/* Layout horizontal centré */
.nav {
    display: flex;
    justify-content: space-between;
    align-items: center;
}

/* Grid de cartes responsive */
.card-container {
    display: flex;
    flex-wrap: wrap;
    gap: 20px;
}

.card {
    flex: 1 1 300px;  /* Cartes flexibles, min 300px */
}
```

---

## CSS Grid {#css-grid}

### 8. Comment utiliser CSS Grid ?

```css
/* Conteneur grid */
.grid-container {
    display: grid;

    /* Définir les colonnes */
    grid-template-columns: 200px 1fr 200px;  /* 3 colonnes */
    /* ou */
    grid-template-columns: repeat(3, 1fr);  /* 3 colonnes égales */
    /* ou */
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));  /* Responsive */

    /* Définir les lignes */
    grid-template-rows: auto 1fr auto;

    /* Espacement */
    gap: 20px;
    /* ou séparément */
    row-gap: 20px;
    column-gap: 10px;

    /* Zones nommées */
    grid-template-areas:
        "header header header"
        "sidebar main main"
        "footer footer footer";
}

/* Items grid */
.header {
    grid-area: header;
}

.sidebar {
    grid-area: sidebar;
}

.main {
    grid-area: main;
}

/* Positionnement manuel */
.item {
    grid-column: 1 / 3;  /* De la colonne 1 à 3 */
    grid-row: 2 / 4;     /* De la ligne 2 à 4 */
    /* ou */
    grid-column: span 2;  /* S'étend sur 2 colonnes */
}
```

**Exemple pratique :**
```css
/* Layout de page */
.page-layout {
    display: grid;
    grid-template-columns: 250px 1fr;
    grid-template-rows: 60px 1fr 40px;
    min-height: 100vh;
    gap: 20px;
}

/* Grid responsive de cartes */
.cards {
    display: grid;
    grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
    gap: 20px;
}
```

---

## Responsive Design {#responsive-design}

### 9. Comment créer un design responsive ?

```css
/* Mobile-first approach */
.container {
    width: 100%;
    padding: 15px;
}

/* Tablet */
@media (min-width: 768px) {
    .container {
        max-width: 720px;
        margin: 0 auto;
    }
}

/* Desktop */
@media (min-width: 1024px) {
    .container {
        max-width: 960px;
    }

    .grid {
        display: grid;
        grid-template-columns: repeat(3, 1fr);
    }
}

/* Large desktop */
@media (min-width: 1200px) {
    .container {
        max-width: 1140px;
    }
}

/* Responsive images */
img {
    max-width: 100%;
    height: auto;
}

/* Responsive typography */
html {
    font-size: 16px;
}

@media (max-width: 768px) {
    html {
        font-size: 14px;
    }
}

/* Unités relatives */
.card {
    width: 90vw;  /* 90% de la largeur du viewport */
    max-width: 600px;
    padding: 2rem;  /* Relatif au font-size racine */
}
```

---

## Animations et Transitions {#animations-et-transitions}

### 10. Comment créer des animations CSS ?

```css
/* Transitions : changements fluides */
.button {
    background: blue;
    transition: all 0.3s ease;
    /* ou spécifique */
    transition: background-color 0.3s ease, transform 0.2s;
}

.button:hover {
    background: darkblue;
    transform: scale(1.05);
}

/* Animations : séquences complexes */
@keyframes fadeIn {
    from {
        opacity: 0;
        transform: translateY(20px);
    }
    to {
        opacity: 1;
        transform: translateY(0);
    }
}

.element {
    animation: fadeIn 0.5s ease forwards;
}

/* Animation avec étapes */
@keyframes slide {
    0% {
        transform: translateX(0);
    }
    50% {
        transform: translateX(100px);
    }
    100% {
        transform: translateX(0);
    }
}

.slider {
    animation: slide 2s infinite ease-in-out;
}

/* Transform */
.card:hover {
    transform: rotate(5deg) scale(1.1);
}
```

---

## Préprocesseurs CSS {#préprocesseurs-css}

### 11. Qu'est-ce qu'un préprocesseur CSS (Sass/SCSS) ?

```scss
// Variables
$primary-color: #3498db;
$secondary-color: #2ecc71;
$spacing: 20px;

// Nesting
.nav {
    background: $primary-color;
    padding: $spacing;

    ul {
        list-style: none;

        li {
            display: inline-block;

            a {
                color: white;

                &:hover {  // & = parent selector
                    text-decoration: underline;
                }
            }
        }
    }
}

// Mixins (fonctions réutilisables)
@mixin flexCenter {
    display: flex;
    justify-content: center;
    align-items: center;
}

.container {
    @include flexCenter;
}

// Mixin avec paramètres
@mixin button($bg-color) {
    background: $bg-color;
    padding: 10px 20px;
    border: none;
    border-radius: 4px;

    &:hover {
        background: darken($bg-color, 10%);
    }
}

.btn-primary {
    @include button($primary-color);
}

// Extend
%card-base {
    padding: 20px;
    border-radius: 8px;
    box-shadow: 0 2px 4px rgba(0,0,0,0.1);
}

.card {
    @extend %card-base;
    background: white;
}

// Functions
@function calculate-rem($px) {
    @return #{$px / 16}rem;
}

.text {
    font-size: calculate-rem(18);  // 1.125rem
}
```

---

## Questions Fondamentales TypeScript {#questions-fondamentales-typescript}

### 1. Qu'est-ce que TypeScript et pourquoi l'utiliser ?

**TypeScript** est un superset de JavaScript qui ajoute le typage statique.

**Avantages :**
- Détection d'erreurs à la compilation
- IntelliSense et autocomplétion améliorés
- Refactoring plus sûr
- Documentation via les types
- Meilleure maintenabilité du code

```typescript
// JavaScript
function additionner(a, b) {
    return a + b;
}
additionner(5, "10");  // "510" - comportement inattendu

// TypeScript
function additionner(a: number, b: number): number {
    return a + b;
}
additionner(5, "10");  // ERREUR à la compilation
```

---

### 2. Comment configurer TypeScript (tsconfig.json) ?

```json
{
    "compilerOptions": {
        "target": "ES2020",
        "module": "commonjs",
        "lib": ["ES2020", "DOM"],
        "outDir": "./dist",
        "rootDir": "./src",
        "strict": true,
        "esModuleInterop": true,
        "skipLibCheck": true,
        "forceConsistentCasingInFileNames": true,
        "resolveJsonModule": true,
        "declaration": true,
        "sourceMap": true
    },
    "include": ["src/**/*"],
    "exclude": ["node_modules", "dist"]
}
```

---

## Types et Interfaces TypeScript {#types-et-interfaces-typescript}

### 3. Quels sont les types de base en TypeScript ?

```typescript
// Types primitifs
let nom: string = "Alice";
let age: number = 25;
let estActif: boolean = true;
let valeur: null = null;
let indefini: undefined = undefined;

// Any (à éviter)
let nimporteQuoi: any = "texte";
nimporteQuoi = 123;

// Unknown (plus sûr que any)
let inconnu: unknown = "texte";
if (typeof inconnu === "string") {
    console.log(inconnu.toUpperCase());
}

// Void
function logger(): void {
    console.log("Log");
}

// Never (fonction qui ne retourne jamais)
function erreur(message: string): never {
    throw new Error(message);
}

// Arrays
let nombres: number[] = [1, 2, 3];
let noms: Array<string> = ["Alice", "Bob"];

// Tuple
let personne: [string, number] = ["Alice", 25];

// Enum
enum Couleur {
    Rouge = "RED",
    Vert = "GREEN",
    Bleu = "BLUE"
}
let couleur: Couleur = Couleur.Rouge;

// Object
let utilisateur: {
    nom: string;
    age: number;
    email?: string;  // Optionnel
} = {
    nom: "Alice",
    age: 25
};
```

---

### 4. Quelle est la différence entre interface et type ?

```typescript
// Interface : pour les objets et classes
interface Utilisateur {
    id: number;
    nom: string;
    email: string;
    age?: number;
}

// Extension d'interface
interface Admin extends Utilisateur {
    role: string;
    permissions: string[];
}

// Type : plus flexible
type ID = number | string;

type Point = {
    x: number;
    y: number;
};

// Union types
type Resultat = Success | Error;

// Intersection types
type PersonneAvecAdresse = Personne & Adresse;

// Type alias pour fonctions
type Operation = (a: number, b: number) => number;

const addition: Operation = (a, b) => a + b;
```

**Différences :**
- Interface : peut être étendue et fusionnée (declaration merging)
- Type : supporte unions, intersections, tuples, plus flexible
- Préférer **interface** pour les objets, **type** pour les unions/intersections

---

### 5. Comment typer des fonctions ?

```typescript
// Fonction simple
function saluer(nom: string): string {
    return `Bonjour ${nom}`;
}

// Paramètres optionnels
function creerUtilisateur(nom: string, age?: number): Utilisateur {
    return { nom, age: age || 0 };
}

// Paramètres par défaut
function multiplier(a: number, b: number = 1): number {
    return a * b;
}

// Rest parameters
function somme(...nombres: number[]): number {
    return nombres.reduce((acc, n) => acc + n, 0);
}

// Fonction comme type
type OperationMath = (a: number, b: number) => number;

const diviser: OperationMath = (a, b) => a / b;

// Overloading
function formater(valeur: string): string;
function formater(valeur: number): string;
function formater(valeur: string | number): string {
    if (typeof valeur === "number") {
        return valeur.toFixed(2);
    }
    return valeur.toUpperCase();
}

// Arrow function
const doubler = (n: number): number => n * 2;

// Callback
function traiterAsync(callback: (resultat: string) => void): void {
    callback("Terminé");
}
```

---

## Generics TypeScript {#generics-typescript}

### 6. Comment utiliser les Generics ?

```typescript
// Generic function
function identity<T>(arg: T): T {
    return arg;
}

const nombre = identity<number>(42);
const texte = identity("hello");  // Type inféré

// Generic avec contraintes
function afficherLongueur<T extends { length: number }>(item: T): number {
    return item.length;
}

afficherLongueur("hello");  // OK
afficherLongueur([1, 2, 3]);  // OK
// afficherLongueur(123);  // ERREUR

// Generic interface
interface Response<T> {
    data: T;
    status: number;
    message: string;
}

const userResponse: Response<Utilisateur> = {
    data: { id: 1, nom: "Alice", email: "alice@example.com" },
    status: 200,
    message: "Success"
};

// Generic class
class DataStore<T> {
    private data: T[] = [];

    add(item: T): void {
        this.data.push(item);
    }

    get(index: number): T | undefined {
        return this.data[index];
    }

    getAll(): T[] {
        return [...this.data];
    }
}

const numberStore = new DataStore<number>();
numberStore.add(42);

// Multiple generic types
function pair<T, U>(first: T, second: U): [T, U] {
    return [first, second];
}

const result = pair<string, number>("age", 25);
```

---

## Types Avancés TypeScript {#types-avancés-typescript}

### 7. Quels sont les types avancés en TypeScript ?

```typescript
// Union types
type Resultat = "success" | "error" | "pending";
let status: Resultat = "success";

// Intersection types
type Personne = { nom: string };
type Employe = { entreprise: string };
type PersonneEmploye = Personne & Employe;

const employe: PersonneEmploye = {
    nom: "Alice",
    entreprise: "TechCorp"
};

// Literal types
type Direction = "nord" | "sud" | "est" | "ouest";
let direction: Direction = "nord";

// Type guards
function estString(valeur: unknown): valeur is string {
    return typeof valeur === "string";
}

// Mapped types
type Readonly<T> = {
    readonly [P in keyof T]: T[P];
};

type Partial<T> = {
    [P in keyof T]?: T[P];
};

// Utility types
interface Utilisateur {
    id: number;
    nom: string;
    email: string;
    age: number;
}

// Partial : tous les champs optionnels
type UtilisateurPartiel = Partial<Utilisateur>;

// Required : tous les champs requis
type UtilisateurRequis = Required<Utilisateur>;

// Pick : sélectionner certains champs
type UtilisateurPublic = Pick<Utilisateur, "nom" | "email">;

// Omit : exclure certains champs
type UtilisateurSansId = Omit<Utilisateur, "id">;

// Record : créer un objet avec clés et valeurs typées
type Roles = Record<string, string[]>;
const roles: Roles = {
    admin: ["read", "write", "delete"],
    user: ["read"]
};

// Conditional types
type IsString<T> = T extends string ? true : false;
type Test1 = IsString<string>;  // true
type Test2 = IsString<number>;  // false

// Template literal types
type EmailLocale = "en" | "fr" | "es";
type EmailKey = `email_${EmailLocale}`;
// "email_en" | "email_fr" | "email_es"
```

---

## Décorateurs TypeScript {#décorateurs-typescript}

### 8. Qu'est-ce qu'un décorateur et comment l'utiliser ?

```typescript
// Activer dans tsconfig.json
// "experimentalDecorators": true

// Class decorator
function sealed(constructor: Function) {
    Object.seal(constructor);
    Object.seal(constructor.prototype);
}

@sealed
class MaClasse {
    // ...
}

// Method decorator
function log(target: any, propertyKey: string, descriptor: PropertyDescriptor) {
    const originalMethod = descriptor.value;

    descriptor.value = function (...args: any[]) {
        console.log(`Appel de ${propertyKey} avec`, args);
        const result = originalMethod.apply(this, args);
        console.log(`Résultat:`, result);
        return result;
    };

    return descriptor;
}

class Calculator {
    @log
    add(a: number, b: number): number {
        return a + b;
    }
}

// Property decorator
function readonly(target: any, propertyKey: string) {
    Object.defineProperty(target, propertyKey, {
        writable: false
    });
}

class Person {
    @readonly
    name: string = "Alice";
}

// Parameter decorator
function required(target: any, propertyKey: string, parameterIndex: number) {
    console.log(`Paramètre ${parameterIndex} de ${propertyKey} est requis`);
}

class Greeter {
    greet(@required name: string) {
        return `Hello ${name}`;
    }
}
```

---

## TypeScript avec React {#typescript-avec-react}

### 9. Comment utiliser TypeScript avec React ?

```typescript
import React, { useState, useEffect, FC, ReactNode } from 'react';

// Props interface
interface ButtonProps {
    text: string;
    onClick: () => void;
    disabled?: boolean;
    children?: ReactNode;
}

// Functional Component
const Button: FC<ButtonProps> = ({ text, onClick, disabled = false }) => {
    return (
        <button onClick={onClick} disabled={disabled}>
            {text}
        </button>
    );
};

// Component avec useState
interface User {
    id: number;
    name: string;
    email: string;
}

const UserProfile: FC = () => {
    const [user, setUser] = useState<User | null>(null);
    const [loading, setLoading] = useState<boolean>(false);

    useEffect(() => {
        fetchUser();
    }, []);

    const fetchUser = async (): Promise<void> => {
        setLoading(true);
        try {
            const response = await fetch('/api/user');
            const data: User = await response.json();
            setUser(data);
        } catch (error) {
            console.error(error);
        } finally {
            setLoading(false);
        }
    };

    if (loading) return <div>Loading...</div>;
    if (!user) return <div>No user</div>;

    return (
        <div>
            <h1>{user.name}</h1>
            <p>{user.email}</p>
        </div>
    );
};

// Event handlers
interface FormProps {
    onSubmit: (data: FormData) => void;
}

interface FormData {
    email: string;
    password: string;
}

const LoginForm: FC<FormProps> = ({ onSubmit }) => {
    const [formData, setFormData] = useState<FormData>({
        email: '',
        password: ''
    });

    const handleChange = (e: React.ChangeEvent<HTMLInputElement>): void => {
        const { name, value } = e.target;
        setFormData(prev => ({ ...prev, [name]: value }));
    };

    const handleSubmit = (e: React.FormEvent<HTMLFormElement>): void => {
        e.preventDefault();
        onSubmit(formData);
    };

    return (
        <form onSubmit={handleSubmit}>
            <input
                type="email"
                name="email"
                value={formData.email}
                onChange={handleChange}
            />
            <input
                type="password"
                name="password"
                value={formData.password}
                onChange={handleChange}
            />
            <button type="submit">Login</button>
        </form>
    );
};

// Generic component
interface ListProps<T> {
    items: T[];
    renderItem: (item: T) => ReactNode;
}

function List<T>({ items, renderItem }: ListProps<T>): JSX.Element {
    return (
        <ul>
            {items.map((item, index) => (
                <li key={index}>{renderItem(item)}</li>
            ))}
        </ul>
    );
}

// Utilisation
<List
    items={[1, 2, 3]}
    renderItem={(num) => <span>{num * 2}</span>}
/>
```

---

## Questions Fondamentales Docker {#questions-fondamentales-docker}

### 1. Qu'est-ce que Docker et pourquoi l'utiliser ?

**Docker** est une plateforme de conteneurisation qui permet d'empaqueter une application avec toutes ses dépendances.

**Avantages :**
- **Portabilité** : "fonctionne sur ma machine" → fonctionne partout
- **Isolation** : chaque conteneur est isolé
- **Léger** : plus rapide que les VM (pas de système d'exploitation complet)
- **Reproductibilité** : même environnement en dev, test et prod
- **Scalabilité** : facile de multiplier les instances

**Concepts clés :**
- **Image** : template en lecture seule (blueprint)
- **Conteneur** : instance en cours d'exécution d'une image
- **Dockerfile** : fichier de recette pour créer une image
- **Docker Hub** : registry public d'images

---

### 2. Quelle est la différence entre une image et un conteneur ?

```bash
# Image : template statique
docker images                    # Lister les images
docker pull nginx:latest         # Télécharger une image

# Conteneur : instance en cours d'exécution
docker ps                        # Lister les conteneurs actifs
docker ps -a                     # Tous les conteneurs
docker run nginx                 # Créer et démarrer un conteneur

# Analogie
# Image = Classe
# Conteneur = Instance d'objet
```

---

## Images et Conteneurs {#images-et-conteneurs}

### 3. Quelles sont les commandes Docker de base ?

```bash
# Images
docker pull <image>              # Télécharger une image
docker images                    # Lister les images
docker rmi <image>               # Supprimer une image
docker build -t <name> .         # Construire une image

# Conteneurs
docker run <image>               # Créer et démarrer
docker run -d <image>            # En arrière-plan (detached)
docker run -p 8080:80 <image>    # Mapper les ports (host:container)
docker run --name mon-app <image>  # Nommer le conteneur
docker run -v /host:/container <image>  # Monter un volume

docker ps                        # Conteneurs actifs
docker ps -a                     # Tous les conteneurs
docker start <container>         # Démarrer
docker stop <container>          # Arrêter
docker restart <container>       # Redémarrer
docker rm <container>            # Supprimer
docker logs <container>          # Voir les logs
docker logs -f <container>       # Suivre les logs en temps réel
docker exec -it <container> bash # Entrer dans le conteneur

# Nettoyage
docker system prune              # Nettoyer les ressources inutilisées
docker container prune           # Supprimer conteneurs arrêtés
docker image prune               # Supprimer images non utilisées
docker volume prune              # Supprimer volumes non utilisés
```

---

## Dockerfile {#dockerfile}

### 4. Comment créer un Dockerfile ?

```dockerfile
# Dockerfile pour une app Node.js

# Image de base
FROM node:18-alpine

# Métadonnées
LABEL maintainer="dev@example.com"
LABEL version="1.0"

# Créer le répertoire de travail
WORKDIR /app

# Copier package.json et package-lock.json
COPY package*.json ./

# Installer les dépendances
RUN npm ci --only=production

# Copier le code source
COPY . .

# Exposer le port
EXPOSE 3000

# Variables d'environnement
ENV NODE_ENV=production

# Utilisateur non-root (sécurité)
USER node

# Commande de démarrage
CMD ["node", "server.js"]
```

**Dockerfile multi-stage (optimisé) :**
```dockerfile
# Stage 1: Build
FROM node:18-alpine AS builder
WORKDIR /app
COPY package*.json ./
RUN npm ci
COPY . .
RUN npm run build

# Stage 2: Production
FROM node:18-alpine
WORKDIR /app
COPY --from=builder /app/dist ./dist
COPY --from=builder /app/node_modules ./node_modules
COPY package*.json ./
EXPOSE 3000
USER node
CMD ["node", "dist/server.js"]
```

**Dockerfile pour app Python :**
```dockerfile
FROM python:3.11-slim

WORKDIR /app

COPY requirements.txt .
RUN pip install --no-cache-dir -r requirements.txt

COPY . .

EXPOSE 8000

CMD ["python", "app.py"]
```

---

### 5. Quelles sont les bonnes pratiques pour un Dockerfile ?

```dockerfile
# ✅ Utiliser des images officielles et légères
FROM node:18-alpine

# ✅ Ordre optimal (du moins au plus changeant)
WORKDIR /app
COPY package*.json ./           # Dépendances d'abord
RUN npm ci
COPY . .                        # Code source après

# ✅ Minimiser les layers
RUN apt-get update && \
    apt-get install -y curl vim && \
    apt-get clean && \
    rm -rf /var/lib/apt/lists/*

# ✅ .dockerignore pour exclure des fichiers
# node_modules
# .git
# *.log

# ✅ Multi-stage pour images plus petites
FROM node:18 AS builder
# ... build steps ...
FROM node:18-alpine
COPY --from=builder /app/dist ./dist

# ✅ Ne pas run en tant que root
USER node

# ✅ Utiliser COPY au lieu de ADD
COPY . .

# ✅ Spécifier des versions exactes
FROM node:18.17.0-alpine

# ✅ Health check
HEALTHCHECK --interval=30s --timeout=3s \
    CMD curl -f http://localhost:3000/health || exit 1
```

---

## Docker Compose {#docker-compose}

### 6. Qu'est-ce que Docker Compose et comment l'utiliser ?

Docker Compose permet de définir et gérer des applications multi-conteneurs :

```yaml
# docker-compose.yml
version: '3.8'

services:
  # Application web
  web:
    build: .
    ports:
      - "3000:3000"
    environment:
      - NODE_ENV=production
      - DATABASE_URL=postgresql://user:pass@db:5432/mydb
    depends_on:
      - db
      - redis
    volumes:
      - ./src:/app/src
    networks:
      - app-network

  # Base de données PostgreSQL
  db:
    image: postgres:15-alpine
    environment:
      POSTGRES_USER: user
      POSTGRES_PASSWORD: pass
      POSTGRES_DB: mydb
    ports:
      - "5432:5432"
    volumes:
      - postgres-data:/var/lib/postgresql/data
    networks:
      - app-network

  # Redis cache
  redis:
    image: redis:7-alpine
    ports:
      - "6379:6379"
    networks:
      - app-network

  # Nginx reverse proxy
  nginx:
    image: nginx:alpine
    ports:
      - "80:80"
    volumes:
      - ./nginx.conf:/etc/nginx/nginx.conf
    depends_on:
      - web
    networks:
      - app-network

volumes:
  postgres-data:

networks:
  app-network:
    driver: bridge
```

**Commandes Docker Compose :**
```bash
docker-compose up                 # Démarrer tous les services
docker-compose up -d              # En arrière-plan
docker-compose down               # Arrêter et supprimer
docker-compose down -v            # Inclure les volumes
docker-compose ps                 # Statut des services
docker-compose logs               # Logs de tous les services
docker-compose logs -f web        # Suivre les logs du service web
docker-compose exec web bash      # Entrer dans le conteneur
docker-compose build              # Rebuild les images
docker-compose restart            # Redémarrer les services
```

---

## Réseaux et Volumes Docker {#réseaux-et-volumes-docker}

### 7. Comment gérer les réseaux et volumes Docker ?

**Volumes (persistance des données) :**
```bash
# Créer un volume
docker volume create mon-volume

# Lister les volumes
docker volume ls

# Utiliser un volume
docker run -v mon-volume:/app/data nginx

# Volume bind mount (lier un dossier local)
docker run -v /chemin/local:/app/data nginx

# Inspecter un volume
docker volume inspect mon-volume

# Supprimer un volume
docker volume rm mon-volume
```

**Réseaux :**
```bash
# Créer un réseau
docker network create mon-reseau

# Lister les réseaux
docker network ls

# Utiliser un réseau
docker run --network mon-reseau nginx

# Connecter un conteneur existant
docker network connect mon-reseau mon-conteneur

# Inspecter un réseau
docker network inspect mon-reseau

# Types de réseaux
# - bridge (défaut) : réseau isolé
# - host : utilise le réseau de l'hôte
# - none : pas de réseau
```

---

## Optimisation Docker {#optimisation-docker}

### 8. Comment optimiser les images Docker ?

```dockerfile
# ❌ Image non optimisée (1GB+)
FROM ubuntu:latest
RUN apt-get update
RUN apt-get install -y python3
RUN apt-get install -y pip
COPY . .
CMD ["python3", "app.py"]

# ✅ Image optimisée (50MB)
FROM python:3.11-alpine
WORKDIR /app
COPY requirements.txt .
RUN pip install --no-cache-dir -r requirements.txt
COPY . .
CMD ["python", "app.py"]

# ✅ Multi-stage pour encore plus petit
FROM python:3.11 AS builder
WORKDIR /app
COPY requirements.txt .
RUN pip install --user -r requirements.txt

FROM python:3.11-alpine
WORKDIR /app
COPY --from=builder /root/.local /root/.local
COPY . .
ENV PATH=/root/.local/bin:$PATH
CMD ["python", "app.py"]
```

**Techniques d'optimisation :**
- Utiliser des images Alpine (petites)
- Multi-stage builds
- Mettre en cache les layers (ordre optimal)
- Minimiser le nombre de layers (combiner RUN)
- Utiliser .dockerignore
- Ne pas inclure les outils de build dans l'image finale

---

## Concepts Fondamentaux DevOps {#concepts-fondamentaux-devops}

### 1. Qu'est-ce que DevOps ?

**DevOps** est une culture et un ensemble de pratiques qui combinent le développement (Dev) et les opérations (Ops).

**Principes clés :**
- **Collaboration** : Dev et Ops travaillent ensemble
- **Automatisation** : CI/CD, IaC, tests automatisés
- **Monitoring** : surveillance continue de la production
- **Feedback rapide** : déploiements fréquents et itératifs
- **Amélioration continue** : apprendre des échecs

**Bénéfices :**
- Déploiements plus rapides et fréquents
- Réduction des erreurs
- Meilleure qualité du code
- Time-to-market réduit

---

### 2. Qu'est-ce que CI/CD ?

**CI (Continuous Integration)** : intégration continue du code
**CD (Continuous Delivery/Deployment)** : livraison/déploiement continu

```
Code Push → Tests automatiques → Build → Tests d'intégration → Déploiement staging → Tests E2E → Déploiement production
```

---

## CI/CD {#cicd}

### 3. Comment mettre en place un pipeline CI/CD ?

**Exemple avec GitHub Actions :**
```yaml
# .github/workflows/ci-cd.yml
name: CI/CD Pipeline

on:
  push:
    branches: [main, develop]
  pull_request:
    branches: [main]

jobs:
  test:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v3

      - name: Setup Node.js
        uses: actions/setup-node@v3
        with:
          node-version: '18'
          cache: 'npm'

      - name: Install dependencies
        run: npm ci

      - name: Run linter
        run: npm run lint

      - name: Run tests
        run: npm test

      - name: Run coverage
        run: npm run test:coverage

  build:
    needs: test
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v3

      - name: Build Docker image
        run: docker build -t myapp:${{ github.sha }} .

      - name: Push to registry
        run: |
          echo ${{ secrets.DOCKER_PASSWORD }} | docker login -u ${{ secrets.DOCKER_USERNAME }} --password-stdin
          docker push myapp:${{ github.sha }}

  deploy:
    needs: build
    runs-on: ubuntu-latest
    if: github.ref == 'refs/heads/main'
    steps:
      - name: Deploy to production
        run: |
          # Commandes de déploiement
          kubectl set image deployment/myapp myapp=myapp:${{ github.sha }}
```

**Exemple avec GitLab CI :**
```yaml
# .gitlab-ci.yml
stages:
  - test
  - build
  - deploy

variables:
  DOCKER_IMAGE: registry.gitlab.com/$CI_PROJECT_PATH

test:
  stage: test
  image: node:18
  script:
    - npm ci
    - npm run lint
    - npm test
  coverage: '/Statements\s*:\s*(\d+\.\d+)%/'

build:
  stage: build
  image: docker:latest
  services:
    - docker:dind
  script:
    - docker build -t $DOCKER_IMAGE:$CI_COMMIT_SHA .
    - docker push $DOCKER_IMAGE:$CI_COMMIT_SHA
  only:
    - main

deploy:
  stage: deploy
  image: alpine:latest
  script:
    - apk add --no-cache curl
    - curl -X POST $DEPLOY_WEBHOOK
  only:
    - main
  environment:
    name: production
```

---

## Infrastructure as Code {#infrastructure-as-code}

### 4. Qu'est-ce que l'Infrastructure as Code (IaC) ?

Gestion de l'infrastructure via du code (version control, review, automatisation).

**Terraform :**
```hcl
# main.tf
terraform {
  required_providers {
    aws = {
      source  = "hashicorp/aws"
      version = "~> 5.0"
    }
  }
}

provider "aws" {
  region = "eu-west-1"
}

# VPC
resource "aws_vpc" "main" {
  cidr_block = "10.0.0.0/16"

  tags = {
    Name = "main-vpc"
  }
}

# EC2 Instance
resource "aws_instance" "web" {
  ami           = "ami-0c55b159cbfafe1f0"
  instance_type = "t2.micro"
  
  tags = {
    Name = "web-server"
  }
}

# S3 Bucket
resource "aws_s3_bucket" "storage" {
  bucket = "my-app-storage"

  versioning {
    enabled = true
  }
}
```

**Commandes Terraform :**
```bash
terraform init        # Initialiser
terraform plan        # Voir les changements
terraform apply       # Appliquer les changements
terraform destroy     # Détruire l'infrastructure
```

**Ansible (configuration management) :**
```yaml
# playbook.yml
- name: Configure web servers
  hosts: webservers
  become: yes
  tasks:
    - name: Install nginx
      apt:
        name: nginx
        state: present
        update_cache: yes

    - name: Start nginx
      service:
        name: nginx
        state: started
        enabled: yes

    - name: Copy website files
      copy:
        src: ./website/
        dest: /var/www/html/
```

---

## Monitoring et Logging {#monitoring-et-logging}

### 5. Comment mettre en place le monitoring ?

**Prometheus + Grafana :**
```yaml
# docker-compose.yml
version: '3.8'

services:
  prometheus:
    image: prom/prometheus
    ports:
      - "9090:9090"
    volumes:
      - ./prometheus.yml:/etc/prometheus/prometheus.yml
      - prometheus-data:/prometheus

  grafana:
    image: grafana/grafana
    ports:
      - "3000:3000"
    environment:
      - GF_SECURITY_ADMIN_PASSWORD=admin
    volumes:
      - grafana-data:/var/lib/grafana

  # Application avec métriques
  app:
    build: .
    ports:
      - "8080:8080"
    environment:
      - METRICS_ENABLED=true

volumes:
  prometheus-data:
  grafana-data:
```

**Prometheus config :**
```yaml
# prometheus.yml
global:
  scrape_interval: 15s

scrape_configs:
  - job_name: 'app'
    static_configs:
      - targets: ['app:8080']
```

**Logging avec ELK Stack :**
- **Elasticsearch** : stockage et recherche
- **Logstash** : collecte et traitement
- **Kibana** : visualisation

---

## Cloud Platforms {#cloud-platforms}

### 6. Quelles sont les principales plateformes cloud ?

**AWS (Amazon Web Services) :**
- EC2 : serveurs virtuels
- S3 : stockage objet
- RDS : bases de données managées
- Lambda : serverless functions
- ECS/EKS : orchestration de conteneurs

**Azure (Microsoft) :**
- Virtual Machines
- Blob Storage
- Azure SQL Database
- Azure Functions
- AKS : Kubernetes managé

**GCP (Google Cloud Platform) :**
- Compute Engine
- Cloud Storage
- Cloud SQL
- Cloud Functions
- GKE : Kubernetes managé

**Services communs :**
- Compute (VMs, conteneurs)
- Storage (objet, bloc, fichier)
- Databases (SQL, NoSQL)
- Networking (VPC, load balancers)
- Serverless (functions)

---

## Questions Fondamentales Git {#questions-fondamentales-git}

### 1. Qu'est-ce que Git ?

**Git** est un système de contrôle de version distribué.

**Avantages :**
- Historique complet des modifications
- Collaboration facilitée
- Branches pour développement parallèle
- Retour en arrière possible
- Décentralisé (chaque clone est une sauvegarde)

**Concepts de base :**
```bash
# Initialiser un repo
git init

# Configuration
git config --global user.name "Votre Nom"
git config --global user.email "email@example.com"

# Cloner un repo
git clone https://github.com/user/repo.git

# Statut des fichiers
git status

# Ajouter des fichiers au staging
git add fichier.txt
git add .                # Tous les fichiers

# Commit
git commit -m "Message descriptif"

# Voir l'historique
git log
git log --oneline
git log --graph --all

# Voir les différences
git diff                 # Changements non stagés
git diff --staged        # Changements stagés
```

---

### 2. Quel est le workflow Git de base ?

```
Working Directory → Staging Area → Local Repository → Remote Repository
     (add)              (commit)           (push)
```

```bash
# 1. Modifier des fichiers
vim fichier.txt

# 2. Ajouter au staging
git add fichier.txt

# 3. Commit local
git commit -m "Description du changement"

# 4. Push vers remote
git push origin main
```

---

## Branches et Merge {#branches-et-merge}

### 3. Comment travailler avec les branches ?

```bash
# Lister les branches
git branch                      # Locales
git branch -a                   # Toutes (locales + distantes)

# Créer une branche
git branch feature/nouvelle-fonctionnalite

# Changer de branche
git checkout feature/nouvelle-fonctionnalite
# ou (Git 2.23+)
git switch feature/nouvelle-fonctionnalite

# Créer et changer en une commande
git checkout -b feature/nouvelle-fonctionnalite
# ou
git switch -c feature/nouvelle-fonctionnalite

# Supprimer une branche
git branch -d feature-branch    # Safe delete
git branch -D feature-branch    # Force delete

# Supprimer une branche distante
git push origin --delete feature-branch

# Renommer une branche
git branch -m ancien-nom nouveau-nom
```

---

### 4. Comment merger des branches ?

```bash
# Merger feature dans main
git checkout main
git merge feature/nouvelle-fonctionnalite

# Types de merge
# Fast-forward : historique linéaire
git merge feature-branch

# No-fast-forward : crée un commit de merge
git merge --no-ff feature-branch

# Squash : regroupe tous les commits en un seul
git merge --squash feature-branch
git commit -m "Feature: nouvelle fonctionnalite"

# Annuler un merge
git merge --abort               # Pendant un merge
git reset --hard HEAD~1         # Après un merge
```

---

## Rebase et Cherry-pick {#rebase-et-cherry-pick}

### 5. Quelle est la différence entre merge et rebase ?

```bash
# Merge : crée un commit de merge
git checkout main
git merge feature
# Historique :
#     A---B---C main
#          \   \
#           D---E feature
#                \
#                 M (merge commit)

# Rebase : réécrit l'historique
git checkout feature
git rebase main
# Historique :
#     A---B---C main
#              \
#               D'---E' feature (commits réappliqués)

# Rebase interactif (modifier l'historique)
git rebase -i HEAD~3
# Options :
# pick : garder le commit
# reword : modifier le message
# edit : modifier le contenu
# squash : fusionner avec le commit précédent
# drop : supprimer le commit
```

**Quand utiliser quoi ?**
- **Merge** : historique complet, branches publiques
- **Rebase** : historique propre, branches privées/locales

**Règle d'or :** Ne jamais rebase des commits déjà pushés/publics !

---

### 6. Comment utiliser cherry-pick ?

```bash
# Appliquer un commit spécifique sur la branche actuelle
git cherry-pick abc123

# Cherry-pick plusieurs commits
git cherry-pick abc123 def456

# Cherry-pick avec conflit
git cherry-pick abc123
# Résoudre les conflits
git add .
git cherry-pick --continue

# Annuler un cherry-pick
git cherry-pick --abort
```

---

## Résolution de Conflits {#résolution-de-conflits}

### 7. Comment résoudre les conflits Git ?

```bash
# Conflit lors d'un merge ou rebase
git merge feature-branch
# CONFLICT (content): Merge conflict in fichier.txt

# Voir les fichiers en conflit
git status

# Ouvrir le fichier et éditer
# <<<<<<< HEAD
# Code de la branche actuelle
# =======
# Code de l'autre branche
# >>>>>>> feature-branch

# Après résolution
git add fichier.txt
git commit                      # Pour merge
git rebase --continue           # Pour rebase

# Annuler la résolution
git merge --abort
git rebase --abort

# Outils de merge
git mergetool

# Choisir une version
git checkout --ours fichier.txt    # Garder votre version
git checkout --theirs fichier.txt  # Garder leur version
```

---

## Bonnes Pratiques Git {#bonnes-pratiques-git}

### 8. Quelles sont les bonnes pratiques Git ?

**Messages de commit :**
```bash
# ✅ Bon format
git commit -m "feat: ajouter authentification OAuth"
git commit -m "fix: corriger bug calcul total panier"
git commit -m "docs: mettre à jour README avec instructions Docker"

# Convention Conventional Commits
# Type: feat, fix, docs, style, refactor, test, chore
# Format: type(scope): description
git commit -m "feat(auth): implémenter login avec JWT"

# Message détaillé
git commit -m "fix: corriger calcul TVA

- Ajouter validation du taux de TVA
- Corriger arrondi à 2 décimales
- Ajouter tests unitaires

Closes #123"
```

**Workflow de branche :**
```bash
# Git Flow
main          # Production
develop       # Intégration
feature/*     # Nouvelles fonctionnalités
hotfix/*      # Corrections urgentes en production
release/*     # Préparation de release

# GitHub Flow (simplifié)
main          # Production
feature/*     # Tout le développement

# Créer une feature
git checkout -b feature/user-profile
# Développer, commit
git push -u origin feature/user-profile
# Créer une Pull Request
# Après review : merge dans main
```

**Commandes utiles :**
```bash
# Sauvegarder temporairement des changements
git stash
git stash list
git stash pop
git stash apply stash@{0}

# Modifier le dernier commit
git commit --amend -m "Nouveau message"

# Annuler des changements
git restore fichier.txt         # Annuler modifications non stagées
git restore --staged fichier.txt # Retirer du staging
git reset HEAD~1                # Annuler dernier commit (garde les changements)
git reset --hard HEAD~1         # Annuler commit et changements

# Nettoyer les fichiers non trackés
git clean -n                    # Voir ce qui serait supprimé
git clean -f                    # Supprimer
git clean -fd                   # Supprimer dossiers aussi

# Retrouver des commits perdus
git reflog
git checkout abc123
```

---

## Questions Fondamentales GitHub {#questions-fondamentales-github}

### 1. Qu'est-ce que GitHub ?

**GitHub** est une plateforme d'hébergement de code basée sur Git avec fonctionnalités collaboratives.

**Fonctionnalités :**
- Hébergement de repos Git
- Pull Requests pour code review
- Issues pour suivi de bugs/tâches
- GitHub Actions pour CI/CD
- Projects pour gestion de projet
- Wiki pour documentation
- Releases et tags

---

### 2. Comment contribuer à un projet sur GitHub ?

```bash
# 1. Fork le repo sur GitHub (bouton Fork)

# 2. Clone votre fork
git clone https://github.com/VOTRE-USERNAME/repo.git
cd repo

# 3. Ajouter l'upstream (repo original)
git remote add upstream https://github.com/ORIGINAL-OWNER/repo.git

# 4. Créer une branche pour votre contribution
git checkout -b fix/bug-description

# 5. Faire vos modifications et commit
git add .
git commit -m "fix: corriger le bug xyz"

# 6. Push vers votre fork
git push origin fix/bug-description

# 7. Créer une Pull Request sur GitHub

# 8. Mettre à jour depuis upstream
git fetch upstream
git checkout main
git merge upstream/main
git push origin main
```

---

## Pull Requests {#pull-requests}

### 3. Comment créer une bonne Pull Request ?

**Structure d'une bonne PR :**
```markdown
## Description
Courte description des changements

## Type de changement
- [ ] Bug fix
- [x] Nouvelle fonctionnalité
- [ ] Breaking change
- [ ] Documentation

## Comment tester ?
1. Checkout la branche
2. Lancer `npm install`
3. Lancer `npm test`
4. Tester manuellement en naviguant vers /login

## Checklist
- [x] Tests ajoutés/modifiés
- [x] Documentation mise à jour
- [x] Code lint sans erreurs
- [x] Tous les tests passent

## Screenshots (si applicable)
![capture d'écran](url)

## Issues liées
Closes #123
Fixes #456
```

**Bonnes pratiques :**
- PR petites et focalisées (un seul but)
- Titre descriptif
- Description claire
- Tests inclus
- Code review demandé

---

### 4. Comment faire une code review ?

```markdown
# Commentaires constructifs

✅ Bon commentaire :
"Cette fonction pourrait être simplifiée avec Array.map() au lieu d'une boucle for. 
Exemple :
```javascript
const result = items.map(item => item.value);
```
Qu'en penses-tu ?"

❌ Mauvais commentaire :
"Ce code est mauvais"

# Types de commentaires
- **Nit** : suggestion mineure
- **Question** : demande de clarification  
- **Blocking** : doit être corrigé avant merge
- **Praise** : encouragement positif

# Review checklist
- [ ] Le code fait ce qu'il prétend faire
- [ ] Tests suffisants
- [ ] Pas de régression
- [ ] Lisibilité et maintenabilité
- [ ] Performance acceptable
- [ ] Sécurité (pas de failles)
- [ ] Documentation à jour
```

---

## GitHub Actions {#github-actions}

### 5. Comment utiliser GitHub Actions ?

```yaml
# .github/workflows/ci.yml
name: CI

on:
  push:
    branches: [main, develop]
  pull_request:
    branches: [main]

jobs:
  test:
    runs-on: ubuntu-latest

    strategy:
      matrix:
        node-version: [16, 18, 20]

    steps:
      - name: Checkout code
        uses: actions/checkout@v3

      - name: Setup Node.js ${{ matrix.node-version }}
        uses: actions/setup-node@v3
        with:
          node-version: ${{ matrix.node-version }}
          cache: 'npm'

      - name: Install dependencies
        run: npm ci

      - name: Run linter
        run: npm run lint

      - name: Run tests
        run: npm test

      - name: Upload coverage
        uses: codecov/codecov-action@v3
        with:
          files: ./coverage/coverage-final.json

  deploy:
    needs: test
    runs-on: ubuntu-latest
    if: github.ref == 'refs/heads/main'

    steps:
      - uses: actions/checkout@v3

      - name: Deploy to production
        env:
          DEPLOY_KEY: ${{ secrets.DEPLOY_KEY }}
        run: |
          echo "Deploying..."
          # Commandes de déploiement
```

**Actions courantes :**
- `actions/checkout` : clone le repo
- `actions/setup-node` : configure Node.js
- `actions/cache` : cache des dépendances
- `actions/upload-artifact` : sauvegarde des artifacts
- `codecov/codecov-action` : upload coverage

---

## GitHub Workflows {#github-workflows}

### 6. Quels sont les workflows GitHub courants ?

**Release automatique :**
```yaml
name: Release

on:
  push:
    tags:
      - 'v*'

jobs:
  release:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v3

      - name: Build
        run: npm run build

      - name: Create Release
        uses: actions/create-release@v1
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
        with:
          tag_name: ${{ github.ref }}
          release_name: Release ${{ github.ref }}
          draft: false
          prerelease: false

      - name: Upload Release Asset
        uses: actions/upload-release-asset@v1
        with:
          upload_url: ${{ steps.create_release.outputs.upload_url }}
          asset_path: ./dist/app.zip
          asset_name: app.zip
          asset_content_type: application/zip
```

---

## Collaboration GitHub {#collaboration-github}

### 7. Comment gérer un projet collaboratif sur GitHub ?

**Organisation du repo :**
```
repo/
├── .github/
│   ├── workflows/           # CI/CD
│   ├── ISSUE_TEMPLATE/      # Templates d'issues
│   ├── PULL_REQUEST_TEMPLATE.md
│   └── CODEOWNERS           # Reviewers automatiques
├── docs/                    # Documentation
├── README.md                # Introduction
├── CONTRIBUTING.md          # Guide de contribution
├── CODE_OF_CONDUCT.md       # Code de conduite
└── LICENSE                  # Licence
```

**Protections de branches :**
```
Settings → Branches → Branch protection rules

✅ Require pull request reviews (1-2 reviews)
✅ Require status checks (CI doit passer)
✅ Require branches to be up to date
✅ Restrict who can push
✅ Require signed commits (optionnel)
```

**Labels pour issues/PRs :**
- `bug` : problème à corriger
- `enhancement` : nouvelle fonctionnalité
- `documentation` : amélioration doc
- `good first issue` : pour débutants
- `help wanted` : besoin d'aide
- `wontfix` : ne sera pas traité

**Milestones :**
Regrouper issues/PRs par version ou sprint

**Projects :**
Kanban board pour organiser le travail
- To Do
- In Progress
- Review
- Done

---

