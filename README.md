# Nothingan Pri – ERP/CRM per a lloguer de vehicles
![Portada del projecte Nothingan Pri](docs/portada.png)

Producte mínim viable (MVP) d'una aplicació web d'ERP i CRM per a **Nothingan Pri S.A.**, empresa familiar de lloguer de vehicles a Terrassa. L'aplicació cobreix tot el procés de negoci: des de l'alta del client fins al retorn del vehicle i el càlcul de la fiança.

## 👥 Equip
- Nil Mampel – responsable de la gestió de vehicles
- Zohaib Zaib – responsable de la gestió d'usuaris
- Ruben García - responsable de la gestió de reserves

## 🛠 Tecnologies
Java · Spring Boot · Thymeleaf · Maven · base de dades relacional · MongoDB · JUnit 5 · Git

## ✨ Funcionalitats
- Alta de clients (per web o per un agent), amb validació de l'administrador si és per web
- Clients premium amb descompte a la fiança
- Gestió de vehicles: alta, baixa, activació, desactivació, lliurament i retorn
- Reserves amb bloqueig automàtic del vehicle
- Lliurament i retorn amb fotos i observacions d'incidències
- Càlcul automàtic de la retenció de fiança
- Informes de reserves filtrables
- Aplicació multiusuari amb permisos per rol (administrador, agent i client)
- Interfície responsive, accessible i en català

## 🗄️ Arquitectura de dades
- **Base de dades relacional:** clients, vehicles, reserves i fiances.
- **MongoDB (NoSQL):** fotos i documents (DNI, llicència, lliuraments, retorns, incidències), notificacions, logs del sistema i preferències de client. La base relacional només guarda referències a aquests documents.

## 📄 Documentació
- [Memòria del projecte](docs/memoria.pdf)
- [Diagrama de base de dades](docs/diagrama-bd.png)

## ▶️ Com executar-lo
1. Clona el repo: `git clone https://github.com/nmampel24/nothingan-pri-erp-crm.git`
2. Copia `application.properties.example` a `application.properties` i omple les teves dades de connexió
3. Executa: `mvn spring-boot:run`
