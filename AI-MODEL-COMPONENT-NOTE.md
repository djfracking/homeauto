<!-- AI-MODEL-COMPONENT-NOTE.md -->
<!-- Interpretive clarification for software incorporating AI model components. -->
<!-- Text: AI Model Component Note, v1.1-draft (June 2026), inno³ — CC0. -->
<!-- Preamble and Section 0 are verbatim from the published text. -->
<!-- Sections 1–3 are a faithful reconstruction from the published summary; -->
<!-- check the inno³ project repository for the canonical wording before final adoption. -->

## AI Model Component Note

*Interpretive clarification for software incorporating AI model components*

The following interpretive clarification applies to the work to which it is attached (the "**Program**") and is provided by the copyright holder(s) of the Program. This clarification supplements – and shall be read together with – the license under which the Program is distributed (the "**Applicable License**"). It does not add to or remove from the rights and obligations established by the Applicable License; rather, it makes explicit how certain existing obligations apply when the Program incorporates AI model components. To the extent that any provision of this clarification conflicts with the Applicable License, the Applicable License prevails.

### 0. Definitions

The "**Program**" means the work on which the Applicable License imposes the obligation to provide source code (or its preferred form for making modifications) – that is, the covered or licensed work as the Applicable License itself defines it. This clarification does not extend that obligation to any other work; it only makes explicit how the existing obligation applies to AI Model Components within that work.

An "**AI Model Component**" means any part of the Program whose behavior is determined, in whole or in part, by a machine learning model – including but not limited to trained parameters (weights, biases, embeddings), model configuration files, calibration data, quantization tables, or any other artifact whose modification is necessary to adapt, correct, or improve the behavior of that part of the Program. Whether an AI Model Component falls within this definition is determined by the role it plays in the Program's behavior, and not by the technical form of its packaging or by its conceptual independence from the surrounding code. For the avoidance of doubt, an AI Model Component is part of the Program; the fact that its behavior results from learned parameters rather than from explicitly programmed instructions does not, by itself, take that Component outside the scope of the Applicable License when it is distributed as part of the Program. Sections 2(a), 2(b) and 2(c) below identify the configurations in which a model is *not* considered part of the Program.

The "**Model Corresponding Information**" for an AI Model Component means the set of information, data, and instructions sufficient for a skilled person to understand, retrain, fine-tune, replace, and reintegrate that Component into the Program – that is, the preferred form of the AI Model Component for making modifications to it. This includes, without limitation:

(a) the specification of the model architecture (topology, layer configuration, activation functions, normalization schemes) sufficient for a skilled person to understand and modify the Component, in a documented, machine-readable format;

(b) the trained parameters (weights, biases) in a standard or well-documented format;

(c) the complete source code of the training, fine-tuning, and evaluation procedures used to produce the distributed parameters, including data preprocessing and augmentation pipelines;

(d) the training configuration (hyperparameters, optimization settings, random seeds where deterministic reproduction is feasible);

(e) a sufficiently detailed description of the training data – including its provenance, collection method, and processing steps – enabling a skilled person to assemble a functionally equivalent dataset; the training data itself, where it can be lawfully redistributed; or, where the training data is publicly available or obtainable from third parties, a listing of that data and of where to obtain it, including, where applicable, for a fee; and

(f) the instructions necessary to retrain, fine-tune, or replace the AI Model Component and to reintegrate the modified version into the Program, such that the Program can be built and run with the modified Component in the same manner as with the original.

The Model Corresponding Information is sufficient when it enables a skilled person to retrain, fine-tune, or replace the AI Model Component and to reintegrate it into the Program. As for the preferred form of a work for making modifications, the reference is the form actually used: the Model Corresponding Information comprises the elements of points (a) to (f) as the licensor or distributor itself uses or holds them in order to modify the Component. It does not require acquiring elements that have never been in the distributor's possession (Section 2 governs that case); it does require providing, without degradation, the forms actually used. The source code and the trained parameters of the Component, as distributed, are in all cases provided.

The Applicable License's own definition of Corresponding Source continues to govern what is excluded from it (such as System Libraries or general-purpose development tools); this clarification adds inclusions, and does not remove those exclusions. The software and any training dataset are distinct creations subject to distinct rights; this clarification does not extend the Applicable License to a dataset or other work that is not itself part of the licensed Program. Whatever the form in which the information is provided, it must remain possible for a skilled person to produce a functionally equivalent model.

### 1. Scope

This clarification applies to every AI Model Component distributed as part of the Program, and only to such Components. Where the Program, as distributed by or under the direction of a copyright holder, incorporates an AI Model Component without which the Program would not function as intended, that Component forms part of the Program, and the Model Corresponding Information for that Component forms part of the source code (or preferred form for making modifications) that the Applicable License obliges distributors to provide.

### 2. Configurations outside the scope

(a) **Mere aggregation.** A model distributed merely on the same medium as the Program, or stored alongside it, without the Program depending on that model to function as intended, is not an AI Model Component of the Program.

(b) **Independent services accessed through an interface.** A model operated by a third party and reached by the Program through a public or general-purpose interface (such as a public API) is not part of the Program, and the obligations of the Applicable License do not attach to it.

(c) **Third-party pre-trained models.** Where the Program incorporates a pre-trained model obtained from a third party, the distributor shall precisely identify that model, its provenance, and the applicable license, and shall document the integration, fine-tuning, calibration, or modification steps that the distributor itself performed. The distributor provides the Model Corresponding Information to the extent it holds or uses it; this clarification does not require the distributor to produce elements that were never in its possession, provided the missing elements and the reason they cannot be provided are precisely documented.

(d) **Lawful limits on redistribution.** Where an element of the Model Corresponding Information cannot be lawfully redistributed (for example personal data, or databases protected by a sui generis right), the distributor provides everything that can be provided and precisely documents what is missing and why. Transparency about the limits is the compliance standard; it does not exempt the distributor from providing the remaining elements.

### 3. Delivery standard

The Model Corresponding Information is provided by the same customary means, and subject to the same timing, as the source code required by the Applicable License. Where the Applicable License contains a no-further-restrictions clause (GPL-3.0 §10, AGPL-3.0 §10, GPL-2.0 §6, and equivalents), any contractual or technical barrier preventing recipients from using, studying, modifying, or redistributing the Model Corresponding Information is treated as a further restriction within the meaning of that clause.

---

*Text of the note: AI Model Component Note, v1.1-draft, © inno³, licensed CC0. Interpretive clarification in the tradition of the Linux kernel syscall note and the FSF GPL FAQ. To the extent of any conflict with the Applicable License, the Applicable License prevails.*
