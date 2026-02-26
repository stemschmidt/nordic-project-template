# 3 - Scope and Context {#page_03_scope_and_context}

## System Context Diagram

Show:

- Sensors

- Actuators

- Cloud backend

- Mobile app

- Debug interface

- Power supply

## External Interfaces

- GPIO

- UART

- I2C / SPI

- LTE / BLE

- Debug (SWD)

@startuml
!include https://raw.githubusercontent.com/plantuml-stdlib/C4-PlantUML/master/C4_Context.puml

<style>
header {
    HorizontalAlignment left
    FontSize 16
    FontColor black
    FontStyle bold
}
<style>

header "[System Context] xx Sensor"

SetDefaultLegendEntries("")

SHOW_PERSON_OUTLINE()
 

SHOW_LEGEND()
@enduml
