# The Ontological Prism

“The checker verifies a total before the reporter publishes it.”

Suppose record R17 contains the numbers 7 and 5. The calculator produces 12, and the checker confirms the addition. The reporter then publishes 12 under the heading R18.

The calculation is correct. The report attaches it to a different record. Asking the model to “check the answer more carefully” may simply produce another demonstration that 7 + 5 = 12. A useful inquiry has to recover what the answer is an answer *about*.

The **Ontological Prism** brings attention to the kinds of things, distinctions and relationships involved in a situation. The same case can then be examined through relevant knowledge domains. The subject remains available while the inquiry changes its view.

## 1. What is being checked?

Our opening sentence contains several things that can be confused: a checker, a numerical value, a record, and a report. It also contains relationships. The value was calculated from R17; the checker verified that calculation; the report presents the value as belonging to R18.

The bare number 12 does not preserve these relationships. It can be copied faithfully while its meaning in the report changes. Similarly, the word “verified” can travel with the value after the connection to the verified record has been lost.

An ontological account makes the objects and their relationships explicit enough to distinguish those cases. For this application, “verified result” needs to identify both the result and the record whose calculation was checked. Otherwise, the reporter may receive a true value with an ambiguous claim attached to it.

The contributing moves are *decomposition* and *relation extraction*: separate the compact sentence into its participants and recover how they are connected. *Comparison* then shows the mismatch between the record checked and the record named in the report. Their combination locates a failure that a second arithmetic check would leave untouched.

## 2. From a particular record to an identity class

R17 is a particular record. The example specifies its values and its use in the checking workflow, but not what the quantities represent. More usefully for the attribution problem, we can describe a class of results whose verification remains attached to their source records.

This movement is *abstraction*. The names R17 and R18 can be set aside while retaining the relationship that makes the case significant:

> A result checked for one record is presented as a result checked for another.

An **identity class** specifies what an instance must retain to count as the kind of thing under discussion. Here, numerical equality alone is insufficient for two reported results to be interchangeable. Their source records matter too. In another task—collecting examples of sums that equal 12—the record identity might be irrelevant. The application determines which distinctions must survive.

*Concretization* brings the class back to R17: which supplied record, value and checking statement instantiate it? *Comparison* checks whether the generalized description still explains the actual error. Together, abstraction and return make the account reusable without discarding its reason for being useful.

The same care applies to the participants. “Checker” describes a role. It does not by itself tell us which program occupies that role, what information the program receives, or whether it may authorize publication. Those questions remain available for later analysis.

## 3. Looking through relevant domains

Once the subject is clear, different domains can expose different aspects of it. **CDP**, the framework's bounded domain-selection method, asks which lenses can materially change this inquiry.

The attribution problem is specified, but the application behind the numbers is not. If R17 belongs to a spreadsheet, does the mathematically correct total make sense in that larger context? What ontology dimensions should be considered? At first glance, the AI might settle on a balance of accounts or some other accounting exercise. Could that framing overlook physics and harmonics, economics and business, music and measures, or religion and theology? For example, a symbolic reading of 7 + 5 = 12 could associate covenant completion (7) and divine grace (5) with perfect organizational structure and governance (12). Such a reading concerns what the numbers represent; it does not change the arithmetic equality.

The prism keeps plausible interpretations available while further context guides a bounded selection of useful lenses. It can retain possibilities without developing every one, and further context may narrow the inquiry without settling it completely.

Returning to the stated R17/R18 error, the mathematical view checks the addition. The information view examines how the value represents its source record. Both concern the same result, but they answer different questions:

| Lens | Question in this case | What it contributes |
|---|---|---|
| Mathematics | Does 7 + 5 equal 12? | The stated calculation is correct. |
| Information | Does the report preserve which record was checked? | R17 becomes R18, changing the claim. |

Changing view is a *rotation of attention*. The facts stay fixed while another relationship becomes prominent. *Salience reweighting* gives the record mismatch priority once the arithmetic has been settled. Repeating the settled calculation then has little value compared with tracing the record reference.

Suppose the application adds one condition: the checker may confirm arithmetic, while permission to publish must come from a separate approval. An ethical lens concerning permission now changes the analysis. A report can preserve R17 and its correct total while still lacking the required permission. Without that condition, introducing a discussion of publication authority may add an assumption rather than solve the stated problem.

CDP provides 19 broad domain axes, including `math`, `info` and `eth`. These are possible places to look. The label `info` does not identify R17, define a verified result, or establish its provenance. Likewise, assigning `eth` does not grant anyone authority. An identity class describes what we are considering; a domain lens selects knowledge through which to examine it.

The combination adds breadth with a purpose. *Rotation* opens another view; *comparison* identifies what that view contributes; *evaluation* retains it when it exposes a missing variable, changes a candidate arrangement, or supplies a useful challenge.

## 4. Keeping the prism bounded

“Use every perspective” can make a small problem harder to see. Music, biology and geography need no place in the R17 analysis unless some supplied feature makes them consequential. The number of named domains is a poor substitute for progress.

CDP therefore prefers a small set of useful lenses. It can retain a possible lens for reconsideration without developing it immediately. If the value and source record are now preserved but publication still fails, the unresolved discrepancy can justify reopening the domain selection.

The initial account may itself be uncertain. “The report is wrong” could concern arithmetic, record identity or permission. **KCE** helps produce provisional structural descriptions while preserving those alternatives. CDP can examine the material candidates separately, rather than making the first clean description govern every later view.

There is also a vocabulary trap. “Correct” may mean numerically correct, attached to the correct record, or permitted for publication. Keeping those meanings distinct prevents agreement on a word from concealing disagreement about the claim. This combines *label decomposition*, *comparison* and *concretization*: each sense is returned to the actual check it requires.

The package distributes this work between KCE's provisional extraction and CDP's domain selection; it does not supply a separate module named Ontological Prism. CDP's profiles, weights and scores organize the requested inquiry. They are design controls, not measurements of the model's neural attention.

A capable model may perform much of this work natively when prompted. Its useful contribution is the explicit distinction it returns: what was checked, what the report claims, and which further fact matters. The analysis alone cannot establish what a running program actually received or published.

## 5. A bounded request to the model

The following request invites the combined method while keeping the example small:

> Record R17 contains 7 and 5. The calculator produces 12, and the checker verifies that addition. The reporter publishes 12 under R18. Identify the things and relationships needed to explain the error. Abstract one reusable description, then show how it applies to these facts. Use mathematical and information lenses only where each changes the analysis. Explain what the arithmetic check establishes, what it leaves unresolved, and what information a corrected report must preserve. Do not assume publication rules that have not been supplied.

**References:** [CDP reader guide](04_ONTOLOGICAL_PRISM.md) · [CDP v1.2 specification](../../framework/CDP_Parallax_v1.2_BoundedDomainSpace.json) · [KCE v2.3 specification](../../framework/KCE_Parallax_v2.3_SplitLayerAnchor.json) · [O/D/R/O guide](../appendices/REFERENCE.md#represent-the-case)

[Previous: Sentence-thought vectors](03_SENTENCE_THOUGHT_VECTORS.md) · [Next: The Dynamical Prism](05_DYNAMICAL_PRISM.md)
