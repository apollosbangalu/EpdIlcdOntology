# EPD+ILCD Dataset Ontology

## Overview
The Environmental Product Declaration (EPD) and International Life Cycle Data (ILCD) Dataset Ontology is a semantic web knowledge model for representing environmental product declarations of building materials and products within the construction industry. Version 0.1 of this ontology provides a comprehensive framework for describing environmental impacts, life cycle assessments, and related properties according to the EPD+ILCD format.

## License
This ontology is licensed under [Creative Commons Attribution 4.0 International License](https://creativecommons.org/licenses/by/4.0/).

## Authors
- Creator: Bangalu Apollos Yohanna https://dc.rwth-aachen.de/en/apollos-bangalu-2/
- Contributor: Univ.-Prof. Dr.Jakob Beetz Jakob Beetz https://dc.rwth-aachen.de/en/jakob-beetz-2/

## Description
The ontology provides a taxonomy and vocabulary to describe Environmental Product Declarations of building materials and products, with their corresponding properties and individuals relevant within the construction industry. It follows the EPD+ILCD Format to enable semantic interoperability solutions within the knowledge domain. This ontology is developed strictly for research purposes.

## Key Features
- Comprehensive environmental impact indicator representation
- Detailed life cycle assessment structure
- Administrative and validation information framework
- Hierarchical classification system for building materials
- Standardised units and measurements
- Process data set management

## Core Components

### 1. Main Classes
- **BuildingProductOrMaterial**: Root class for building products and materials
- **ProcessDataSet**: Container for EPD process information
- **EnvironmentalIndicator**: Framework for environmental impact measurements
- **AdministrativeInformation**: Management of metadata and ownership
- **ClassificationOrCategory**: Hierarchical classification structure

### 2. Environmental Indicators
#### Core Indicators
- Global Warming Potential (GWP)
- Ozone Depletion Potential (ODP)
- Acidification Potential (AP)
- Eutrophication Potential (EP)
- Photochemical Ozone Creation Potential (POCP)

#### Resource Use Indicators
- Use of renewable primary energy (PERE)
- Use of non-renewable primary energy (PENRE)
- Use of secondary materials (SM)
- Use of water resources (FW)

#### Waste Categories
- Hazardous waste disposed (HWD)
- Non-hazardous waste disposed (NHWD)
- Radioactive waste disposed (RWD)

### 3. Life Cycle Phases
- Raw Material Supply (A1)
- Transport (A2)
- Manufacturing (A3)
- Construction Process (A4-A5)
- Use Stage (B1-B7)
- End of Life (C1-C4)
- Benefits and Loads Beyond System Boundary (D)

## Usage

### Ontology URI
```
http://www.EpdLcaOntlogy.com/EpdLcaDataSetOntology
```

### Preferred Namespace
```
@prefix epd: <http://www.EpdLcaOntlogy.com/EpdLcaDataSetOntology/>
```

### Required Dependencies
- RDF/XML syntax
- OWL DL expressivity
- Dublin Core terms vocabulary

## Implementation

### Data Properties
The ontology includes numerous data properties for capturing specific information:
- Administrative details
- Classification information
- Environmental measurements
- Temporal aspects
- Geographic information
- Technical specifications

### Object Properties
Key object properties include:
- hasProcessDataSet
- hasEnvironmentalIndicator
- hasLifeCyclePhase
- hasAdministrativeInformation
- hasClassificationOrCategory

## Documentation Structure

### Class Hierarchy
The ontology maintains a clear hierarchical structure for:
- Building materials and products
- Environmental indicators
- Administrative information
- Process data
- Life cycle phases

### Property Documentation
Each property includes:
- Domain and range specifications
- Label and comment annotations
- Usage examples where applicable

## SPARQL QUERY SAMPLES
- see the text file

## Integration Guidelines

### 1. Data Import
- Use standard RDF/OWL tools for ontology import
- Maintain namespace consistency
- Verify property constraints

### 2. Data Validation
- Check compliance with EPD+ILCD format
- Verify required properties
- Validate measurement units

### 3. Classification Implementation
- Follow hierarchical structure
- Use appropriate classification levels
- Maintain consistent naming conventions

## Best Practices

### 1. Data Entry
- Provide complete administrative information
- Use standardized units
- Include validation data
- Document data sources

### 2. Classification
- Use most specific category available
- Maintain hierarchical relationships
- Document classification decisions

### 3. Environmental Data
- Include all relevant indicators
- Provide complete life cycle data
- Document calculation methods

## Technical Requirements

### Software Support
- OWL 2 compliant tools
- RDF triple stores
- SPARQL query support

### Format Compatibility
- RDF/XML
- Turtle
- JSON-LD
- N-Triples

## Future Development

### Planned Enhancements
- Extended environmental indicators
- Additional classification categories
- Enhanced validation framework
- Improved data quality metrics

### Community Contribution
- Issue reporting guidelines
- Contribution process
- Documentation updates

## Support and Contact
For questions and support regarding the ontology, please contact the authors or raise issues through appropriate channels.

## Changelog
### Version 0.1
- Initial release
- Core ontology structure
- Basic environmental indicators
- Administrative framework
- Classification system

## Citation
When using this ontology, please cite:
```
EPD+ILCD Dataset Ontology v0.1
Creator: Bangalu Apollos Yohanna
Contributor: Univ.-Prof. Dr. Jakob Beetz
License: CC BY 4.0
```

## Acknowledgments
- Special thanks to contributors and organisations supporting the development of this ontology.

- Ecoplatorm https://www.eco-platform.org/epd-data.html
- EPD Danmark https://ecosmdp-prod.eco-platform.org/
- Ireland's EPD Platform https://www.igbc.ie/epd-home
- Kiwa https://www.kiwa.com/de/en/
- EPD Italy https://node.epditaly.it/
- DAPCONS Programa DAPconstrucción http://soda.dapcons.com:8080/
- BRE https://bregroup.com/services/standards/environmental/en-15804-environmental-product-declaration-epd
- International EPD System https://environdec.com/home
- EPD-Norge Digi https://digi.epd-norge.no/

-  The authors would like to thank Silvio Peroni for developing LODE, a Live OWL Documentation Environment, which is used for representing the Cross Referencing Section of this document and Daniel Garijo for developing Widoco, the program used to create the template used in this documentation.
