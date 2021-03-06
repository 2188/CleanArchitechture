All Architecture have the same objective, which is the separation of concerns. They all achieve
this separation by dividing the software into layers. Each has at least one layer for
business rules, and another for interfaces.

The clean architecture have several layer:

1) Entity -> Which consist of Enterprise business rules.
2) Use cases -> Which consist of application business rule.
3) Controller or Presenter or Gateway -> Which consist interactor interfaces (Adapter interfaces)
4) Framework or Drivers or Device

In that the Presenter interact with Use case of Output port and Controller will interact with Input port
and both input and output port will communicate with Interface adapter.

All the architecture will produce a systems that are:

- Independent of Frameworks:- The architecture does not depend on the existence of some library
 of feature laden software. This allows you to use such frameworks as tools, rather than having
 to cram your system into their limited constraints.

- Testable:- The business rules can be tested without the UI, Database, Web Server, or any other
external element.

- Independent of UI:- The UI can change easily, without changing the rest of the system. A Web
UI could be replaced with a console UI, for example, without changing the business rules.

- Independent of Database:- You can swap out Oracle or SQL Server, for Mongo, BigTable, CouchDB,
or something else. Your business rules are not bound to the database.

- Independent of any external agency:- In fact your business rules simply don’t know anything
at all about the outside world.

