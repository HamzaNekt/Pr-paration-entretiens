# Guide d'Entretien Technique - Questions et Réponses

Ce document contient une collection structurée de questions fréquemment posées lors d'entretiens techniques, accompagnées de réponses détaillées et d'exemples de code. Il couvre Java, Spring Boot, JavaScript, Angular et React.

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