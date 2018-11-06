# conver

ArcheTECTURE GLOBALE D’application :

The Model-View-Controller (MVC) is an architectural pattern that separates an application into three main logical components: the model, the view, and the controller. Each of these components are built to handle specific development aspects of an application. MVC is one of the most frequently used industry-standard web development framework to create scalable and extensible projects.
Model
The Model component corresponds to all the data-related logic that the user works with. This can represent either the data that is being transferred between the View and Controller components or any other business logic-related data. For example, a Customer object will retrieve the customer information from the database, manipulate it and update it data back to the database or use it to render data.
View
The View component is used for all the UI logic of the application. For example, the Customer view will include all the UI components such as text boxes, dropdowns, etc. that the final user interacts with.
Controller
Controllers act as an interface between Model and View components to process all the business logic and incoming requests, manipulate data using the Model component and interact with the Views to render the final output. For example, the Customer controller will handle all the interactions and inputs from the Customer View and update the database using the Customer Model. The same controller will be used to view the Customer data.



Architecture dla la couche donnee :
 		

L'architecture trois tiers, également appelée architecture à trois niveaux ou à trois couches, est une architecture client-serveur dans laquelle coexistent et sont maintenus des modules indépendants permettant le rendu d'une interface utilisateur (GUI), les process logiques, fonctionnels et métiers ainsi que l'accès aux données. On parle donc ici d'une infrastructure physique qui va servir de support à une infrastructure logicielle (l'infrastructure trois tiers sous-tend l'infrastructure logicielle).En effet, n'importe quelle application peut-être découpée en trois parties : une partie interface graphique, une partie fonctionnelle, et une partie de stockage de données. Et c'est à ces besoins précis que l'architecture trois-tiers s'est dessinée en découpant trois parties distinctes :
 
- L'IHM : le navigateur installé sur le poste client qui fait un rendu visuel,
- Le serveur Applicatif : pour la partie traitement et fonctionnelle (de nombreux langages applicatifs tels que Java, PHP, Ruby peuvent être utilisés)
- Le serveur de base de données : ce qui va permettre de stocker et de restituer les données (MySQL, PostgreSQL, Cassandra)
L'architecture trois tiers se veut moderne et son découpage en trois parties fait d'elle un essentiel pour le développement d'applications Web, afin d'apporter plus de performances, de sécurité mais en apportant également une maintenance plus aisée. Elle vient s'opposer à l'infrastructure traditionnelle 2-tiers qui ne dissocie pas la partie serveur applicatif de la partie base de données (les deux sont sur le même support logique).
Le plan de cet article sera donc découpé en trois parties logiques : tout d'abord, nous parlerons de la couche de présentation. Dans un second temps, nous aborderons la la couche de traitement. Puis nous finirons par parler du dernier tiers de ce type d'architecture : le tiers d'accès aux données.
La couche de présentation :

C'est la première couche qui compose l'infrastructure trois tiers : il s'agit de la partie rendu logiciel. Elle est rendue possible grâce aux langages de rendus, en l'occurence pour une application Web, le HTML5, le CSS3 et le Javascript pour ajouter une partie fonctionnelle à ce rendu.
 
La couche Métier ou Fonctionnelle :
C'est la seconde couche qui compose l'infrastructure trois tiers : elle correspond à un ensemble de composants métiers qui permettent de traiter un ensemble d'actions sur un serveur, et de faire éventuellement appel à des services externes pour envoyer une réponse au client. Le client communique donc avec le serveur grâce à l'interface graphique, puis le serveur fait son traitement et renvoie la réponse au client. Les langages serveurs les plus utilisés sont : le PHP, le Ruby, le C/C++/C#, mais également le Python.
 
è
La couche d'accès aux données
C'est la troisième couche qui compose l'infrastructure trois-tiers : elle correspond au serveur de base de données. Il s'agit de la couche d'accès aux données. Sur ce troisième ters, un SGBD (Système de Gestion de Base de Données) est installé, comme par exemple MySQL ou Microsoft SQL Server, et ce serveur est requêté par le serveur applicatif afin d'utiliser un certain nombre de données.
 

La technologie utilisee pour le devloppement :
Java ee :  


Java Platform, Enterprise Edition (Java EE) is the standard in community-driven enterprise software. Java EE is developed using the Java Community Process, with contributions from industry experts, commercial and open source organizations, Java User Groups, and countless individuals. Each release integrates new features that align with industry needs, improves application portability, and increases developer productivity.
 - Java EE 8 continues to improve API and programming models needed for today's applications and adds features requested by our world-wide community. This release modernizes support for many industry standards and continues simplification of enterprise ready APIs. Enhancements include:
•Java Servlet 4.0 API with HTTP/2 support
•Enhanced JSON support including a new JSON binding API
•A new REST Reactive Client API
•Asynchronous CDI Events
•A new portable Security API
•Server-Sent Events support (Client & Server-side)
•Support for Java SE 8 new capabilities (e.g. Date & Time API, Streams API, annotations enhancements)
Java EE 8 builds on Java EE 7. The following JSRs are new or updated in Java EE 8:
•JSR 366 – Java EE 8 Platform
•JSR 365 – Contexts and Dependency Injection (CDI) 2.0
•JSR 367 – The Java API for JSON Binding (JSON-B) 1.0
•JSR 369 – Java Servlet 4.0
•JSR 370 – Java API for RESTful Web Services (JAX-RS) 2.1
•JSR 372 – JavaServer Faces (JSF) 2.3
•JSR 374 – Java API for JSON Processing (JSON-P)1.1
•JSR 375 – Java EE Security API 1.0
•JSR 380 – Bean Validation 2.0
•JSR 250 – Common Annotations 1.3
•JSR 338 – Java Persistence 2.2
•JSR 356 – Java API for WebSocket 1.1
•JSR 919 – JavaMail 1.6

