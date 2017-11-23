# Void Empires Design

## Designs

- "Restoration Specialists"
  - Requires one point of Materialist
  - Cannot colonize worlds
  - Gains unity from restoring damaged megastructures
  - Unique Start (Phoenix)
    - Starts on a Ringworld
      - Other three segments are destroyed
    - Starts next to a destroyed Ringworld (Ashes)
    - Destroyed Megastructure (Colossus)
  - Unique event chain to restore the three damaged segments
    - grants megastructure restoration
    - repairs damaged segments (but costs influence)
    - flavor description of empire's purpose

** To Do:**
- Civic icon

** Not Implemented Yet:**

- "Planetary Conservationists"
  - Requires one point of Spiritualist
  - Cannot colonize worlds
  - Gains unity by building "Planetary Conservation Shrine" megastructure around habitable world
  - Unique Start (Eden)
    - Starts on a Ringworld segment
      - Other three segments are destroyed
    - Starts next to two systems with Gaia worlds
      - Pishon (2 gaia worlds, uninhabited)
      - Cush (2 gaia worlds, inhabited by primitives)
  - Unique event chain to restore the three damaged segments
    - grants megastructure restoration
    - repairs damaged segments (but costs influence)
    - flavor description of empire's purpose
    - grants Voidborne ascension perk

## System Initializers

- Phoenix (one ringworld, 3 broken segments)
- Ashes (destroyed ringworld)
- Colossus (destroyed megastructure)
- Eden (one ringworld, 3 broken segments)
- Pishon (2 gaia worlds, uninhabited)
- Cush (2 gaia worlds, inhabited by primitives)

## Civics

- civic_restoration_specialist
- civic_planetary_conservationist

## on_action

- when megastructure restored, grant unity to civic_restoration_specialist
- when megastructure_planetary_shrine built, update bonus of civic_planetary_conservationist

## event chains

- event_phoenix_rises
- event_eden_reclaimed

## Megastructures

- megastructure_planetary_shrine
