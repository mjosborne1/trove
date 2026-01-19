# Welcome to Trove

## About

Trove is a collection of links to practical, hands-on FHIR Terminology and SNOMED CT resources. [ECL Examples](ecl_examples/) are largely drawn from the [SNOMED Expression Constraint Language Examples](https://github.com/IHTSDO/snomed-expression-constraint-language/tree/main/examples), which is an open source starter set for learning ECL. 


## Glossary

* **Domain** is the hierarchy to which a specific SNOMED CT attribute can be applied. For example a Procedure has a PROCEDURE MORPHOLOGY, but does not have an ASSOCIATED MORPHOLOGY, which is in the domain of the Clinical finding hierarchy. Domain and it's partner, Range, are so critical to ECL, they have a dedicated tutorial.

* **ECL (Expression Constraint Language)** is a formal, declarative language for defining precise, computable subsets of clinical meanings within SNOMED CT, allowing rich querying and constraint definition for tasks like restricting EHR data, building value sets (e.g., for FHIR), and defining reference sets by specifying relationships and attributes between concepts. ECL expressions are executable rules that define intensional sets, enabling powerful data analysis and interoperability by precisely identifying groups of related clinical concepts. 

* **Extensional value set** a predefined, explicit list of specific concepts in a value set. The value set can only contain those enumerated values in the expansion. The value set expansion cannot change without redefining the logical definition of the valueset. For example a 'Gender Identity ValueSet' might contain explicitly stated concepts for 'Female gender identity', 'Male gender identity' and 'Non-binary gender identity'. 

* **Intensional value set** defines a group of SNOMED CT concepts using a logical rule or algorithm, rather than listing every single code, allowing it to dynamically update as new codes are added. For example, a 'Diabetes ValueSet' could be defined as "all descendants of the 'Diabetes' concept". 

* **Range** is the set of values allowed for each SNOMED CT attribute. For example, the Range for ASSOCIATED MORPHOLOGY is Morphologically abnormal structure (morphologic abnormality) and its descendents. Domain and Range are so critical to ECL, they have a dedicated tutorial.

* **Reference Set** is a set of SNOMED CT Concepts for a particular purpose. Some examples are: to represent subsets of concepts; to indicate language/dialect preferences; to represent maps to or from other code systems. For example, a Reference Set (RefSet for short) might contain all body sites that are direct sites for surgical procedures.




## Links

### ECL (Expression Constraint Language)
* [What is ECL?](https://docs.snomed.org/snomed-ct-user-guides/snomed-ct-browser-guide/faqs/the-expression-constraint-language-ecl) - The definitive SNOMED International documentation
* [Shrimp ECL Builder](https://ontoserver.csiro.au/shrimp/ecl/?fhir=https://r4.ontoserver.csiro.au/fhir) - SNOMED CT ECL Builder tool shipped with Ontoserver Terminology Server 
* [ECL Builder](https://ecl-builder.vercel.app/) - A UI to build ECL expressions from CSIRO AEHRC
* [ECL Expression Tester](https://ecl-tester.onrender.com/) - A repository of testable ECL expressions by myself
* [SNOMED Expression Constraint Language Examples](https://github.com/IHTSDO/snomed-expression-constraint-language/tree/main/examples) - Examples of SNOMED CT ECL expressions produced by SNOMED International
* [ECL Formatter](https://mattcordell.github.io/ecl-formatter/) - A tool to make ECL expressions more readable by Matt Cordell from CSIRO AEHRC
