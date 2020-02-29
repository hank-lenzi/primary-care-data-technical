# Australian Primary Care Practice-to-Practice Record Transfer IG

This project contains all the files necessary to generate the Implementation Guide (IG) for the primary care data technical project. 

It uses FHIR Shorthand (see http://build.fhir.org/ig/HL7/fhir-shorthand/) for simple definition of Profiles, terminology resources, and examples.
Run `sushi . -o .` to re-generate the FHIR Resources

The IG publisher is used to build the IG and you can obatain the latest copy with `_updatePublisher.sh`

You should specify the terminology server using the -tx option. https://primarycare.ontoserver.csiro.au/fhir has all the referenced ValueSets and CodeSystems referred to by the IG.

Example usage:
```
_genonce.sh -tx https://primarycare.ontoserver.csiro.au/fhir
```

