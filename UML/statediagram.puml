@startuml

title State Diagram

  state "Ready" as INIT
  state "Preview" as PREV
  state "Scanning" as SCAN
  state "Stop" as STOP
  
  [*] --> INIT: HW ready
  INIT --> INIT: system setting
  INIT --> PREV: insert slides
  PREV --> SCAN: scan
  SCAN --> STOP: output image
  STOP --> [*]: exit application
@enduml
