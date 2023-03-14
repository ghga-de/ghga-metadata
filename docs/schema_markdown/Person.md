
# Class: person


A member of the species Homo sapiens.

URI: [https://w3id.org/GHGA-Submission-Metadata-Schema/Person](https://w3id.org/GHGA-Submission-Metadata-Schema/Person)


[![img](https://yuml.me/diagram/nofunky;dir:TB/class/[Person&#124;given_name:string%20%3F;family_name:string%20%3F;additional_name:string%20%3F;id(i):string;alias(i):string;xref(i):string%20*]^-[Member],[Person]^-[Individual],[NamedThing]^-[Person],[NamedThing],[Member],[Individual])](https://yuml.me/diagram/nofunky;dir:TB/class/[Person&#124;given_name:string%20%3F;family_name:string%20%3F;additional_name:string%20%3F;id(i):string;alias(i):string;xref(i):string%20*]^-[Member],[Person]^-[Individual],[NamedThing]^-[Person],[NamedThing],[Member],[Individual])

## Parents

 *  is_a: [NamedThing](NamedThing.md) - A database entity, concept or class. This is a generic class that is the root of all the other classes.

## Children

 * [Individual](Individual.md) - An Individual is a Person who is participating in a Study.
 * [Member](Member.md) - Member of an Organization or a Committee.

## Referenced by Class


## Attributes


### Own

 * [person➞given name](person_given_name.md)  <sub>0..1</sub>
     * Description: First name.
     * Range: [String](types/String.md)
     * in subsets: (restricted)
 * [person➞family name](person_family_name.md)  <sub>0..1</sub>
     * Description: Last name.
     * Range: [String](types/String.md)
     * in subsets: (restricted)
 * [person➞additional name](person_additional_name.md)  <sub>0..1</sub>
     * Description: Additional name(s).
     * Range: [String](types/String.md)
     * in subsets: (restricted)

### Inherited from named thing:

 * [named thing➞id](named_thing_id.md)  <sub>1..1</sub>
     * Description: The internal unique identifier for an entity.
     * Range: [String](types/String.md)
     * in subsets: (restricted)
 * [named thing➞alias](named_thing_alias.md)  <sub>1..1</sub>
     * Description: The alias (alternate identifier) for an entity.
     * Range: [String](types/String.md)
     * in subsets: (restricted)
 * [named thing➞xref](named_thing_xref.md)  <sub>0..\*</sub>
     * Description: Holds one or more database cross references for an entity.
     * Range: [String](types/String.md)

## Other properties

|  |  |  |
| --- | --- | --- |
| **Exact Mappings:** | | NCIT:C25190 |
|  | | SIO:000498 |
|  | | prov:Person |
