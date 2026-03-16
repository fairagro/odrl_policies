# FAIRagro ODRL Policies

This repository contains the **legal policy templates** used within the FAIRagro infrastructure to represent **licensing, access conditions, and regulatory obligations** for agrosystems datasets.

The policies are expressed using the **Open Digital Rights Language (ODRL)** in **JSON-LD format** and are intended to be referenced from dataset metadata via **schema.org**.

The repository supports the implementation of the **FAIRagro Legal Metadata Standards** and accompanies the FAIRagro deliverables on legal metadata.

---

# Background

Research data infrastructures (RDIs) participating in FAIRagro provide datasets with varying legal conditions, including:

- different licensing models
- access restrictions
- authentication requirements
- regulatory obligations

To enable **machine-readable representation of these legal conditions**, FAIRagro uses the **ODRL standard**.

Legal policies are referenced from dataset metadata using the **schema.org property `usageInfo`**, typically pointing to a persistent identifier (URL or DOI) representing the policy.

Example:

```json
{
  "@context": "https://schema.org/",
  "@type": "Dataset",
  "name": "Example Dataset",
  "usageInfo": "https://example.org/policies/open-access"
}
