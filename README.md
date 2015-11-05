# Limitation of Liability (Australia)

### Purpose

The limitation language in this repo is language for limitation of liability positions in **Australian** legal agreements.  The examples assume the use of the LawPatch clause <a href="https://github.com/lawpatch/lawpatch-docs" target="_blank">here</a>.

### Simple Limitations with LawPatch

Limitation of liability is a technical area.  If you want to draft an effective limitation, you end up with a lot of formulaic language.  LawPatch allows you to factor the technical language out.  Here's an example of a full limitation of liability using LawPatch:

> Provider <a href="https://github.com/lawpatch/au-limitation/blob/90bb197e3299a4025af8c3db50e33b3f291e66a2/au-limitation-0.md" target="_blank">limits liability as much as the law allows</a> to Customer for the Services, including liabilities caused by:
- data loss;
- software bugs, viruses and vulnerabilities; and
- accessibility of any software or data.

Simple.

### Spectrum of Positions

There are a number of liability positions available in this repo:

- `au-limitation-0.md` limits liability to the fullest extent possible under the law;
- `au-limitation-1.md` limits liability to the amount described;
- `au-limitation-2.md` limits consequential loss liabilities only; and
- `au-limitation-3.md` does not limit liability at all (except liabilities arising from implied conditions).

### Position Parameters

The language in this repo is *not* language that you can import wholesale with a simple incorporation by reference - it assumes that you have included certain information in the clause that imports it (the `Exception` parameter is optional).

**au-limitation-0: Full liability limitation**

Position parameters are:

- `Limiting Party` - The party relying on the limitation;
- `Subject` - What the Limiting Party is limiting liability in relation to (subject of limitation);
- `Risks` - A description of specific risks that liability is limited in relation to; and
- `Exception` (optional) - An exception to the limitation of liability.

Here is an example of language importing the full limitation of liability.

> Provider <a href="https://github.com/lawpatch/au-limitation/blob/90bb197e3299a4025af8c3db50e33b3f291e66a2/au-limitation-0.md" target="_blank">limits liability as much as the law allows</a> to Customer for the Services, including liabilities caused by:
- data loss;
- software security vulnerabilities; and
- accessibility of any software or data.

**au-limitation-1: Amount limitation**

Position parameters are:

- `Amount` - Means the amount that the limitation limits liability to;
- `Limiting Party` - The party relying on the limitation;
- `Subject` - What the Limiting Party is limiting liability in relation to (subject of limitation);
- `Risks` - A description of specific risks that liability is limited in relation to; and
- `Exception` (optional) - An exception to the limitation of liability.

Here is an example of language importing the limitation to amount.

> Provider limits liability to Customer for the Services to the cost of the Services in accordance with the <a href="https://github.com/lawpatch/au-limitation/blob/90bb197e3299a4025af8c3db50e33b3f291e66a2/au-limitation-1.md" target="_blank">LawPatch amount limitation</a>, including liabilities caused by:
- data loss;
- software bugs, viruses and vulnerabilities; and
- accessibility of any software or data.

**au-limitation-2: Covering liability (except limiting consequential loss)**

Position parameters are:

- `Limiting Party` - The party relying on the limitation;
- `Subject` - What the Limiting Party is limiting and assuming liability in relation to (subject of limitation);
- `Risks` - A description of specific risks that liability is limited in relation to; and
- `Exception` (optional) - An exception to the limitation of liability.

Here is an example of language importing the limitation of consequential loss.

> Provider <a href="https://github.com/lawpatch/au-limitation/blob/90bb197e3299a4025af8c3db50e33b3f291e66a2/au-limitation-2.md" target="_blank">covers liabilities (except for consequential loss)</a> to Customer for the Services, including liabilities caused by:
- data loss;
- software bugs, viruses and vulnerabilities; and
- accessibility of any software or data.

**au-limitation-3: Covering all liability**

Position parameters are:

- `Subject` - What the Limiting Party is assuming liability in relation to (subject of limitation); and
- `Exception` (optional) - An exception to the limitation of liability.

Here is an example of language calling a module to cover all losses.

> Provider <a href="https://github.com/lawpatch/au-limitation/blob/90bb197e3299a4025af8c3db50e33b3f291e66a2/au-limitation-3.md" target="_blank">covers all liabilities incurred</a> by Customer for the Services.

### Using Multiple Positions

The parties will often have different liability positions in respect of each other.  Here's an example.

> - Provider <a href="https://github.com/lawpatch/au-limitation/blob/90bb197e3299a4025af8c3db50e33b3f291e66a2/au-limitation-0.md" target="_blank">limits liability as much as the law allows</a> to Customer for the Services, including liabilities caused by:
    - data loss;
    - software bugs, viruses and vulnerabilities; and
    - accessibility of any software or data.
- Customer <a href="https://github.com/lawpatch/au-limitation/blob/90bb197e3299a4025af8c3db50e33b3f291e66a2/au-limitation-2.md" target="_blank">covers liability except for consequential loss</a> to Customer for breaches of the Agreement.

There is an optional exception parameter for each position listed above. Here's how it might look if you use it.  In this example, the Provider fully limits liability for services but makes an exception for maintenance work, where there is no limitation.

> Provider <a href="https://github.com/lawpatch/au-limitation/blob/90bb197e3299a4025af8c3db50e33b3f291e66a2/au-limitation-0.md" target="_blank">limits liability as much as the law allows</a> to Customer for the Services, including liabilities caused by:
- data loss;
- software bugs, viruses and vulnerabilities; and
- accessibility of any software or data,

> except for Maintenance where Provider <a href="https://github.com/lawpatch/au-limitation/blob/90bb197e3299a4025af8c3db50e33b3f291e66a2/au-limitation-3.md" target="_blank">covers all liability</a> of Customer.

### Not Legal Advice

This is not legal advice.  Lawyers are involved in producing these terms, but they obviously aren't familiar with your circumstances.  Speak to your lawyer to make sure that the limitation language is well aligned with your circumstances.

### Licence

The limitation language is released under the license in license.md.


