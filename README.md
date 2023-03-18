# InstagramClone
We are developing a simpler and abridged version of Instagram for a University Project.

# Code Compilation and Code Execution

Different layer combinations can be used by manipulating a simple configuration file, by the name of Layer.cfg, placed in the Models package. Setting the “Database” property to “Firebase” allows for the program to work with a DB and setting the property to “Text” allows the program to work in a textual database.  The Interface used can be manipulated by changing the “User_Interface”, property to “Graphical” for a GUI and “Console” for a CLI. The “Main.java” class in the Package “Combination” needs to be run to execute the project.

# Design Principles

-Single Purpose - i.e all Modules are developed in such a way as to enusre that they cater to a single responsibility
-Interface Segregation - All Interfaces are created while ensuring that the modules implementing them do not have to implement any functions not part of thei design
-Dependency Inversion - Is ensured by making sure that no one module depends on how another module implements a feature and instead that a module does implement any given feature
-Polymorphism - As there are multiple implementations present for the same layer, polymorphism is used to make sure that program can run smoothly irrespective of layer used. e.g CLI or GUI is used.

# Design Decision

-Use of Models - Models/Dat Structures are used to transfer data across layers. This is done because using JSON would have required constant packing and unpacking of data which would result in excessive and needless operations
-Use of Factories - Done to enusre that layers remain independant of how other layers work
-Service Classes - Service Classes are used to implement methods needed by Data Structures
-Interfaces - Used to enusre that different layers are not affected by how other layers implemnt their code
