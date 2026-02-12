```kroki-plantuml
@startuml 

!include https://raw.githubusercontent.com/plantuml-stdlib/C4-PlantUML/latest/C4_Context.puml

Person(P, "Клиент")
System(S1, "Хрень1")
System(S2, "Хрень1")
System(S3, "Хрень3")
System(S4, "Система упралвения устройствами и пользователями")

Rel(P, S1, "Регулирует температуру")
Rel(S1,P, "Плучает температуру")

@enduml
``` 