# Eval Case: CV PDF + JD PDF + Company URL

## User Prompt

I uploaded my current CV as a PDF and the JD as another PDF. Company website: https://example-ai-startup.com. Help me make a CV for this application.

## Expected Behavior

- Acknowledges PDF inputs and extracts/uses available content if tool context provides it.
- If PDF content is not accessible, asks user to paste text or provide extracted content.
- Reviews company website/context before recommending direction, if browsing is available.
- Offers CV strategy options based on company/JD: likely ATS-first plus AI/product/startup narrative alternatives.
- Does not fabricate company details if website cannot be read.

## Failure Modes

- Pretends to read inaccessible PDFs.
- Pretends to know company details without fetching/reading.
- Drafts final CV without strategy options.
