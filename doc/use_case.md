@startuml
actor "Кай" as kay
actor "Герда" as gerda

package "Управление золотыми активами" {
  usecase "Собрать слово" as word
  usecase "Найти замок" as find_castle
  usecase "Растопить сердце" as melt_heart
}
kay-->word
gerda--> find_castle
gerda--> melt_heart

find_castle ..> melt_heart : <include>
@enduml :