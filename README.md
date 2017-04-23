Prerequisites:
- instalati MongoDB urmand pasii specificati in urmatorul link:
https://docs.mongodb.com/manual/tutorial/install-mongodb-enterprise-on-windows/

Cerinte:
1. Introduceti un layer the legatura intre repository si controller (service layer, asa cum am facut in toate 
exemplele anterioare)
2. Introduceti defensive coding si builder in controller(de ex: operatia POST nu contine defensive coding)
3. Modificati UI-ul (java script si html) astfel incat marcarea unui task (TODO) sa nu fie facuta print-un radio button, asa cum este acum (ci prin doua butoane => MarkAsDone, MarkAsNotDone imediat dupa butoanele de Edit si Delete)
	a) modificarea de mai sus necesita si modificarea action-urilor din controller (vor exista 2 action-uri pentru fiecare tip de Mark)
	b) pentru ca operatiile de Mark sunt update-uri partiale folositi PATCH ca HttpVerb

Nota: puteti folosi un toggle button pentru a simula activa/dezactivarea. Daca folositi 2 butoane atunci va trebui sa gestionati si starea lor la afisare:
	- cand este adaugat un task nou doar butonul MarkAsDone este activ
	- cand este este apasat MarkAsDone, acesta va trimite comanda catre server si va deveni disable iar MarkAsNotDone este activ.

Challenge:
	- adaugati un nou document in MongoDB unde sa tineti un History al starilor

Suplimentar:
	- http://websystique.com/springmvc/spring-4-mvc-angularjs-crud-application-using-ngresource/
