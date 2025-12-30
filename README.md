# Bhutan Notable Waterbirds

A collaborative repository for verifying and maintaining a verified list of notable, rare, or first-record waterbird sightings in Bhutan.

## Purpose

This repository establishes a standardized workflow for the Ugyen Wangchuck Institute of Conservation and Environment (UWICE) team to submit, review, and officially record significant waterbird sightings in Bhutan. The system ensures data integrity, creates a verifiable record of first-of-its-kind sightings, and contributes to the long-term dataset on waterbird diversity and climate change impacts.

## Workflow

1. **Submit a sighting**: Use the [Notable Waterbird Sighting issue template](.github/ISSUE_TEMPLATE/notable_sighting.yml) to open a new issue with all relevant details (date, species, location, observer, evidence, notes). The issue will be labeled `status:pending-review` and assigned to a verifier.

2. **Review**: A verifier (typically a UWICE member) reviews the submission, checks evidence, and may request additional information. Once verified, the verifier creates a new branch, adds the sighting to `verified_sightings.csv`, and opens a pull request referencing the issue.

3. **Integration**: The pull request is reviewed and merged (squash merge) into the main dataset. The original issue is closed with a comment referencing the commit and labeled `status:verified-added`.

## Data Structure

The primary dataset is `verified_sightings.csv` with the following columns:

- `SightingID`: Unique identifier (e.g., UWICE-001)
- `DateOfSighting`: YYYY-MM-DD
- `CommonName`: Common name of the species
- `ScientificName`: Scientific name
- `Location`: Specific location description
- `ObserverName`: Name(s) of the observer(s)
- `VerifierName`: Name of the verifier who confirmed the sighting
- `Notes`: Additional information (plumage, behavior, conservation notes, etc.)

## Example

See issue #1 and pull request #1 for a demonstration of the workflow using a hypothetical Ferruginous Pochard sighting.

## Contributing

Members of UWICE and authorized collaborators are welcome to submit sightings. Please ensure you have appropriate evidence (photographs, audio recordings, detailed field notes) to support the submission.