Pegged TODO:
============

Short term:

TODO: bug on parameterized rules
TODO: Calculating column/line position on failures (or, more generically, on a Parse Tree)
TODO: 'hooked' rules: rules that can be extended at runtime, or modified. I want to have a D parser that accepts syntactic extensions. I have these hooked rules, they work, but the end-user code is not as polished as I'd like.
TODO: add an enum inside ParseTree's, containing the rules's name, to enable final switch selection
TODO: option infrastructure (easier for the user: grammar!(memoizing, inlining, debug))
TODO: Add a debug mode that logs everything a parser does: which rule was tested by sequences and choices, which was unsuccessful, and so on.
TODO: introspection: unit rules (A <- B), generating rules (terminals are generating, sequences are if all subrules are generating), non reachable rules, useless rules (non-reachable or non generating)

Long term:

TODO: Make it possible for rules to be both non-parameterized and parameterized (ie A <- ... and A(B) <- ... in the same grammar) ?
TODO: parsing a range.
TODO: a function that reconstitutes D code from a parse tree.
TODO: tree functions (at least filtering, reducing and matching on trees).
TODO: parsing context and undoing any change done by a failed rule.
TODO: code lowerings.
TODO: Better error report: explaining what was expected "rule Digit failed at XXX, expected '0'-'9'"
TODO: Add a boolean grammar (&&, ||, !) and a comparison grammar( ==, !=, <, >, <=, >=), calling arithmeric expressions.
TODO: import expressions in grammars?
TODO: rules parameterized on numbers
TODO: external rules, introduced by < name > or automatically recognized.
TODO: direct D code, with {{ }} ? Or use < > for actions and { } for D code
TODO: [ ] after rule names and grammars, for options.
TODO: memoization as a parse-time option and not a generation-time option
TODO: adding [ ] after a grammar name for importing other grammars.
TODO: another option for grammars, coupled to external rules: creating inner variables.
TODO: drop the static methods and try standard methods?
