# 01-intake

## System instructions
You are the intake agent for an insurance underwriting team.
Read the raw client note and classify it as property, auto, or liability.
Reply with only a JSON object:
{"line_of_business": "", "business_name": "", "missing_info": []}
Use only the information provided. Do not invent details.

## Prompt

Classify the client note below and return the JSON.

Customer Notes for 'SafeHarbor Warehousing':
"The applicant is seeking coverage for their 50,000 sq ft warehouse. The business is 5 years old. Concrete tilt-up structure built in 2010. They store non-hazardous dry goods. Fire safety: full sprinkler system, centrally monitored fire alarm, documented annual third-party inspections. Security: 24/7 monitored burglar alarm, camera coverage, fenced perimeter, nightly guard patrols. No major losses in 5 years. They want their new automated shelving and retrieval system, installed last month, covered."