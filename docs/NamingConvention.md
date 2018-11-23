
  
# Naming conventions in Nature 4.0 
## Naming conventions for study locations and sensor platforms

The names for study plots and sensor plattforms are made up of the following elements:
1. Three-digit letter sequence for the study area.
2. Three-letter sequence for the entity.
3. Five-digit number sequence for consecutive numbering.
Letter sequences are always in lowercase letters. The elements are separated by underscores snake_cases. 

### Three-digit letter sequence for the study area
This describes the parent region. For the entire Marburg Open Forest, the name is "mof". 

### Three-character string for the entity
This describes the type of plot. The encoding is derived from the entity's English name and, if possible, matches the first three letters. The following types are already set:

| Entity | Description |
|--|--|
| Places | |
| plt  | Study plots |
| cst  | Trees (core study trees) |
| Technical | |
| cbh | Cableways (horizontal) |
| cbv | Cableways (vertical) |
| clm | Climate station |
| rve | Rovers |
| Humans | |
| exp | Expert |
| std | Student |
| class | School or university class |
| ppl | Pupil |
| Animals | |
| bat | Bats |
| brd | Birds |
| der | Deers |
| hrs | Horses |




### Five-digit number sequence for ongoing numbering
This numbers the individual entities.

### Example
The following designation would be used for the first core study tree in the Marburg Open Forest: *mof_cstr_00001*

## Naming conventions for sensor boxes
The names for sensor boxes are regulated as follows:
1. Small b to indicate that it is a box
2. Three-digit letter sequence for the type of sensor box 
3. Three-digit number sequence for consecutive numbering
 | Entity | Description |
|--|--|
| base | Base component (data logger, energy supply, communication etc.) |
| metc | Meteorlogical core unit (temperature, humidity, light) |
| audi | Audio recording unit (microphone arrays) |

# Example
The following name would be used for the first meteorological core unit metc_00001.
