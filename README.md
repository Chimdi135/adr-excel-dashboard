# adr-excel-dashboard
Practice project on 50,000 synthetic adverse drug reaction reports across 20 drugs. The data is synthetic, so findings do not apply to real drugs.

Questions: Which drugs get the most reports? How does severity change with age? How common are concomitant drugs?

Cleaning: removed “mg” from Dosage; added a yes/no concomitant-drug column; checked ReportID for duplicates (none); grouped Seriousness into Severe/fatal versus Not severe; grouped age into 10-year bands.

Findings: reports are spread evenly across drugs (2,382 to 2,591 each); 5.03% of reports are severe or fatal; severe or fatal share is about 4.6% to 5.2% in most age bands (6.23% in 80-90, from only about 1,140 reports); 56% of reports list other drugs.

Limits: synthetic data; a report doesn’t prove causation; ADR codes aren’t decoded; no statistical tests run.

Tools: Excel (PivotTables, slicers, calculated columns, charts)
