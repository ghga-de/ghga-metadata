
# Class: Experiment


An Experiment is an investigation that consists of a coordinated set of actions and observations designed to generate data with the goal of verifying, falsifying, or establishing the validity of a hypothesis.

URI: [GHGA:Experiment](https://w3id.org/GHGA/Experiment)


[![img](https://yuml.me/diagram/nofunky;dir:TB/class/[Submission],[Sample],[ResearchDataFile],[IdentifiedByAliasMixin],[ExperimentalMethod],[ExperimentalMethod]<experimental_methods%201..*-%20[Experiment&#124;title:string;description:string;type:string%20%3F;alias:string],[ResearchDataFile]<research_data_files%201..*-%20[Experiment],[Sample]<samples%201..*-%20[Experiment],[Submission]++-%20experiments%201..*>[Experiment],[Submission]-%20experiments(i)%200..*>[Experiment],[Experiment]uses%20-.->[IdentifiedByAliasMixin],[Experiment]uses%20-.->[AttributeMixin],[AttributeMixin],[Attribute])](https://yuml.me/diagram/nofunky;dir:TB/class/[Submission],[Sample],[ResearchDataFile],[IdentifiedByAliasMixin],[ExperimentalMethod],[ExperimentalMethod]<experimental_methods%201..*-%20[Experiment&#124;title:string;description:string;type:string%20%3F;alias:string],[ResearchDataFile]<research_data_files%201..*-%20[Experiment],[Sample]<samples%201..*-%20[Experiment],[Submission]++-%20experiments%201..*>[Experiment],[Submission]-%20experiments(i)%200..*>[Experiment],[Experiment]uses%20-.->[IdentifiedByAliasMixin],[Experiment]uses%20-.->[AttributeMixin],[AttributeMixin],[Attribute])

## Uses Mixin

 *  mixin: [IdentifiedByAliasMixin](IdentifiedByAliasMixin.md)
 *  mixin: [AttributeMixin](AttributeMixin.md) - Mixin for entities that can have one or more attributes.

## Referenced by Class

 *  **[Submission](Submission.md)** *[Submission➞experiments](Submission_experiments.md)*  <sub>1..\*</sub>  **[Experiment](Experiment.md)**
 *  **None** *[experiment](experiment.md)*  <sub>0..1</sub>  **[Experiment](Experiment.md)**
 *  **None** *[experiments](experiments.md)*  <sub>0..\*</sub>  **[Experiment](Experiment.md)**

## Attributes


### Own

 * [Experiment➞title](Experiment_title.md)  <sub>1..1</sub>
     * Description: The title for this Sequencing Experiment (e.g., GHGAE_PBMC_RNAseq).
     * Range: [String](types/String.md)
 * [Experiment➞description](Experiment_description.md)  <sub>1..1</sub>
     * Description: A detailed description of this Sequencing Experiment.
     * Range: [String](types/String.md)
 * [Experiment➞type](Experiment_type.md)  <sub>0..1</sub>
     * Description: The type of this Sequencing Experiment.
     * Range: [String](types/String.md)
 * [Experiment➞samples](Experiment_samples.md)  <sub>1..\*</sub>
     * Description: One or more Samples that associated with this Experiment.
     * Range: [Sample](Sample.md)
 * [Experiment➞research_data_files](Experiment_research_data_files.md)  <sub>1..\*</sub>
     * Description: One or more Research Data Files that are associated with this Experiment.
     * Range: [ResearchDataFile](ResearchDataFile.md)
 * [Experiment➞experimental_methods](Experiment_experimental_methods.md)  <sub>1..\*</sub>
     * Description: One or more Experimental Methods that are associated with this Experiment.
     * Range: [ExperimentalMethod](ExperimentalMethod.md)

### Mixed in from IdentifiedByAliasMixin:

 * [IdentifiedByAliasMixin➞alias](IdentifiedByAliasMixin_alias.md)  <sub>1..1</sub>
     * Description: The alias for an entity at the time of submission.
     * Range: [String](types/String.md)

### Mixed in from AttributeMixin:

 * [AttributeMixin➞attributes](AttributeMixin_attributes.md)  <sub>0..\*</sub>
     * Description: Key/value pairs corresponding to an entity.
     * Range: [Attribute](Attribute.md)

## Other properties

|  |  |  |
| --- | --- | --- |
| **Exact Mappings:** | | SIO:000994 |
