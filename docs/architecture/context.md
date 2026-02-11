```kroki-plantuml
@startuml 

!include https://raw.githubusercontent.com/plantuml-stdlib/C4-PlantUML/master/C4_Context.puml

Person(P, "Клиент")
System(S1, "Система управления воротами")
System(S2, "Система управления видеонаблюдением")
System(S3, "Система управления отоплением")
System(S4, "Система упралвения устройствами и пользователями")

Rel(P, S1, "Регулирует температуру")
Rel(S1,P, "Плучает температуру")

@enduml
``` 