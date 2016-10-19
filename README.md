# OOAD-WEEK08

## Use Case Diagram (ภาษาไทย)
###ภาพที่ 1
```
@startuml
'default
top to bottom direction
taxidriver --> (driver)
customer --> (pay)
@enduml
```
###![](http://www.plantuml.com/plantuml/img/DOp12e0W40Nl-nLxAm_-GlWhcne8wee-e_w-8BeDmp1kG3fcoRI4UCZC86XZAEyAQE6GUlH8MWbofT3J6JjRk_7wiI4_nnl-jibjY5oiuPq-)

####ภาพที่ 2 หาหมอ 
```
@startuml
left to right direction
skinparam packageStyle rect
actor customer
actor doctor
actor staff
rectangle healty {
  customer -- (heal)
  (assignt) -- (staff)
  customer --(assignt)
  customer -- (pay)
  (pay) -- (staff)
  (heal) -- doctor
}
@enduml
```
####![](http://www.plantuml.com/plantuml/img/NOvB3iCW34JtdCBBiCWTUeUUm2A6eF0JE0jKzUu5WYAbgz6CPvxyAeoPJ--48yt04R8rEyDcCocsCOXos90meuU4wa13RwwEe9y5AeuPr5auUihJRh7BD0sljUXb3ARDTaB75Ju2xXciAomzborSi1Hh0ikHZhLyTk_6Fo9X7OIkp_L5xzdyxVi3)

#####ภาพที่ 3 taxi 
```
@startuml
left to right direction

taxidriver --> (start car)
taxidriver --> (change gear)
taxidriver --> (driver)
@enduml
```
#####![](http://www.plantuml.com/plantuml/img/ROqn2e0m303tl2AZ7Ve5wLT26zj0JI56yVcAZheT7CUbpSbyNpjqNXnze4bjZaMCiyjG0ATJYid1XZ7EE3q5PhBmKRcHLiRAV_Bb08crtCCB)

######ภาพที่ 4 จ่ายค่าห้อง
```@startuml
left to right direction
skinparam packageStyle rect
actor customer
actor occupant
rectangle room{
  customer -- (payment)
  (payment) .> (calculate)
 (payment) .>(check)
(check) -- occupant
(calculate) --occupant
}@enduml
```
######![] (http://www.plantuml.com/plantuml/img/JOqn3iCW34LtJk6H3EaHgjoX9x1Sbw00Hc26gEhT2rA4Cjb-xzlUgcBH5eC9_55GWUBThl3sXKcz95CFdp8MZ92H3dJyqZCm36sGL0fGgogHopKAKSkOr8m89ZV28l5hO2PXNS5cF2CdNJgVFJoUO0a3jO3ANTsDfPtfMCnLnv7vwxRK-SI_Fm00)

######ภาพที่ 5 เช็คเอ้าท์ 
```@startuml
left to right direction
skinparam packageStyle rect
actor customer
actor clerk
rectangle checkout {
  customer -- (checkout)
  (checkout) .> (payment)
  (payment) -- clerk
}
@enduml
```
######![](http://www.plantuml.com/plantuml/img/HSuz3iCm20NWdLCmfaDwX2ftw0cGGntBly9uYAhUlROYjnjFtmEnLINH5WC4VYbgHd7sKDoTi56N4rJlKY6XY8MC9yjFFGFZO22ZMT2qgZcop1XOF0odP7lJ76nyReflm5yNrnMNARSE_u3t1ow5piZfaZcFdUlu1pPEU__w2m00)
