# Milk Recommendation System
### A student-built nutrition comparison and preference-matching prototype

This project explores how nutrition information can become easier to compare and use. It began with a question about school milk products and developed into a browser-based prototype combining nutrition interests with software development.

**Current status:** working prototype code with an 11-product local dataset, rule-based rankings, and barcode lookup integration. Product data, scoring rules, and external-data handling still require validation. This is not a clinically validated dietary recommendation system.

## Why we built it

Our initial question was: **Which milk should we choose, and why?**

Simply collecting nutrition facts was not enough: those facts already appear on packaging. During team discussions, Zion challenged the usefulness of an information-only website. That feedback shifted the project toward preference-based comparison. A teacher's suggestion to make product recognition more interactive helped motivate the scanning feature.

The project now asks a more focused design question:

**How can we help students compare milk products against their stated preferences while understanding the evidence and limitations behind each result?**

## What is implemented

The following describes code in `index.html`, reviewed on October 14, 2026. Code presence does not establish successful operation on every device.

| Component | Current implementation |
| --- | --- |
| Local product catalog | 11 hard-coded milk entries with nutrition values, lactose-free flags, and prices |
| Preference controls | Lactose-free, protein, sugar, fat, calories, calcium, and price importance |
| Ranking | Hand-written weighted scoring, a top-three display, and full rankings |
| Product details | Nutrient values, preference-related warnings, and comparisons with local entries |
| Barcode input | Camera scanning through html5-qrcode and manual barcode entry |
| External lookup | Open Food Facts product API integration |
| Actual-intake calculator | Not implemented |
| Nutrition-label OCR | Not implemented |
| Machine learning | Not implemented; current scoring is rule-based |
| Validated unit normalization | Not yet implemented consistently across external data |

## How the prototype works

1. A user selects preferences and price importance.
2. The application applies fixed rules and weights to local products.
3. It displays ranked products and individual nutrient information.
4. Alternatively, a barcode lookup retrieves an external product and compares its score with local entries.

The displayed percentage is a normalized **preference score**. It is not a probability of health benefit, a medical suitability estimate, or a validated measure of nutritional quality. The weights and cutoffs are prototype design choices, not established clinical thresholds.

## What the code review revealed

These issues are open engineering and scientific limitations, not completed fixes:

- **Inconsistent measurement bases:** the external lookup reads fields named `*_100g`. Energy can fall back to a per-serving field without conversion. Therefore, the earlier claim that all values are standardized per 100 mL was too strong. Mass, volume, and serving bases must be recorded and reconciled before comparison.
- **Missing values become zero:** absent nutrient fields and external prices are currently assigned zero. Missing price can then earn favorable price points; missing sugar or fat can also appear favorable.
- **Lactose-free status is incomplete:** external products default to `false`, which cannot distinguish an unknown status from a confirmed non-lactose-free product.
- **A requirement is treated as a preference:** selecting lactose-free adds a scoring weight rather than excluding products that fail the requirement.
- **Data provenance is missing:** local entries do not record label photographs, source dates, or verification history. The interface labels prices as per 500 mL, but the underlying source and conversion are not documented.
- **Nutrient naming needs verification:** the internal field `fat` is displayed as saturated fat and populated from an external saturated-fat field. Local values need label verification before their meaning can be confirmed.
- **External product scope is unchecked:** the lookup does not explicitly restrict results to milk products.
- **Validation remains outstanding:** this README does not report measured improvements in nutrition understanding, real-world adoption, or health outcomes.

## Biology and health-literacy contribution

The biological component should be demonstrated through accurate concepts and evidence-based design decisions:

- Distinguish total sugars from added sugars. Naturally occurring milk sugar contributes to total sugars.
- Explain lactose digestion and distinguish lactose intolerance from milk-protein allergy.
- Do not describe lactose-free dairy as safe for someone with milk allergy.
- Distinguish total fat from saturated fat and document measurement units.
- Explain tradeoffs between nutrients, serving volume, cost, and user preferences without declaring one product universally healthiest.

These concepts should guide the interface and dataset. They should not be used to imply that the app diagnoses conditions or prescribes diets.

## Proposed next phase: a school nutrition-literacy pilot

**Proposed research question:** Does a verified comparison tool help students answer milk-label questions more accurately than viewing labels alone?

This is a proposed study, not a completed result.

### Phase 1 — Establish trustworthy inputs

- Audit the existing 11 products against current packaging or manufacturer information.
- Record source, verification date, serving volume, nutrient units, package size, and price basis.
- Preserve unknown values explicitly.
- Implement documented per-100-mL comparisons only where the source supports a volume conversion.
- Separate verified requirements from optional scoring preferences.
- Publish the scoring rules and explain each recommendation.

### Phase 2 — Add one useful feature

Build an actual-intake calculator from verified volume-based data:

`nutrient consumed = nutrient per 100 mL × volume consumed in mL / 100`

Show both the common comparison basis and the user's chosen volume. Add short explanations of the concepts above.

### Phase 3 — Test understanding and usability

Start with a small, voluntary school pilot after agreeing on an appropriate process with a supervising teacher.

- Use matched label-reading tasks: nutrient comparison, serving-size calculation, and identifying whether information is unknown.
- Compare labels alone with the tool using randomized groups or counterbalanced task order.
- Use equivalent task sets to reduce practice effects.
- Define answer keys and the primary outcome before collecting data.
- Measure accuracy, completion time, and observed misunderstandings; record satisfaction separately.
- Report participant count separately from the number of task responses.
- Avoid collecting unnecessary health information; this pilot does not require milk consumption or symptom testing.
- Report small-sample and single-school limitations. Improved task performance would not establish improved health.

### Phase 4 — Evaluate practical use

If the pilot supports usefulness, test an accessible school QR-code entry point and a maintainable verified catalog. Measure voluntary reuse, failed lookups, and the effort required to keep data current before expanding to more products.

OCR, international catalogs, and machine learning are longer-term possibilities. They should follow evidence of user need and reliable data handling.

## Collaboration and ownership

The project originated from the student project initiator's milk-comparison idea and developed through collaboration with Zion, who is interested in computer science. Team discussion and teacher feedback shaped the direction.

Detailed individual implementation, research, testing, and AI-assisted contributions should be documented from actual work records. This README does not infer authorship of specific code components.

## Running the prototype

The interface is contained in `index.html` and uses HTML, CSS, and JavaScript. Serve it through a static web server. Camera access generally requires an appropriate secure browser context and permission. External fonts, the scanner library, and product lookups require network access.

## Evidence to collect as the project develops

- A source-backed product dataset and a reproducible data audit
- A documented scoring specification and worked examples
- A pilot protocol and anonymized aggregate findings
- A development log linking feedback to changes
- Clear individual contributions and accurate implementation status

## References

- [FDA: Added Sugars on the Nutrition Facts Label](https://www.fda.gov/food/nutrition-facts-label/added-sugars-nutrition-facts-label)
- [NIDDK: Definition and Facts for Lactose Intolerance](https://www.niddk.nih.gov/health-information/digestive-diseases/lactose-intolerance/definition-facts)
- [Open Food Facts](https://world.openfoodfacts.org/)

The project's next milestone is a trustworthy, explainable tool with measured educational usefulness.
