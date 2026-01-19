# SNOMED CT Attributes

SNOMED CT currently uses over 50 defining attributes to model concept definitions. SNOMED CT defining attributes are relationship types used to represent inherent, necessary characteristics of a concept's meaning, forming part of its logical definition. 
The hierarchy or hierarchies to which an attribute can be applied are referred to as the “domain” of the attribute. Each attribute can be given a limited set of values; this set of values is called the “range” of the attribute. A sample of these are demonstrated below.

## Attribute Domain and Range Examples

| Domain | Attribute | Range | Example ECL |
|---|---|---|---|
| Clinical finding | Finding site (363698007) | Anatomical structure | `< 404684003 |Clinical finding| : `<br>` 363698007 |Finding site| = << 442083009 | Anatomical or acquired body structure |` |
| Clinical finding | Associated morphology (116676008) | Morphologic abnormality | `< 19829001 |Pulmonary disease| :`<br>` 116676008 |Associated morphology| = << 79654002 |Oedema|` |
| Clinical finding | Associated with (47429007) | Clinical finding | `<< 404684003 |Clinical finding| : `<br>` << 47429007 |Associated with| = << 271737000 | Anaemia |` | 
| Disease | Causative agent (246075003) | Substance (organism/chemical) | `< 64572001 |Disease| :`<br>` 246075003 |Causative agent| = << 65119002 |Staphylococcus species|` |
| Body structure | Laterality (272741003) | Laterality values (e.g., Left) | `<< 91723000 |Anatomical structure (body structure)|:`<br>`     272741003 |Laterality| = 18237771000 |Left|` |
| Medicinal product | Has active ingredient (127489000) | Substance | `< 763158003 |Medicinal product| : `<br>` << 127489000 |Has active ingredient| = 190332006 |Paracetamol|` |
| Pharmaceutical/biologic product | Has manufactured dose form (411116001) | Pharmaceutical dose form | `< 373873005 |Pharmaceutical / biologic product| : `<br>` 411116001 |Has manufactured dose form| = << 421026006 |Tablet|` |
| Procedure | Procedure site (363704007) | Anatomical structure | `< 71388002 |Procedure| : `<br>` << 363704007 |Procedure site| = << 39057004 |Pulmonary valve structure| ` |
| Procedure | Using device (424226004) | Device | `< 71388002 |Procedure| : `<br>` << 424226004 |Using device| = << 90412006 |Colonoscope|` |

Note:  The authoritative domain/range constraints for attributes are defined in the [SNOMED CT Editorial Guide](https://docs.snomed.org/snomed-ct-specifications/snomed-ct-editorial-guide/readme/authoring/domain-specific-modeling).

