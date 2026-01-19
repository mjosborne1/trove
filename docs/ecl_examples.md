# ECL Examples

This page contains examples of Expression Constraint Language (ECL) expressions used in SNOMED CT.

## Basic Examples

### 1.1 Self

Reference to a specific concept by its identifier.

```
404684003 |clinical finding|
```

### 1.2 Descendant Of

Matches all descendants of the specified concept.

```
< 404684003 |clinical finding|
```

### 1.3 Descendant Or Self Of

Matches the concept itself and all its descendants.

```
<< 73211009 |diabetes mellitus|
```

### 1.4 Ancestor Of

Matches all ancestors of the specified concept.

```
> 40541001 |Acute pulmonary oedema|
```

### 1.5 Ancestor Or Self Of

Matches the concept itself and all its ancestors.

```
>> 40541001|Acute pulmonary oedema|
```

### 1.6 Member Of

Matches all concepts that are members of the Problem/Diagnosis reference set.

```
^ 933600511000036109 |Problem/Diagnosis reference set|
```

### 1.7 Any

Matches any concept in SNOMED CT.

```
*
```

### 1.8 Child Of

Matches the direct children of the specified concept.

```
<! 404684003 |clinical finding|
```

### 1.9 Parent Of

Matches the direct parents of the specified concept.

```
>! 40541001 |acute pulmonary edema|
```

## Intermediate Examples

### 2.1 Attribute

Specifies a constraint with a single attribute and value.

```
< 19829001 |disorder of lung|: 
    116676008 |associated morphology| = 79654002 |edema|
```

### 2.2 Attribute Group

Groups multiple attributes together, where all attributes in a group must be satisfied together.

```
< 404684003 |clinical finding|:
    { 363698007 |finding site| = << 39057004 |pulmonary valve structure|,
      116676008 |associated morphology| = << 415582006 |stenosis| },
    { 363698007 |finding site| = << 53085002 |right ventricular structure|,
      116676008 |associated morphology| = << 56246009 |hypertrophy| }
```

### 2.3 Term Filter

Filters concepts by matching disease Causative agents and a text Term filter

```
(< 64572001 |Disease| . 246075003 | Causative agent |) {{ term = "Staph" }}
```

### 2.4 Body Structure Left

References all left-sided body structure concepts 

```
<123037004 | Body structure | : 272741003 | Laterality | = 7771000 | Left |
```

### 2.6 Attribute Constraint Operator

Constrains attribute values using operators like descendant-or-self.

```
<< 404684003 |clinical finding|:
    << 47429007 |associated with| = << 267038008 |edema|
```

### 2.7 Any Attribute Name Value

Uses wildcard to match any attribute with a specific value.

```
< 404684003 |clinical finding|:
    * = 79654002 |edema|
```


### 2.8 Dotted Attributes

Chains attributes together using dot notation to navigate through nested relationships.

```
< 91723000 |Anatomical structure| AND ( < 125605004 |Fracture of bone| . 363698007 |Finding site| )
```
