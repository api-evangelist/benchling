# Benchling

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

Benchling is a life sciences R&D cloud platform offering a comprehensive REST API for programmatically managing molecular biology entities, assay results and runs, electronic lab notebook entries, DNA/RNA/protein sequences, inventory, and experiment workflows. The API enables integrations with lab instruments, ERP systems, LIMS, and external databases, as well as bulk data ingest/export and event-driven automation via webhooks and AWS EventBridge. API access is available to Professional and Enterprise tenants and supports user API keys, OAuth 2.0 client credentials, and OIDC authentication.

**Areas:** Life Sciences · Biotechnology · R&D · Molecular Biology · Laboratory Information Management · Electronic Lab Notebook · Assay Management · Inventory · Sequence Management · Experiment Workflows · REST · Webhook

## Benchling on APIs.io

Everything profiled for Benchling is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/benchling/](https://apis.io/providers/benchling/)** — or go straight to one of the APIs or properties below.

### APIs (203)

- [Benchling AA Sequences API](https://apis.io/apis/benchling/benchling-aa-sequences-api/) — AA Sequences are the working units of cells that make everything run (they help make structures, catalyze reactions and allow for signaling - a kind of…
- [Benchling Apps API](https://apis.io/apis/benchling/benchling-apps-api/) — Create and manage Benchling apps on your tenant
- [Benchling Assay Results API](https://apis.io/apis/benchling/benchling-assay-results-api/) — Results represent the output of assays that have been performed. You can customize the schemas of results to fit your needs. Results can link to runs,…
- [Benchling Assay Runs API](https://apis.io/apis/benchling/benchling-assay-runs-api/) — Runs capture the details / parameters of a run that was performed. Results are usually nested under a run.
- [Benchling Audit API](https://apis.io/apis/benchling/benchling-audit-api/) — Export audit log data for Benchling objects.
- [Benchling Authentication API](https://apis.io/apis/benchling/benchling-authentication-api/) — Endpoints to help authenticate with the rest of the API resources.
- [Benchling Blobs API](https://apis.io/apis/benchling/benchling-blobs-api/) — Blobs are opaque files that can be linked to other items in Benchling, like assay runs or results. For example, you can upload a blob, then upload an assay…
- [Benchling Boxes API](https://apis.io/apis/benchling/benchling-boxes-api/) — Boxes are a structured inventory type, consisting of a grid of positions that can each hold one container. Unlike locations, there are a maximum number of…
- [Benchling Codon Usage Tables API](https://apis.io/apis/benchling/benchling-codon-usage-tables-api/) — Benchling curates codon usage data for a variety of organisms to support operations such as Codon Optimization and Back Translation.
- [Benchling Connect API](https://apis.io/apis/benchling/benchling-connect-api/) — Connect endpoints support Benchling Connect actions, like instrument data conversion.
- [Benchling Containers API](https://apis.io/apis/benchling/benchling-containers-api/) — Containers are the backbone of sample management in Benchling. They represent physical containers, such as tubes or wells, that hold quantities of…
- [Benchling Custom Entities API](https://apis.io/apis/benchling/benchling-custom-entities-api/) — Benchling supports custom entities for biological entities that are neither DNA, RNA, nor AA sequences. Custom entities must have an entity schema set and…
- [Benchling Custom Notations API](https://apis.io/apis/benchling/benchling-custom-notations-api/) — Benchling allows users to configure their own fully-custom string representation formats for import/export of nucleotide sequences (including chemical…
- [Benchling Data Frames API](https://apis.io/apis/benchling/benchling-data-frames-api/) — Data frames in Benchling represent tabular data that is not schematized. They contain columns with defined types and rows of data. Data frames are primarily…
- [Benchling Datasets API](https://apis.io/apis/benchling/benchling-datasets-api/) — Similar to Data frames, datasets in Benchling represent tabular data that is not schematized. Datasets are saved to folders within Benchling with additional…
- [Benchling DNA Alignments API](https://apis.io/apis/benchling/benchling-dna-alignments-api/) — A DNA alignment is a Benchling object representing an alignment of multiple DNA sequences. This endpoint is deprecated, please migrate to the existing…
- [Benchling DNA Oligos API](https://apis.io/apis/benchling/benchling-dna-oligos-api/) — DNA Oligos are short linear DNA sequences that can be attached as primers to full DNA sequences. Just like other entities, they support schemas, tags, and…
- [Benchling DNA Sequences API](https://apis.io/apis/benchling/benchling-dna-sequences-api/) — DNA sequences are the bread and butter of the Benchling Molecular Biology suite. On Benchling, these are comprised of a string of nucleotides and…
- [Benchling Dropdowns API](https://apis.io/apis/benchling/benchling-dropdowns-api/) — Dropdowns are registry-wide enums. Use dropdowns to standardize on spelling and naming conventions, especially for important metadata like resistance markers.
- [Benchling Entities API](https://apis.io/apis/benchling/benchling-entities-api/) — Entities include DNA and AA sequences, oligos, molecules, custom entities, and other biological objects in Benchling. Entities support schemas, tags, and…
- [Benchling Entries API](https://apis.io/apis/benchling/benchling-entries-api/) — Entries are rich text documents that allow you to capture all of your experimental data in one place.
- [Benchling Enzymes API](https://apis.io/apis/benchling/benchling-enzymes-api/) — Restriction enzymes are curated by Benchling for operations such as Digests and Codon Optimization.
- [Benchling Events API](https://apis.io/apis/benchling/benchling-events-api/) — The Events system allows external services to subscribe to events that are triggered in Benchling (e.g. plasmid registration, request submission, etc).
- [Benchling Exports API](https://apis.io/apis/benchling/benchling-exports-api/) — Export a Notebook Entry or a Legacy Workflow Stage Entry.
- [Benchling Feature Libraries API](https://apis.io/apis/benchling/benchling-feature-libraries-api/) — Feature Libraries are collections of shared canonical patterns that can be used to generate annotations on matching regions of DNA Sequences or AA Sequences.
- [Benchling Files API](https://apis.io/apis/benchling/benchling-files-api/) — Files are Benchling objects that represent files and their metadata. Compared to Blobs, which are used by most Benchling products for attachments, Files are…
- [Benchling Folders API](https://apis.io/apis/benchling/benchling-folders-api/) — Folders are nested within projects to provide additional organization.
- [Benchling Instrument Queries API](https://apis.io/apis/benchling/benchling-instrument-queries-api/) — Instrument Queries are used to query the instrument service.
- [Benchling Inventory API](https://apis.io/apis/benchling/benchling-inventory-api/) — Manage inventory wide objects.
- [Benchling Lab Automation API](https://apis.io/apis/benchling/benchling-lab-automation-api/) — Lab Automation endpoints support integration with lab instruments, and liquid handlers to create samples or results, and capture transfers between…
- [Benchling Label Templates API](https://apis.io/apis/benchling/benchling-label-templates-api/) — List label templates.
- [Benchling Legacy Requests API](https://apis.io/apis/benchling/benchling-legacy-requests-api/) — Legacy Requests allow scientists and teams to collaborate around experimental assays and workflows.
- [Benchling Legacy Workflows API](https://apis.io/apis/benchling/benchling-legacy-workflows-api/) — Legacy Workflows allow orchestrating complex experiments.
- [Benchling Legacy Workflows (deprecated) API](https://apis.io/apis/benchling/benchling-legacy-workflows-deprecated-api/) — Please use endpoints for Legacy Workflows. These deprecated endpoints will be removed once users are migrated onto Legacy Workflows endpoints.
- [Benchling Locations API](https://apis.io/apis/benchling/benchling-locations-api/) — Manage locations objects. Like all inventory, every Location has a barcode that is unique across the registry.
- [Benchling Mixtures API](https://apis.io/apis/benchling/benchling-mixtures-api/) — Mixtures are solutions comprised of multiple ingredients where the exact quantities of each ingredient are important to track. Each ingredient is uniquely…
- [Benchling Molecules API](https://apis.io/apis/benchling/benchling-molecules-api/) — Molecules are groups of atoms held together by bonds, representing entities smaller than DNA Sequences and AA Sequences. Just like other entities, they…
- [Benchling Monomers API](https://apis.io/apis/benchling/benchling-monomers-api/) — Monomers are chemical building blocks with specified structures used to compose modified nucleotides. Note that monomer write endpoints require tenant admin…
- [Benchling Nucleotide Alignments API](https://apis.io/apis/benchling/benchling-nucleotide-alignments-api/) — A Nucleotide Alignment is a Benchling object representing an alignment of multiple DNA and/or RNA sequences.
- [Benchling Oligos API](https://apis.io/apis/benchling/benchling-oligos-api/) — Oligos are short linear DNA sequences that can be attached as primers to full DNA sequences. Just like other entities, they support schemas, tags, and…
- [Benchling Organizations API](https://apis.io/apis/benchling/benchling-organizations-api/) — View organization objects.
- [Benchling Plates API](https://apis.io/apis/benchling/benchling-plates-api/) — Plates are a structured inventory type, grids of wells that each function like containers. Plates come in two types: a traditional "fixed" type, where the…
- [Benchling Printers API](https://apis.io/apis/benchling/benchling-printers-api/) — List printers.
- [Benchling Projects API](https://apis.io/apis/benchling/benchling-projects-api/) — Manage project objects.
- [Benchling Registry API](https://apis.io/apis/benchling/benchling-registry-api/) — Manage registry objects. See our documentation on [how to register entities](https://docs.benchling.com/docs/registering-entities).
- [Benchling RNA Oligos API](https://apis.io/apis/benchling/benchling-rna-oligos-api/) — RNA Oligos are short linear RNA sequences that can be attached as primers to full DNA sequences. Just like other entities, they support schemas, tags, and…
- [Benchling RNA Sequences API](https://apis.io/apis/benchling/benchling-rna-sequences-api/) — Chains of linear, single stranded RNA that support most capabilities and attributes of DNA Sequences.
- [Benchling Schemas API](https://apis.io/apis/benchling/benchling-schemas-api/) — Schemas represent custom configuration of objects in Benchling. See this [guide in our documentation](https://docs.benchling.com/docs/schemas) on how…
- [Benchling Tasks API](https://apis.io/apis/benchling/benchling-tasks-api/) — Endpoints that perform expensive computations launch long-running tasks. These endpoints return the task ID (a UUID) in the response body. After launching a…
- [Benchling Teams API](https://apis.io/apis/benchling/benchling-teams-api/) — View team objects.
- [Benchling Users API](https://apis.io/apis/benchling/benchling-users-api/) — Manage user objects.
- [Benchling Warehouse API](https://apis.io/apis/benchling/benchling-warehouse-api/) — Manage warehouse credentials.
- [Benchling Workflow Flowchart Config Versions API](https://apis.io/apis/benchling/benchling-workflow-flowchart-config-versions-api/) — Workflow flowchart config versions are versioned graphs of flowchart configurations.
- [Benchling Workflow Flowcharts API](https://apis.io/apis/benchling/benchling-workflow-flowcharts-api/) — Workflow flowcharts represent the nodes and edges that a flowchart is comprised of.
- [Benchling Workflow Outputs API](https://apis.io/apis/benchling/benchling-workflow-outputs-api/) — Workflow outputs are outputs of a workflow task
- [Benchling Workflow Task Groups API](https://apis.io/apis/benchling/benchling-workflow-task-groups-api/) — Workflow task groups are groups of workflow tasks of the same schema
- [Benchling Workflow Tasks API](https://apis.io/apis/benchling/benchling-workflow-tasks-api/) — Workflow tasks encapsulate a single unit of work
- [Benchling Aa Sequence API](https://apis.io/apis/benchling/benchling-aasequence-api/) — Represents an amino acid sequence in Benchling's molecular biology platform. An AaSequence stores the one-letter amino acid code string along with…
- [Benchling Aa Sequence Schema API](https://apis.io/apis/benchling/benchling-aasequenceschema-api/) — Defines the structure, field definitions, and configuration options for AA sequences.
- [Benchling Agent API](https://apis.io/apis/benchling/benchling-agent-api/) — The Agent API from Benchling — 1 operation(s) for agent.
- [Benchling Analysis API](https://apis.io/apis/benchling/benchling-analysis-api/) — Operations for Analysis
- [Benchling Analysis Template API](https://apis.io/apis/benchling/benchling-analysistemplate-api/) — A reusable pipeline configuration that can be instantiated to create new Analysis objects. AnalysisTemplates define a complete data processing workflow with…
- [Benchling Analysis Template Data Frame Variable API](https://apis.io/apis/benchling/benchling-analysistemplatedataframevariable-api/) — Defines a data frame placeholder within an AnalysisTemplate that users must provide when applying the template. Each variable specifies which PipelineStep…
- [Benchling Analysis Template Variable API](https://apis.io/apis/benchling/benchling-analysistemplatevariable-api/) — Defines a configuration parameter within an AnalysisTemplate that users can customize when applying the template. Unlike AnalysisTemplateDataFrameVariable…
- [Benchling App Canvas API](https://apis.io/apis/benchling/benchling-appcanvas-api/) — Represents a Benchling App canvas, an embedded UI surface that apps use to render custom interactive content within notebook entries, entry templates, assay…
- [Benchling App Config Value API](https://apis.io/apis/benchling/benchling-appconfigvalue-api/) — Represents a configured value for a Benchling App on a specific tenant. Each config value has a path identifying its location in the configuration hierarchy…
- [Benchling App Session API](https://apis.io/apis/benchling/benchling-appsession-api/) — Represents a running or completed session for a Benchling App. App sessions track long-running app operations, providing status updates and user-facing…
- [Benchling Assembly API](https://apis.io/apis/benchling/benchling-assembly-api/) — Represents a molecular cloning assembly that combines multiple DNA fragments into complete constructs. Assemblies model the process of joining fragment…
- [Benchling Box API](https://apis.io/apis/benchling/benchling-box-api/) — A Box is a grid-based storage container in Benchling's inventory system, designed to hold multiple sample containers (tubes, vials, etc.) in an organized…
- [Benchling Box Schema API](https://apis.io/apis/benchling/benchling-boxschema-api/) — Defines the structure and constraints for a category of Boxes in Benchling's inventory system. A BoxSchema specifies the grid dimensions (height and width)…
- [Benchling Chart API](https://apis.io/apis/benchling/benchling-chart-api/) — A Chart is a data visualization within Benchling. Charts can be created directly (for example, via APIs or the UI) or generated from other workflows. Charts…
- [Benchling Collaboration API](https://apis.io/apis/benchling/benchling-collaboration-api/) — A Collaboration indicates that a Principal or Group is granted a Policy on a Resource. Some Collaborations represent Ownership, while others indicate that a…
- [Benchling Config Import History Entry API](https://apis.io/apis/benchling/benchling-configimporthistoryentry-api/) — Records a configuration import operation from one Benchling tenant to another. Each entry captures the source tenant, target organization, who performed the…
- [Benchling Container API](https://apis.io/apis/benchling/benchling-container-api/) — A Container is a physical vessel (such as a tube, vial, or cryotube) that holds biological or chemical samples in Benchling's inventory system. Containers…
- [Benchling Container Schema API](https://apis.io/apis/benchling/benchling-containerschema-api/) — Defines the structure and metadata for a category of Containers in Benchling's inventory system. A `ContainerSchema` specifies the container type (e.g.,…
- [Benchling Custom Entity API](https://apis.io/apis/benchling/benchling-customentity-api/) — A flexible, user-defined entity type in Benchling's Registry. Unlike specialized entity types such as DnaSequence or Molecule, CustomEntities allow…
- [Benchling Custom Entity Schema API](https://apis.io/apis/benchling/benchling-customentityschema-api/) — Operations for CustomEntitySchema
- [Benchling Data Frame API](https://apis.io/apis/benchling/benchling-dataframe-api/) — `DataFrame` stores non-schematized tabular data, with Benchling-aware column types (see `DataFrameColumn`). Data frames are not searchable and lack their…
- [Benchling Dataset API](https://apis.io/apis/benchling/benchling-dataset-api/) — `Dataset` stores non-schematized tabular data, with Benchling-aware column types. Datasets are first-class, searchable, archivable folder items. A Dataset's…
- [Benchling Dna Oligo API](https://apis.io/apis/benchling/benchling-dnaoligo-api/) — Represents a short single-stranded DNA oligonucleotide in Benchling's molecular biology platform. DNA oligos are typically synthetic sequences used as…
- [Benchling Dna Oligo Schema API](https://apis.io/apis/benchling/benchling-dnaoligoschema-api/) — Defines the structure, field definitions, and configuration options for DNA oligos.
- [Benchling Dna Sequence API](https://apis.io/apis/benchling/benchling-dnasequence-api/) — Represents a DNA sequence in Benchling's molecular biology platform. A `DnaSequence` stores the nucleotide bases of the forward strand along with rich…
- [Benchling Dna Sequence Schema API](https://apis.io/apis/benchling/benchling-dnasequenceschema-api/) — Defines the structure, field definitions, and configuration options for DNA sequences.
- [Benchling Document Export API](https://apis.io/apis/benchling/benchling-documentexport-api/) — The DocumentExport API from Benchling — 3 operation(s) for documentexport.
- [Benchling Document Part API](https://apis.io/apis/benchling/benchling-documentpart-api/) — Represents an ordered piece of content within an entry, template, subtemplate, or document. Each document part wraps one content block and records its…
- [Benchling Dropdown API](https://apis.io/apis/benchling/benchling-dropdown-api/) — A configurable list of predefined values used for standardizing data entry in schema fields. Dropdowns provide controlled vocabulary choices that ensure…
- [Benchling Dropdown Link Field Definition API](https://apis.io/apis/benchling/benchling-dropdownlinkfielddefinition-api/) — A schema field definition that links to a dropdown for value selection. The `linkDefinition` field references the `Dropdown` configuration that defines the…
- [Benchling Dropdown Option API](https://apis.io/apis/benchling/benchling-dropdownoption-api/) — An individual selectable value within a Dropdown. Each DropdownOption represents one valid choice that users can select when populating a schema field…
- [Benchling Entity Schema API](https://apis.io/apis/benchling/benchling-entityschema-api/) — Defines the structure and behavior for a category of registered entities in Benchling. EntitySchemas specify the field definitions (see `fieldDefinitions`…
- [Benchling Entry API](https://apis.io/apis/benchling/benchling-entry-api/) — An Entry is the core document type in Benchling's Electronic Lab Notebook (ELN), used by scientists to record experimental work and observations. Entries…
- [Benchling Entry Schema API](https://apis.io/apis/benchling/benchling-entryschema-api/) — Defines a schema that can be applied to Entries to add structured metadata through custom fields. Entry schemas allow organizations to standardize the…
- [Benchling Entry Subtemplate API](https://apis.io/apis/benchling/benchling-entrysubtemplate-api/) — A reusable content block that can be inserted into `DocumentLike` objects. Subtemplates contain pre-defined note content (text, tables, etc.) that…
- [Benchling Entry Template API](https://apis.io/apis/benchling/benchling-entrytemplate-api/) — A template used to create new `DocumentLike` objects with pre-populated content and structure. `EntryTemplate`s contain boilerplate text, tables,…
- [Benchling Enzyme API](https://apis.io/apis/benchling/benchling-enzyme-api/) — Represents a restriction enzyme from Benchling's global catalog of commercially available enzymes. Restriction enzymes (also known as restriction…
- [Benchling Enzyme List API](https://apis.io/apis/benchling/benchling-enzymelist-api/) — Represents a user-curated collection of restriction enzymes for molecular cloning workflows. EnzymeLists allow users and organizations to organize commonly…
- [Benchling Equipment Schema API](https://apis.io/apis/benchling/benchling-equipmentschema-api/) — Defines the structure, field definitions, and configuration options for Equipments.
- [Benchling Event Subscription API](https://apis.io/apis/benchling/benchling-eventsubscription-api/) — Configures delivery of Benchling events to external systems via AWS EventBridge. Event subscriptions enable real-time integration by streaming events (such…
- [Benchling Feature Library API](https://apis.io/apis/benchling/benchling-featurelibrary-api/) — Represents a reusable collection of biological features for auto-annotating nucleotide and AA sequences. FeatureLibraries enable users to define common…
- [Benchling Feature Library Item API](https://apis.io/apis/benchling/benchling-featurelibraryitem-api/) — Represents a single feature definition within a FeatureLibrary used for auto-annotation. Each item defines a searchable pattern (nucleotide or amino acid…
- [Benchling Fieldset API](https://apis.io/apis/benchling/benchling-fieldset-api/) — A tenant-defined schema interface (also known as a "Fieldset") that groups related fields to be shared across multiple schemas. Fieldsets are created and…
- [Benchling File API](https://apis.io/apis/benchling/benchling-file-api/) — A File represents an uploaded document or data file that is surfaced in Benchling's Data Catalog for discovery and organization. Files are primarily created…
- [Benchling Folder API](https://apis.io/apis/benchling/benchling-folder-api/) — A hierarchical container for organizing entities, notebook entries, and other items within a Project. Folders support nested structures through parent-child…
- [Benchling Germline API](https://apis.io/apis/benchling/benchling-germline-api/) — A database of reference sequences used to characterize protein sequences via alignment.
- [Benchling Group Membership API](https://apis.io/apis/benchling/benchling-groupmembership-api/) — Indicates that a Principal is a member of Group. Role indicates that the Principal is a member of a subgroup, such as Admins of the Group. Teams are the…
- [Benchling Label Template API](https://apis.io/apis/benchling/benchling-labeltemplate-api/) — A `LabelTemplate` defines the format for printing physical labels for inventory items, such as containers, plates, and boxes. Each template contains a…
- [Benchling Legacy App Installation API](https://apis.io/apis/benchling/benchling-legacyappinstallation-api/) — Represents a legacy (pre-App Store) Benchling App installation on a tenant. Legacy apps are configured directly with webhook URLs and configuration specs…
- [Benchling Library Parameter Definition API](https://apis.io/apis/benchling/benchling-libraryparameterdefinition-api/) — A reusable parameter definition stored in the Parameter Library. LibraryParameterDefinitions allow organizations to standardize parameters used across…
- [Benchling Limits API](https://apis.io/apis/benchling/benchling-limits-api/) — The limits API from Benchling — 1 operation(s) for limits.
- [Benchling Location API](https://apis.io/apis/benchling/benchling-location-api/) — A Location represents a physical storage area in Benchling's inventory system, such as a freezer, refrigerator, shelf, room, or building. Locations form a…
- [Benchling Location Schema API](https://apis.io/apis/benchling/benchling-locationschema-api/) — Defines the structure and metadata for a category of Locations in Benchling's inventory system. A LocationSchema specifies schema field definitions for…
- [Benchling Matrix Plate API](https://apis.io/apis/benchling/benchling-matrixplate-api/) — A MatrixPlate is a rack-style storage plate where Containers (tubes, vials) can be inserted into and removed from grid positions. Unlike FixedPlate or…
- [Benchling Matrix Plate Schema API](https://apis.io/apis/benchling/benchling-matrixplateschema-api/) — Defines the structure and constraints for a category of MatrixPlates in Benchling's inventory system. A MatrixPlateSchema specifies the grid dimensions…
- [Benchling Mixture API](https://apis.io/apis/benchling/benchling-mixture-api/) — A Mixture is a formulation entity in Benchling that represents a combination of ingredients with specified amounts. Mixtures are commonly used for buffers,…
- [Benchling Mixture Schema API](https://apis.io/apis/benchling/benchling-mixtureschema-api/) — Defines the structure, field definitions, and configuration options for Mixtures.
- [Benchling Molecule API](https://apis.io/apis/benchling/benchling-molecule-api/) — A Molecule represents a small molecule chemical compound in Benchling that is imported either as a MolFile or using SMILES (Simplified Molecular Input Line…
- [Benchling Molecule Schema API](https://apis.io/apis/benchling/benchling-moleculeschema-api/) — Defines the structure, field definitions, and configuration options for Molecule schemas.
- [Benchling Nucleotide Alignment API](https://apis.io/apis/benchling/benchling-nucleotidealignment-api/) — Represents a multiple sequence alignment of nucleotide sequences (DNA or RNA). Nucleotide alignments are used to compare sequence reads against a reference…
- [Benchling Nucleotide Monomer API](https://apis.io/apis/benchling/benchling-nucleotidemonomer-api/) — A building block component of modified oligonucleotides, representing a sugar, phosphate, or base subunit. Monomers are the chemical units that assemble to…
- [Benchling Oligo Conjugate API](https://apis.io/apis/benchling/benchling-oligoconjugate-api/) — An oligo conjugate is a therapeutic modality consisting of a single-stranded oligonucleotide backbone with one or more attached conjugate molecules. Common…
- [Benchling Oligo Conjugate Schema API](https://apis.io/apis/benchling/benchling-oligoconjugateschema-api/) — Defines the structure, field definitions, and configuration options for Oligo Conjugates.
- [Benchling Oligo Duplex API](https://apis.io/apis/benchling/benchling-oligoduplex-api/) — An oligo duplex is a therapeutic modality consisting of two complementary oligonucleotide strands (forward and reverse) with optional conjugate molecules…
- [Benchling Oligo Duplex Schema API](https://apis.io/apis/benchling/benchling-oligoduplexschema-api/) — Defines the structure, field definitions, and configuration options for Oligo Duplexes.
- [Benchling Organization API](https://apis.io/apis/benchling/benchling-organization-api/) — Represents a group of users within Benchling, typically corresponding to a company, department, or research group. Organizations provide a many-to-many…
- [Benchling Pipeline Step Data API](https://apis.io/apis/benchling/benchling-pipelinestepdata-api/) — Represents actual data attached to an input or output slot of a PipelineStep during execution. Each PipelineStepData corresponds to a defined data shape…
- [Benchling Plate API](https://apis.io/apis/benchling/benchling-plate-api/) — A Plate is a legacy unified type representing both well plates and tube racks in Benchling's inventory system. The type field (see PlateType) indicates…
- [Benchling Plate Design Template API](https://apis.io/apis/benchling/benchling-platedesigntemplate-api/) — A named plate design template backed by a scratch plate that lives in a template collection. Plate design templates allow scratch plates to be organized and…
- [Benchling Plate Schema API](https://apis.io/apis/benchling/benchling-plateschema-api/) — Defines the structure and constraints for a category of Plates in Benchling's inventory system. A PlateSchema specifies the grid dimensions (height and…
- [Benchling Policy API](https://apis.io/apis/benchling/benchling-policy-api/) — Defines a named set of permissions that can be assigned to users or groups through collaborations. Policies contain PolicyStatements that specify allowed…
- [Benchling Prediction Batch API](https://apis.io/apis/benchling/benchling-predictionbatch-api/) — Represents an execution of a Model Hub model against multiple data inputs (resulting in multiple Predictions). A PredictionBatch tracks the input…
- [Benchling Prediction Job API](https://apis.io/apis/benchling/benchling-predictionjob-api/) — Represents a single prediction within a PredictionBatch. Each PredictionJob captures the input configuration for one prediction and its association with…
- [Benchling Printer API](https://apis.io/apis/benchling/benchling-printer-api/) — A Printer represents a network-connected label printer configured in Benchling for printing barcode labels on inventory items. Printers are associated with…
- [Benchling Procedure API](https://apis.io/apis/benchling/benchling-procedure-api/) — A reusable template that defines a structured experimental workflow. Procedures specify a sequence of method steps (see `ProcedureMethodDefinitionVersion`)…
- [Benchling Procedure Flowchart API](https://apis.io/apis/benchling/benchling-procedureflowchart-api/) — Contains the flowchart configuration for a Procedure or TemplateCollection. A ProcedureFlowchart acts as a container for flowchart versions (see…
- [Benchling Procedure Flowchart Config Version Proxy API](https://apis.io/apis/benchling/benchling-procedureflowchartconfigversionproxy-api/) — Represents a snapshot of a procedure's flowchart configuration at a specific point in time. The flowchart defines the structure of a procedure as a directed…
- [Benchling Procedure Flowchart Version API](https://apis.io/apis/benchling/benchling-procedureflowchartversion-api/) — An immutable snapshot of a procedure's flowchart structure at a specific point in time. Each version contains the complete graph of method steps (see…
- [Benchling Procedure Method Definition Version API](https://apis.io/apis/benchling/benchling-proceduremethoddefinitionversion-api/) — A versioned method within a procedure flowchart. Methods are the building blocks of procedures, representing discrete experimental operations that…
- [Benchling Procedure Method Execution Instance API](https://apis.io/apis/benchling/benchling-proceduremethodexecutioninstance-api/) — An instance of a method being executed within a procedure run. When a scientist runs a procedure, each method in the flowchart becomes a…
- [Benchling Procedure Method Execution Instance Association API](https://apis.io/apis/benchling/benchling-proceduremethodexecutioninstanceassociation-api/) — Links two method execution instances across procedure runs to represent an intended connection within a study. This allows scientists to coordinate their…
- [Benchling Procedure Parameter API](https://apis.io/apis/benchling/benchling-procedureparameter-api/) — Represents a parameter entity within a procedure template. Parameters define the data, materials, or equipment that scientists interact with during…
- [Benchling Procedure Parameter Confirmation Value API](https://apis.io/apis/benchling/benchling-procedureparameterconfirmationvalue-api/) — Records a scientist's confirmation of a parameter value during procedure execution. When running a procedure, scientists confirm that inputs (such as…
- [Benchling Procedure Parameter Measured Value API](https://apis.io/apis/benchling/benchling-procedureparametermeasuredvalue-api/) — Records the actual measured or observed value for a parameter during procedure execution. Scientists enter measured values after performing an experimental…
- [Benchling Procedure Parameter Planned Value API](https://apis.io/apis/benchling/benchling-procedureparameterplannedvalue-api/) — Stores the expected or planned value for a parameter, set during procedure setup or run planning. Used to specify anticipated inputs before execution…
- [Benchling Procedure Parameter Version API](https://apis.io/apis/benchling/benchling-procedureparameterversion-api/) — A versioned definition of a procedure parameter. Each version specifies the parameter's name, description, data type configuration (`dataType`), and how…
- [Benchling Procedure Run API](https://apis.io/apis/benchling/benchling-procedurerun-api/) — An active execution of a procedure template. Created when scientists start running an experiment based on a `Procedure`. Contains experimental conditions…
- [Benchling Procedure Run Condition API](https://apis.io/apis/benchling/benchling-procedureruncondition-api/) — A ProcedureRunCondition represents a configuration of the methods of a Procedure that is being executed within a ProcedureRun. The values associated with…
- [Benchling Procedure Run Condition Replicate API](https://apis.io/apis/benchling/benchling-procedurerunconditionreplicate-api/) — A replicate of a `ProcedureRunCondition`, representing one execution of a condition's configuration. Scientists often run the same experimental condition…
- [Benchling Procedure Run Plan API](https://apis.io/apis/benchling/benchling-procedurerunplan-api/) — A draft experiment plan that can be promoted to a `ProcedureRun` for execution. Scientists use run plans to configure experimental conditions, parameter…
- [Benchling Procedure Run Plan Condition API](https://apis.io/apis/benchling/benchling-procedurerunplancondition-api/) — A planned experimental condition within a `ProcedureRunPlan`, representing how a procedure's methods will be configured when the plan is promoted to an…
- [Benchling Procedure Step Definition Version API](https://apis.io/apis/benchling/benchling-procedurestepdefinitionversion-api/) — A versioned definition of a procedure step within a procedure flowchart. Steps represent documentation or instructions that guide scientists through a…
- [Benchling Procedure Step Execution Instance API](https://apis.io/apis/benchling/benchling-procedurestepexecutioninstance-api/) — An execution instance of a procedure step within a `ProcedureMethodExecutionInstance`. Created when a procedure run is started, representing a step where…
- [Benchling Project API](https://apis.io/apis/benchling/benchling-project-api/) — A top-level organizational container in Benchling that groups related work and controls access permissions. Projects contain Folders (see `Folder`) which in…
- [Benchling Protein API](https://apis.io/apis/benchling/benchling-protein-api/) — A Protein is a complex biomolecule entity in Benchling representing immunoglobulins or related therapeutic proteins like T-cell receptors. Proteins are…
- [Benchling Protein Format API](https://apis.io/apis/benchling/benchling-proteinformat-api/) — A ProteinFormat defines the structural template for a class of proteins, specifying the arrangement of chains and domains. Formats can be built-in (e.g.,…
- [Benchling Protein Schema API](https://apis.io/apis/benchling/benchling-proteinschema-api/) — Defines the structure, field definitions, and configuration options for Proteins.
- [Benchling Protein Version API](https://apis.io/apis/benchling/benchling-proteinversion-api/) — A historical snapshot of an `Protein` at a specific point in time, preserving the complete structural state including domains, chains, and HELM notation.…
- [Benchling Reaction API](https://apis.io/apis/benchling/benchling-reaction-api/) — A Chemical Reaction is a process where molecules are transformed into new molecules.
- [Benchling Request V2 Definition API](https://apis.io/apis/benchling/benchling-requestv2definition-api/) — A reusable template that defines the structure and configuration for requests in Benchling. Also known as a "Request Template" in the UI. Each…
- [Benchling Request V2 Submission API](https://apis.io/apis/benchling/benchling-requestv2submission-api/) — A workflow request submitted from a `RequestV2Definition` (known as "Request Template" in the UI). When a request is submitted (status transitions to SENT),…
- [Benchling Result API](https://apis.io/apis/benchling/benchling-result-api/) — A Result represents a single row of experimental measurement data in Benchling's lab automation system. Results conform to a ResultSchema that defines their…
- [Benchling Result Schema API](https://apis.io/apis/benchling/benchling-resultschema-api/) — Defines the structure and metadata fields for a category of assay Results in Benchling's lab automation system. A ResultSchema specifies the field…
- [Benchling Review API](https://apis.io/apis/benchling/benchling-review-api/) — Represents an active or completed review of a reviewable item such as an Entry or StageEntry. A Review tracks the overall status, the assigned reviewers…
- [Benchling Review Change API](https://apis.io/apis/benchling/benchling-reviewchange-api/) — Represents a single action taken within a review. ReviewChanges form an ordered history of all changes made to a review, including status transitions,…
- [Benchling Review Process API](https://apis.io/apis/benchling/benchling-reviewprocess-api/) — Defines a review process configuration that specifies how entries and other reviewable items should be reviewed. A ReviewProcess belongs to an Organization…
- [Benchling Review Process Stage API](https://apis.io/apis/benchling/benchling-reviewprocessstage-api/) — A single stage within a ReviewProcess that defines a required step in the review workflow. Each stage specifies what action reviewers must take (see…
- [Benchling Rna Oligo API](https://apis.io/apis/benchling/benchling-rnaoligo-api/) — Represents a short single-stranded RNA oligonucleotide in Benchling's molecular biology platform. RNA oligos are synthetic sequences used in applications…
- [Benchling Rna Oligo Schema API](https://apis.io/apis/benchling/benchling-rnaoligoschema-api/) — Defines the structure, field definitions, and configuration options for RNA oligos.
- [Benchling Rna Sequence API](https://apis.io/apis/benchling/benchling-rnasequence-api/) — Represents an RNA sequence in Benchling's molecular biology platform. An RnaSequence stores the nucleotide bases (using A, C, G, U) along with annotations…
- [Benchling Rna Sequence Schema API](https://apis.io/apis/benchling/benchling-rnasequenceschema-api/) — Defines the structure, field definitions, and configuration options for RNA sequences
- [Benchling Run API](https://apis.io/apis/benchling/benchling-run-api/) — A Run represents an execution instance of a lab automation workflow in Benchling, capturing the inputs, outputs, and metadata for a single assay or…
- [Benchling Run Schema API](https://apis.io/apis/benchling/benchling-runschema-api/) — Defines the structure and automation configuration for a category of Runs in Benchling's lab automation system. A RunSchema specifies field definitions for…
- [Benchling Scratch File API](https://apis.io/apis/benchling/benchling-scratchfile-api/) — A ScratchFile represents raw file content used as intermediate input or output of pipeline steps (see PipelineStepData). Unlike File, ScratchFiles are not…
- [Benchling Scratch Plate API](https://apis.io/apis/benchling/benchling-scratchplate-api/) — A plate design or record used for designing, tracking, and analyzing experimental plates outside of the inventory. Scratch plates are the working surface…
- [Benchling Search API](https://apis.io/apis/benchling/benchling-search-api/) — The Search API from Benchling — 1 operation(s) for search.
- [Benchling Service Principal API](https://apis.io/apis/benchling/benchling-serviceprincipal-api/) — Represents a non-human identity used for system integrations and automated processes within Benchling. Service principals act as the identity for service…
- [Benchling Sql Dashboard API](https://apis.io/apis/benchling/benchling-sqldashboard-api/) — A SqlDashboard is a configurable analytics page that displays one or more SQL-driven visualizations within Benchling Insights. Dashboards belong to a…
- [Benchling Sql Dashboard Block API](https://apis.io/apis/benchling/benchling-sqldashboardblock-api/) — Represents a single query and visualization pane within a SqlDashboard. Each block contains a SQL query (sqlQuery) that runs against the Benchling data…
- [Benchling Stage Entry API](https://apis.io/apis/benchling/benchling-stageentry-api/) — A StageEntry is an Entry that is associated with a specific stage in a legacy Workflow. Unlike regular Entries which exist independently in folders,…
- [Benchling Study API](https://apis.io/apis/benchling/benchling-study-api/) — A structured unit used to plan and organize research in Benchling. Each study progresses through phases (see `StudyPhase`) sequentially from design to…
- [Benchling Study Item Association API](https://apis.io/apis/benchling/benchling-studyitemassociation-api/) — Represents the link between a Study and a Studyable item (such as entities or molecules). Each association is identified by id and links a specific `study`…
- [Benchling Study Schema API](https://apis.io/apis/benchling/benchling-studyschema-api/) — A configuration template that defines the structure and behavior of Studies within an organization. Each `StudySchema` specifies the `studyType`, which…
- [Benchling Team API](https://apis.io/apis/benchling/benchling-team-api/) — Represents a subgroup of users within an `Organization`, enabling finer-grained user management and data sharing. Teams belong to exactly one organization,…
- [Benchling Template Collection API](https://apis.io/apis/benchling/benchling-templatecollection-api/) — A container that organizes related templates, subtemplates, and other template-like items. Template Collections provide a way to group and manage reusable…
- [Benchling Test Definition API](https://apis.io/apis/benchling/benchling-testdefinition-api/) — A Test Definition is a configuration object that specifies a type of test or assay that can be ordered against samples. Each Test Definition is associated…
- [Benchling Test Order API](https://apis.io/apis/benchling/benchling-testorder-api/) — A Test Order represents an individual request to perform a specific test on a sample. Each Test Order references a `TestDefinition` that specifies what type…
- [Benchling Unit API](https://apis.io/apis/benchling/benchling-unit-api/) — A Unit is a specific measure of a physical quantity within Benchling's tenant-specific unit dictionary, used to capture and convert scientific measurements…
- [Benchling Unit Type API](https://apis.io/apis/benchling/benchling-unittype-api/) — A UnitType is a dimensional category that groups inter-convertible `Unit` objects within Benchling's tenant-specific unit dictionary. Examples include…
- [Benchling User API](https://apis.io/apis/benchling/benchling-user-api/) — Represents a human user in Benchling who can log in, perform actions, and own data. Users belong to one or more Organizations and may be members of Teams…
- [Benchling Warehouse Credential API](https://apis.io/apis/benchling/benchling-warehousecredential-api/) — Represents credentials for connecting to Benchling's data warehouse, enabling users to query data using SQL tools like database clients or BI platforms.…
- [Benchling Warehouse Custom View API](https://apis.io/apis/benchling/benchling-warehousecustomview-api/) — A custom SQL view created by users in Benchling's data warehouse, allowing them to define reusable queries that can be accessed like tables. Views appear in…
- [Benchling Well Plate API](https://apis.io/apis/benchling/benchling-wellplate-api/) — A WellPlate is a multi-well plate in Benchling's inventory system where wells are permanently fixed to the plate structure. This is the standard plate type…
- [Benchling Well Plate Position API](https://apis.io/apis/benchling/benchling-wellplateposition-api/) — Represents a single well within a WellPlate, functioning as a fixed container at a specific grid position. Each WellPlatePosition has coordinates…
- [Benchling Well Plate Schema API](https://apis.io/apis/benchling/benchling-wellplateschema-api/) — Defines the structure and constraints for a category of WellPlates in Benchling's inventory system. A WellPlateSchema specifies the grid dimensions (height…
- [Benchling Workflow Output API](https://apis.io/apis/benchling/benchling-workflowoutput-api/) — Represents the result or product of completing a `WorkflowTask`. Each output is associated with a single task. Outputs can contain schema-defined fields…
- [Benchling Workflow Output Schema API](https://apis.io/apis/benchling/benchling-workflowoutputschema-api/) — Defines the structure of `WorkflowOutput` instances produced by tasks of a given `WorkflowTaskSchema`. Each output schema specifies `fieldDefinitions` for…
- [Benchling Workflow Task Group API](https://apis.io/apis/benchling/benchling-workflowtaskgroup-api/) — A container that groups related `WorkflowTask` instances together, representing a cohesive unit of work. Task groups are created from a `WorkflowTaskSchema`…
- [Benchling Workflow Task Schema API](https://apis.io/apis/benchling/benchling-workflowtaskschema-api/) — A configuration template that defines the structure and behavior of `WorkflowTask` instances. Each schema specifies an `executionType` (direct, entry, or…
- [Benchling Worklist API](https://apis.io/apis/benchling/benchling-worklist-api/) — A typed collection of items used to group related objects for batch operations. Unlike folders, items can belong to multiple worklists simultaneously,…
- [Benchling Worksheet API](https://apis.io/apis/benchling/benchling-worksheet-api/) — A structured document container used to organize and execute procedural work within Benchling's notebook system. Worksheets contain ordered…
- [Benchling App Installation API](https://apis.io/apis/benchling/benchling-app-installation-api/) — Represents an installed Benchling App on a tenant, created from an `AppDefinitionVersion`. App installations store tenant-specific configuration values and…
- [Benchling Audit Log API](https://apis.io/apis/benchling/benchling-audit-log-api/) — Represents a single entry in an object's audit log. Each entry captures what changed, who made the change, and contextual information about the affected…
- [Benchling Bulk Export API](https://apis.io/apis/benchling/benchling-bulk-export-api/) — The Bulk Export API from Benchling — 1 operation(s) for bulk export.
- [Benchling Pipeline Step API](https://apis.io/apis/benchling/benchling-pipeline-step-api/) — Represents a single operation node within a Pipeline's directed acyclic graph (DAG).
- [Benchling Workflow Task API](https://apis.io/apis/benchling/benchling-workflow-task-api/) — Represents a unit of work within a `WorkflowTaskGroup`.

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### AsyncAPI (1)

Event-driven and webhook contracts.

- [Benchling Webhooks](https://apis.io/asyncapis/benchling/benchling-webhooks/)

#### GraphQL (1)

GraphQL schemas.

- [Moved to /providers/benchling/](https://apis.io/graphqls/benchling/benchling-graphql/)

#### MCP servers (1)

Model Context Protocol servers that expose the API to agents.

- [benchling](https://apis.io/servers/benchling/benchling/)

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [Benchling Agentic Access](https://apis.io/agentic-access/benchling/benchling-agentic-access/)

#### JSON Schema (1035)

The data models the API reads and writes.

- [AIGGenerateInputAsyncTask](https://apis.io/schemas/benchling/AIGGenerateInputAsyncTask/)
- [AOPProcessOutputAsyncTask](https://apis.io/schemas/benchling/AOPProcessOutputAsyncTask/)
- [AaAnnotation](https://apis.io/schemas/benchling/AaAnnotation/)
- [AaSequence](https://apis.io/schemas/benchling/AaSequence/)
- [AaSequenceBaseRequest](https://apis.io/schemas/benchling/AaSequenceBaseRequest/)
- [AaSequenceBaseRequestForCreate](https://apis.io/schemas/benchling/AaSequenceBaseRequestForCreate/)
- [AaSequenceBulkCreate](https://apis.io/schemas/benchling/AaSequenceBulkCreate/)
- [AaSequenceBulkUpdate](https://apis.io/schemas/benchling/AaSequenceBulkUpdate/)
- [AaSequenceBulkUpsertRequest](https://apis.io/schemas/benchling/AaSequenceBulkUpsertRequest/)
- [AaSequenceCreate](https://apis.io/schemas/benchling/AaSequenceCreate/)
- [AaSequenceRequestRegistryFields](https://apis.io/schemas/benchling/AaSequenceRequestRegistryFields/)
- [AaSequenceSummary](https://apis.io/schemas/benchling/AaSequenceSummary/)
- [AaSequenceUpdate](https://apis.io/schemas/benchling/AaSequenceUpdate/)
- [AaSequenceUpsert](https://apis.io/schemas/benchling/AaSequenceUpsert/)
- [AaSequenceWithEntityType](https://apis.io/schemas/benchling/AaSequenceWithEntityType/)
- [AaSequencesArchivalChange](https://apis.io/schemas/benchling/AaSequencesArchivalChange/)
- [AaSequencesArchive](https://apis.io/schemas/benchling/AaSequencesArchive/)
- [AaSequencesBulkCreateRequest](https://apis.io/schemas/benchling/AaSequencesBulkCreateRequest/)
- [AaSequencesBulkGet](https://apis.io/schemas/benchling/AaSequencesBulkGet/)
- [AaSequencesBulkUpdateRequest](https://apis.io/schemas/benchling/AaSequencesBulkUpdateRequest/)
- [AaSequencesBulkUpsertRequest](https://apis.io/schemas/benchling/AaSequencesBulkUpsertRequest/)
- [AaSequencesFindMatchingRegion](https://apis.io/schemas/benchling/AaSequencesFindMatchingRegion/)
- [AaSequencesMatchBases](https://apis.io/schemas/benchling/AaSequencesMatchBases/)
- [AaSequencesPaginatedList](https://apis.io/schemas/benchling/AaSequencesPaginatedList/)
- [AaSequencesSearchBases](https://apis.io/schemas/benchling/AaSequencesSearchBases/)
- …and 1010 more published on APIs.io

#### JSON-LD (1)

Linked-data contexts for the provider's vocabulary.

- [Benchling Context](https://apis.io/jsonld/benchling/benchling-context/)

#### Examples (10)

Example requests and responses.

- [Createappconfigurationitem Request](https://apis.io/examples/benchling/createAppConfigurationItem-request/)
- [Createappconfigurationitem Response 201](https://apis.io/examples/benchling/createAppConfigurationItem-response-201/)
- [Createblob Request](https://apis.io/examples/benchling/createBlob-request/)
- [Createdataframe Response 200](https://apis.io/examples/benchling/createDataFrame-response-200/)
- [Createfile Response 200](https://apis.io/examples/benchling/createFile-response-200/)
- [Getappconfigurationitembyid Response 200](https://apis.io/examples/benchling/getAppConfigurationItemById-response-200/)
- [Getdataframe Response 200](https://apis.io/examples/benchling/getDataFrame-response-200/)
- [Gettask Response 200](https://apis.io/examples/benchling/getTask-response-200/)
- [Patchdataframe Response 202](https://apis.io/examples/benchling/patchDataFrame-response-202/)
- [Updateappconfigurationitem Request](https://apis.io/examples/benchling/updateAppConfigurationItem-request/)

#### Collections (57)

Postman and Open Collection request collections.

- [Benchling AA Sequences API](https://apis.io/collections/benchling/open-benchling-aa-sequences-api/)
- [Benchling AA Sequences Apps API](https://apis.io/collections/benchling/open-benchling-apps-api/)
- [Benchling AA Sequences Assay Results API](https://apis.io/collections/benchling/open-benchling-assay-results-api/)
- [Benchling AA Sequences Assay Runs API](https://apis.io/collections/benchling/open-benchling-assay-runs-api/)
- [Benchling AA Sequences Audit API](https://apis.io/collections/benchling/open-benchling-audit-api/)
- [Benchling AA Sequences Authentication API](https://apis.io/collections/benchling/open-benchling-authentication-api/)
- [Benchling AA Sequences Blobs API](https://apis.io/collections/benchling/open-benchling-blobs-api/)
- [Benchling AA Sequences Boxes API](https://apis.io/collections/benchling/open-benchling-boxes-api/)
- [Benchling AA Sequences Codon Usage Tables API](https://apis.io/collections/benchling/open-benchling-codon-usage-tables-api/)
- [Benchling AA Sequences Connect API](https://apis.io/collections/benchling/open-benchling-connect-api/)
- [Benchling AA Sequences Containers API](https://apis.io/collections/benchling/open-benchling-containers-api/)
- [Benchling AA Sequences Custom Entities API](https://apis.io/collections/benchling/open-benchling-custom-entities-api/)
- [Benchling AA Sequences Custom Notations API](https://apis.io/collections/benchling/open-benchling-custom-notations-api/)
- [Benchling AA Sequences Data Frames API](https://apis.io/collections/benchling/open-benchling-data-frames-api/)
- [Benchling AA Sequences Datasets API](https://apis.io/collections/benchling/open-benchling-datasets-api/)
- [Benchling AA Sequences DNA Alignments API](https://apis.io/collections/benchling/open-benchling-dna-alignments-api/)
- [Benchling AA Sequences DNA Oligos API](https://apis.io/collections/benchling/open-benchling-dna-oligos-api/)
- [Benchling AA Sequences DNA Sequences API](https://apis.io/collections/benchling/open-benchling-dna-sequences-api/)
- [Benchling AA Sequences Dropdowns API](https://apis.io/collections/benchling/open-benchling-dropdowns-api/)
- [Benchling AA Sequences Entities API](https://apis.io/collections/benchling/open-benchling-entities-api/)
- [Benchling AA Sequences Entries API](https://apis.io/collections/benchling/open-benchling-entries-api/)
- [Benchling AA Sequences Enzymes API](https://apis.io/collections/benchling/open-benchling-enzymes-api/)
- [Benchling AA Sequences Events API](https://apis.io/collections/benchling/open-benchling-events-api/)
- [Benchling AA Sequences Exports API](https://apis.io/collections/benchling/open-benchling-exports-api/)
- [Benchling AA Sequences Feature Libraries API](https://apis.io/collections/benchling/open-benchling-feature-libraries-api/)
- …and 32 more published on APIs.io

#### Overlays (1)

OpenAPI overlays, including conversational phrasing for each operation.

- [Benchling V3 Overlay](https://apis.io/overlays/benchling/benchling-v3-overlay/)

#### Governance rules (2)

Spectral rulesets for the provider's contracts.

- [Benchling — jsonschema rules](https://apis.io/rules/benchling/benchling-jsonschema-spectral-rules/)
- [Benchling API Rules](https://apis.io/rules/benchling/benchling-rules/)

#### Security (3)

Authentication, trust centre, and vulnerability disclosure.

- [Benchling Authentication](https://apis.io/security/benchling/benchling-authentication/)
- [Benchling Domain Security](https://apis.io/security/benchling/benchling-domain-security/)
- [Benchling Trust Center](https://apis.io/security/benchling/benchling-trust-center/)

#### OAuth scopes (1)

The permissions the API asks for.

- [Benchling Scopes](https://apis.io/scopes/benchling/benchling-scopes/)

#### Plans and pricing (1)

Published plans, tiers and prices.

- [Benchling Plans Pricing](https://apis.io/plans/benchling/benchling-plans-pricing/)

#### Rate limits (1)

Published request limits.

- [Benchling Rate Limits](https://apis.io/rate-limits/benchling/benchling-rate-limits/)

#### FinOps (1)

What the API costs to run, by operation.

- [Benchling Finops](https://apis.io/finops/benchling/benchling-finops/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://www.benchling.com/)
- [Documentation](https://docs.benchling.com/docs/developer-platform-overview)
- [Getting started](https://docs.benchling.com/docs/getting-started-benchling-apps)
- [API reference](https://benchling.com/api/reference)
- [Pricing](https://www.benchling.com/pricing)
- [Sign up](https://benchling.com/signup)
- [Support](https://help.benchling.com/hc/en-us/requests/new)
- [Changelog](https://docs.benchling.com/changelog)
- [Blog](https://www.benchling.com/insights)
- [Terms of service](https://www.benchling.com/agreements-and-terms)
- [Privacy policy](https://www.benchling.com/privacy)
- [GitHub](https://github.com/benchling)

## API Evangelist rating

**Kin Score 65.9** — strong · rubric 0.25.0 · scored 2026-10-23

| Facet | Score |
|---|---|
| Discoverability | 71.7 |
| Contract quality | 66.7 |
| Contract governance | 35.6 |
| Operational transparency | 69.7 |
| Developer ergonomics | 49.4 |
| Access clarity | 68.4 |

**Agent readiness 41.8** — agent-ready (gated down from agent-native)

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | derived (partial credit) |
| Reversibility Documented | — |
| MCP Server | templated |
| Auth Clarity | negotiable (partial credit) |
| Idempotency | — |
| Error Semantics | verified |
| OpenAPI Examples | partial |
| Rate Limit Signal | documented (partial credit) |
| Event Surface Described | yes |
| Agent Skills | derived (partial credit) |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |
| Pagination Ratio | partial |
| Operation Distinctiveness | mostly |

**Regulatory alignment 36.7** — Health

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/benchling/](https://apis.io/providers/benchling/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Benchling: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/benchling/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
