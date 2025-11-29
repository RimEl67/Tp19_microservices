# TP 19 : Orchestration de microservices avec Spring Cloud: Eureka, Gateway et OpenFeign
# par: Rim EL ABBASSI

## 🎯 But du TP
Ce TP a pour objectif de mettre en pratique l'orchestration de microservices à l'aide de Spring Cloud.  
Vous apprendrez à :  
- Déployer un **Eureka Server** pour la découverte des services.  
- Configurer une **API Gateway** pour le routage et l’accès centralisé aux services.  
- Utiliser **OpenFeign** pour la communication inter-services.  
- Comprendre le cycle complet d’une requête dans un environnement microservices.

---

## ⚙️ Concepts principaux
- **Indépendance des services :** chaque microservice gère son domaine et peut être déployé seul.  
- **Communication légère :** échanges via HTTP/REST ou Feign (synchrone).  
- **Base de données isolée :** chaque service dispose de son stockage local (H2 en mémoire).  
- **Scalabilité horizontale :** plusieurs instances d’un service derrière un LoadBalancer.

---


## 🗺️ Architecture du TP
| Service           | Description                               | Port  |
|------------------|-------------------------------------------|-------|
| Eureka Server     | Registre central des microservices        | 8761  |
| SERVICE-CLIENT    | Gestion des clients (H2 en mémoire)      | 8088  |
| SERVICE-VOITURE   | Gestion des voitures, utilise Feign pour SERVICE-CLIENT | 8089  |
| Gateway           | Entrée unique avec routage statique et dynamique | 8888  |

---

## Captures
<img width="1366" height="768" alt="9" src="https://github.com/user-attachments/assets/beda4376-516e-4275-b5d6-80920b5e5571" />
<img width="1366" height="728" alt="7" src="https://github.com/user-attachments/assets/fd010c1d-9599-4757-b2b4-7e098a182f1f" />
<img width="1366" height="732" alt="6" src="https://github.com/user-attachments/assets/0dff3612-22a0-40cb-93e9-5b9b1bfc73c5" />
<img width="1366" height="768" alt="8" src="https://github.com/user-attachments/assets/32a862c3-42e8-4c32-8ae1-95f9f730a7ea" />
