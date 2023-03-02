
# Class: data access committee


A group of members that are delegated to grant access to one or more datasets after ensuring the minimum criteria for data sharing has been met, and request for data use does not raise ethical and/or legal concerns.

URI: [GHGA:DataAccessCommittee](https://w3id.org/GHGA/DataAccessCommittee)


[![img](https://yuml.me/diagram/nofunky;dir:TB/class/[Submission],[Member],[EgaAccessionMixin],[DataAccessPolicy],[Member]<has%20member%200..*-++[DataAccessCommittee&#124;name:string%20%3F;description:string;accession:string;ega_accession:string;id(i):string;alias(i):string;xref(i):string%20%2B;creation_date(i):string;update_date(i):string;schema_type(i):string;schema_version(i):string],[Member]<main%20contact%201..1-++[DataAccessCommittee],[DataAccessPolicy]++-%20has%20data%20access%20committee%201..1>[DataAccessCommittee],[DataAccessPolicy]-%20has%20data%20access%20committee(i)%200..1>[DataAccessCommittee],[Submission]-%20has%20data%20access%20committee(i)%200..1>[DataAccessCommittee],[Submission]++-%20has%20data%20access%20committee%201..*>[DataAccessCommittee],[DataAccessCommittee]uses%20-.->[AttributeMixin],[DataAccessCommittee]uses%20-.->[AccessionMixin],[DataAccessCommittee]uses%20-.->[EgaAccessionMixin],[Committee]^-[DataAccessCommittee],[Committee],[AttributeMixin],[Attribute],[AccessionMixin])](https://yuml.me/diagram/nofunky;dir:TB/class/[Submission],[Member],[EgaAccessionMixin],[DataAccessPolicy],[Member]<has%20member%200..*-++[DataAccessCommittee&#124;name:string%20%3F;description:string;accession:string;ega_accession:string;id(i):string;alias(i):string;xref(i):string%20%2B;creation_date(i):string;update_date(i):string;schema_type(i):string;schema_version(i):string],[Member]<main%20contact%201..1-++[DataAccessCommittee],[DataAccessPolicy]++-%20has%20data%20access%20committee%201..1>[DataAccessCommittee],[DataAccessPolicy]-%20has%20data%20access%20committee(i)%200..1>[DataAccessCommittee],[Submission]-%20has%20data%20access%20committee(i)%200..1>[DataAccessCommittee],[Submission]++-%20has%20data%20access%20committee%201..*>[DataAccessCommittee],[DataAccessCommittee]uses%20-.->[AttributeMixin],[DataAccessCommittee]uses%20-.->[AccessionMixin],[DataAccessCommittee]uses%20-.->[EgaAccessionMixin],[Committee]^-[DataAccessCommittee],[Committee],[AttributeMixin],[Attribute],[AccessionMixin])

## Parents

 *  is_a: [Committee](Committee.md) - A group of people organized for a specific purpose.

## Uses Mixin

 *  mixin: [AttributeMixin](AttributeMixin.md) - Mixin for entities that can have one or more attributes.
 *  mixin: [AccessionMixin](AccessionMixin.md) - Mixin for entities that can be assigned a GHGA accession.
 *  mixin: [EgaAccessionMixin](EgaAccessionMixin.md) - Mixin for entities that can be assigned an EGA accession, in addition to GHGA accession.

## Referenced by Class

 *  **[DataAccessPolicy](DataAccessPolicy.md)** *[data access policy➞has data access committee](data_access_policy_has_data_access_committee.md)*  <sub>1..1</sub>  **[DataAccessCommittee](DataAccessCommittee.md)**
 *  **None** *[has data access committee](has_data_access_committee.md)*  <sub>0..1</sub>  **[DataAccessCommittee](DataAccessCommittee.md)**
 *  **[Submission](Submission.md)** *[submission➞has data access committee](submission_has_data_access_committee.md)*  <sub>1..\*</sub>  **[DataAccessCommittee](DataAccessCommittee.md)**

## Attributes


### Own

 * [name](name.md)  <sub>0..1</sub>
     * Description: The name for an entity.
     * Range: [String](types/String.md)
 * [data access committee➞description](data_access_committee_description.md)  <sub>1..1</sub>
     * Description: A description for the Data Access Committee.
     * Range: [String](types/String.md)
 * [data access committee➞main contact](data_access_committee_main_contact.md)  <sub>1..1</sub>
     * Description: The main contact for the Data Access Committee.
     * Range: [Member](Member.md)
     * in subsets: (restricted)
 * [data access committee➞has member](data_access_committee_has_member.md)  <sub>0..\*</sub>
     * Description: All the members that are part of this Data Access Committee.
     * Range: [Member](Member.md)
 * [data access committee➞name](data_access_committee_name.md)  <sub>1..1</sub>
     * Description: The name for the Data Access Committee.
     * Range: [String](types/String.md)

### Inherited from committee:

 * [named thing➞id](named_thing_id.md)  <sub>1..1</sub>
     * Description: The internal unique identifier for an entity.
     * Range: [String](types/String.md)
     * in subsets: (restricted)
 * [named thing➞alias](named_thing_alias.md)  <sub>1..1</sub>
     * Description: The alias (alternate identifier) for an entity.
     * Range: [String](types/String.md)
     * in subsets: (restricted)
 * [named thing➞xref](named_thing_xref.md)  <sub>1..\*</sub>
     * Description: Holds one or more database cross references for an entity.
     * Range: [String](types/String.md)
 * [named thing➞creation date](named_thing_creation_date.md)  <sub>1..1</sub>
     * Description: Timestamp (in ISO 8601 format) when the entity was created.
     * Range: [String](types/String.md)
 * [named thing➞update date](named_thing_update_date.md)  <sub>1..1</sub>
     * Description: Timestamp (in ISO 8601 format) when the entity was updated.
     * Range: [String](types/String.md)

### Mixed in from attribute mixin:

 * [attribute mixin➞has attribute](attribute_mixin_has_attribute.md)  <sub>1..\*</sub>
     * Description: Key/value pairs corresponding to an entity.
     * Range: [Attribute](Attribute.md)
     * in subsets: (restricted)

### Mixed in from accession mixin:

 * [accession mixin➞accession](accession_mixin_accession.md)  <sub>1..1</sub>
     * Description: A unique GHGA identifier assigned to an entity for the sole purpose of referring to that entity in a global scope.
     * Range: [String](types/String.md)

### Mixed in from ega accession mixin:

 * [ega accession mixin➞ega accession](ega_accession_mixin_ega_accession.md)  <sub>1..1</sub>
     * Description: A unique European Genome-Phenome Archive (EGA) identifier assigned to an entity for the sole purpose of referring to that entity within the EGA federated network.
     * Range: [String](types/String.md)