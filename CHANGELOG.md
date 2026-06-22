# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [2.0.0](https://github.com/fraefel/templify/compare/v1.6.1...v2.0.0) (2026-04-02)


### ⚠ BREAKING CHANGES

* UpdateFieldsOnOpen changed from bool to enum.
* The else marker syntax has changed from {{else}} to {{#else}} to be consistent with other control flow markers ({{#if}}, {{#elseif}}, {{#foreach}}).

### Features

* add .editorconfig for consistent code style ([6b33421](https://github.com/fraefel/templify/commit/6b3342147a3ed9035cb8845ac45693dea2e98b2d)), closes [#10](https://github.com/fraefel/templify/issues/10)
* add .NET 10 support ([#52](https://github.com/fraefel/templify/issues/52)) ([fcd29c4](https://github.com/fraefel/templify/commit/fcd29c488e1f87f0f162f4d5345d7b669a96849d))
* add automated documentation example generator ([eb705cd](https://github.com/fraefel/templify/commit/eb705cdfe08b0cd81bc9c4134b9cf0523bb12002))
* add custom Templify icon and branding ([#76](https://github.com/fraefel/templify/issues/76)) ([ff50e39](https://github.com/fraefel/templify/commit/ff50e39a5c448dd2d6112a9c207adf5e5fbd8fc6))
* add DocumentProperties option for setting document metadata ([#78](https://github.com/fraefel/templify/issues/78)) ([a31038b](https://github.com/fraefel/templify/commit/a31038b55f45c2f997c9abf968d6480212625aec))
* add elseif support for multi-branch conditionals ([#56](https://github.com/fraefel/templify/issues/56)) ([b451e0d](https://github.com/fraefel/templify/commit/b451e0d4d8a4d3c9bf09caa1de3445760a8ddb37))
* add named iteration variable syntax for nested loops ([#63](https://github.com/fraefel/templify/issues/63)) ([b0839af](https://github.com/fraefel/templify/commit/b0839af5debc9445f37a016a7632cb090bd03872))
* add processing warnings with report generation ([#70](https://github.com/fraefel/templify/issues/70)) ([859ec79](https://github.com/fraefel/templify/commit/859ec7966406a5b1ba64adb9a8fb1a281a19d649))
* Add public IConditionContext interface for batch condition evaluations ([#30](https://github.com/fraefel/templify/issues/30)) ([7e31537](https://github.com/fraefel/templify/commit/7e31537ed5bb4aad7969e1511534b67626cf9445))
* Add public IConditionEvaluator interface for standalone condition evaluation ([#29](https://github.com/fraefel/templify/issues/29)) ([951a027](https://github.com/fraefel/templify/commit/951a02731c749e09e519ca98c17baebff5164fa1))
* Add SonarQube integration workflow ([#34](https://github.com/fraefel/templify/issues/34)) ([d4bdc1c](https://github.com/fraefel/templify/commit/d4bdc1c687726853bc3715eda0fbfcadf3fbc6c3))
* add support for headers and footers ([#81](https://github.com/fraefel/templify/issues/81)) ([5b37abe](https://github.com/fraefel/templify/commit/5b37abe3c37f1b23f22a3157d98c125a8409e305))
* add support for inline conditionals ([#44](https://github.com/fraefel/templify/issues/44)) ([0cf0b27](https://github.com/fraefel/templify/commit/0cf0b27ecb7d8960b7c9c3752d3bf130bba3ff0c))
* add text replacement lookup table for HTML entities ([#65](https://github.com/fraefel/templify/issues/65)) ([1378e5c](https://github.com/fraefel/templify/commit/1378e5c5be1d40f295dc185e1b080dee8c4f0b13))
* Add TextTemplateProcessor for email and text templating ([#38](https://github.com/fraefel/templify/issues/38)) ([08b496c](https://github.com/fraefel/templify/commit/08b496cbb61b49cf8987728f32e65015c8d77cab))
* add UpdateFieldsOnOpen option for TOC refresh ([#68](https://github.com/fraefel/templify/issues/68)) ([8bd178e](https://github.com/fraefel/templify/commit/8bd178e46671f4b47604f07236a77b0db0bee81c))
* change {{else}} to {{#else}} for syntax consistency ([#62](https://github.com/fraefel/templify/issues/62)) ([830963c](https://github.com/fraefel/templify/commit/830963ce34462a92ef77318efa11f52d9d4d2918))
* implement non-boolean format specifiers ([#22](https://github.com/fraefel/templify/issues/22)) ([#82](https://github.com/fraefel/templify/issues/82)) ([a4a633c](https://github.com/fraefel/templify/commit/a4a633c53a539159cbac83503d9e1e7a7868a297))
* preserve highlight and shading formatting in per-run placeholder replacement ([#54](https://github.com/fraefel/templify/issues/54)) ([2b633d5](https://github.com/fraefel/templify/commit/2b633d5883caf97c35f2a907d39af8897cf3a7b6))
* support newline characters in variable values ([#57](https://github.com/fraefel/templify/issues/57)) ([08a146e](https://github.com/fraefel/templify/commit/08a146e6f9caa4db5d492f4793e196aeeb6fa68b))
* support typographic/curly quotes in conditional expressions ([#50](https://github.com/fraefel/templify/issues/50)) ([1fd83ae](https://github.com/fraefel/templify/commit/1fd83ae9c77b6935545c1db4a3a8f61861c98cad))
* unify equality operators and add condition validation ([#84](https://github.com/fraefel/templify/issues/84)) ([13883fc](https://github.com/fraefel/templify/commit/13883fce628244750ab0b2aaa5977f1462766f1d))


### Bug Fixes

* case-insensitive boolean comparison in ConditionalEvaluator ([#73](https://github.com/fraefel/templify/issues/73)) ([af35c50](https://github.com/fraefel/templify/commit/af35c504eba135aaacaed0b55a3599c2b1521d2b))
* evaluate conditionals inside loops with correct context ([#59](https://github.com/fraefel/templify/issues/59)) ([#60](https://github.com/fraefel/templify/issues/60)) ([55bec89](https://github.com/fraefel/templify/commit/55bec897376d5844f74257a168eef476b63206a3))
* prevent nested paragraphs in RepeatingConverter ([#42](https://github.com/fraefel/templify/issues/42)) ([91e6aa6](https://github.com/fraefel/templify/commit/91e6aa64cab754539543334662140349423fdc91)), closes [#41](https://github.com/fraefel/templify/issues/41)
* resolve all nullable reference and unused field warnings ([85c62f1](https://github.com/fraefel/templify/commit/85c62f1d76b06054c047beca6c6d550fdd1d36f5))
* sanitize invalid XML characters in template values ([#87](https://github.com/fraefel/templify/issues/87)) ([71a1fa6](https://github.com/fraefel/templify/commit/71a1fa689c24bf27c86b24a096332c7f720a2b78))
* treat null values as valid in template validation ([#48](https://github.com/fraefel/templify/issues/48)) ([02ed1a0](https://github.com/fraefel/templify/commit/02ed1a09402539ed0f1a4e6a6f413196daacb93e))
* Use SONAR_HOST_URL from secrets instead of variables ([#36](https://github.com/fraefel/templify/issues/36)) ([d18d895](https://github.com/fraefel/templify/commit/d18d8951aa0ccc0b2dde150ce4ed39f1f33c2742))
* validate loop-scoped variables correctly in template validation ([#61](https://github.com/fraefel/templify/issues/61)) ([e7be292](https://github.com/fraefel/templify/commit/e7be292f3f6873b3ff7d4097b3343f30ba1e1e1a))

## [1.6.1](https://github.com/TriasDev/templify/compare/v1.6.0...v1.6.1) (2026-04-01)


### Bug Fixes

* sanitize invalid XML characters in template values ([#87](https://github.com/TriasDev/templify/issues/87)) ([71a1fa6](https://github.com/TriasDev/templify/commit/71a1fa689c24bf27c86b24a096332c7f720a2b78))

## [Unreleased]

## [1.6.0] - 2026-03-16

### Added
- **Header & Footer Support** - Process placeholders, conditionals, and loops in document headers and footers (#15)
  - All header/footer types supported: Default, First Page, Even Page
  - Same syntax and features as document body - no additional API calls needed
  - Formatting is preserved in headers and footers
- **Non-Boolean Format Specifiers** - Format numeric, string, and date values directly in placeholders (#22)
  - `:currency` — locale-aware currency formatting (e.g., `$1,234.56` or `1.234,56 €`)
  - `:number:FORMAT` — any .NET numeric format string (e.g., `:number:N2`, `:number:F3`, `:number:P`)
  - `:uppercase` / `:lowercase` — string casing transformations
  - `:date:FORMAT` — any .NET date format string (e.g., `:date:yyyy-MM-dd`, `:date:MMMM d, yyyy`)
  - Works with int, long, decimal, double, float, DateTime, DateTimeOffset, and ISO date strings
  - Culture-aware formatting throughout
- **Unified Equality Operators** - `==` now works as an alias for `=` in both `{{#if}}` conditionals and `{{(...)}}` boolean expressions (#84)
  - Condition validation detects unknown operators (`===`, `<>`, `&&`, `||`) and structural issues (missing operands, unbalanced quotes, consecutive operators)
- **GUI Culture Selector** - Dropdown to choose formatting culture (Invariant, en-US, de-DE, fr-FR, es-ES)

### Improved
- Test coverage increased to 1,095 tests

## [1.5.0] - 2026-02-13

### Added
- **DocumentProperties Option** - Set document metadata properties on the output document (#77)
  - `Author`, `Title`, `Subject`, `Description`, `Keywords`, `Category`, `LastModifiedBy`
  - Null properties preserve original template values; non-null values overwrite
  - Configure via `PlaceholderReplacementOptions.DocumentProperties`
- **Custom Templify Icon and Branding** - New icon for the library, GUI, and documentation (#76)

### Improved
- Test coverage increased to 972 tests

## [1.4.2] - 2026-02-09

### Fixed
- **Case-insensitive boolean comparison** in ConditionalEvaluator - boolean values like `True`/`False`/`TRUE`/`FALSE` are now correctly compared regardless of case, while preserving case-sensitive string comparisons (#72)

### Improved
- Test coverage increased to 965 tests

## [1.4.1] - 2026-01-07

### Added
- **Processing Warnings System** - Collect non-fatal warnings during template processing
  - `ProcessingWarning` class with warning type, variable name, context, and message
  - Warning types: `MissingVariable`, `MissingLoopCollection`, `NullLoopCollection`, `ExpressionFailed`
  - Access warnings via `ProcessingResult.Warnings` and `ProcessingResult.HasWarnings`
  - Generate Word document warning reports with `GetWarningReport()` and `GetWarningReportBytes()`
- GUI: "Generate Warning Report" button and warning summary display

### Improved
- Test coverage increased to 953 tests

## [1.4.0] - 2026-01-07

### Added
- **UpdateFieldsOnOpen Option** - Automatically prompt Word to refresh TOC and dynamic fields when documents are opened
  - `UpdateFieldsOnOpenMode.Never` - Never prompt (default, backward compatible)
  - `UpdateFieldsOnOpenMode.Always` - Always prompt to update fields
  - `UpdateFieldsOnOpenMode.Auto` - Only prompt if document contains dynamic fields (recommended)
  - Auto mode detects: TOC, PAGE, NUMPAGES, PAGEREF, DATE, TIME, FILENAME, REF, NOTEREF, SECTIONPAGES
  - Solves stale page numbers when content changes via conditionals/loops

### Improved
- Test coverage increased to 939 tests
- New test helpers: DocumentBuilder and DocumentVerifier for cleaner TOC testing
- Updated DocumentFormat.OpenXml to 3.4.1 (performance improvements)

## [1.3.0] - 2026-01-05

### Added
- **Text Replacement Lookup Tables** - Pre-process text before template processing
  - `TextReplacementLookup` for custom character/string replacements
  - `HtmlEntityPreset` for common HTML entities (`&amp;`, `&lt;`, `&gt;`, `&nbsp;`, `&mdash;`, `&ndash;`, etc.)
  - GUI support for HTML entity replacement option
- **Named Iteration Variable Syntax** - Access parent loop variables in nested loops
  - New syntax: `{{#foreach item in CollectionName}}...{{item.Property}}...{{/foreach}}`
  - Access parent scope: `{{category.Name}}` inside `{{#foreach product in category.Products}}`
- **ElseIf Support for Conditionals** - Multi-branch conditional logic with `{{#elseif condition}}` syntax
  - Chain multiple conditions: `{{#if A}}...{{#elseif B}}...{{#elseif C}}...{{#else}}...{{/if}}`
  - Conditions evaluated in order - first matching branch wins
  - Strict validation: `{{#else}}` must be the last branch
  - Full support for block-level, inline, and table row conditionals
- **Newline Character Support** - Variable values can now contain `\n` for line breaks
- **Inline Conditionals** - Conditionals within a single paragraph
- **Highlight and Shading Preservation** - Per-run placeholder replacement now preserves highlight and shading formatting
- **Typographic Quote Support** - Conditional expressions now accept curly/smart quotes (`""` `''`)
- **.NET 10 Support** - Added `net10.0` target framework

### Changed
- **BREAKING:** `{{else}}` syntax changed to `{{#else}}` for consistency with other control tags

### Fixed
- Conditionals inside loops now evaluate with correct context
- Loop-scoped variables are now correctly validated in template validation
- Null values are now treated as valid in template validation
- Nested paragraphs no longer generated in RepeatingConverter

### Improved
- Test coverage increased to 929 tests
- Updated NuGet dependencies

## [1.2.0] - 2025-12-15

### Added
- **TextTemplateProcessor** - Process email and plain text templates using the same syntax as Word documents

## [1.1.0] - 2025-12-02

### Added
- **Standalone Condition Evaluation API** - Use Templify's condition engine without processing Word documents
  - `IConditionEvaluator` interface for evaluating conditional expressions against data
  - `ConditionEvaluator` implementation with full operator support
  - `IConditionContext` interface for efficient batch evaluation of multiple expressions
  - `ConditionContext` implementation for reusable evaluation contexts
  - `CreateConditionContext()` methods for creating batch evaluation contexts
  - Async methods with `CancellationToken` support
  - Thread-safe implementation
- **Developer Documentation** - New documentation section for developers
  - Comprehensive condition evaluation API guide
  - Code examples for Dictionary and JSON data sources

### Changed
- Documentation reorganized into template author and developer sections
- Clarified case sensitivity behavior for JSON keys vs object properties

### Improved
- Code quality enforcement via `.editorconfig` rules
- Test coverage increased to 743 tests

## [1.0.0] - 2025-11-20

### Added
- Initial public release of Templify - a high-performance Word document templating engine for .NET
- **Core Features:**
  - Placeholder replacement with `{{variableName}}` syntax
  - Nested property paths: `{{Customer.Address.City}}`
  - Array/list indexing: `{{Items[0].Name}}`
  - Dictionary access: `{{Settings[Theme]}}` or `{{Settings.Theme}}`
- **Conditional Blocks:**
  - If/else statements: `{{#if condition}}...{{#else}}...{{/if}}`
  - Boolean operators: `and`, `or`, `not`
  - Comparison operators: `=`, `!=`, `>`, `<`, `>=`, `<=`
  - Nested conditionals support
- **Loops:**
  - Collection iteration: `{{#foreach Items}}...{{/foreach}}`
  - Table row loops for dynamic tables
  - Loop metadata: `{{@index}}`, `{{@first}}`, `{{@last}}`, `{{@count}}`
  - Nested loops support (arbitrary depth)
- **Markdown Formatting:**
  - Bold: `**text**` or `__text__`
  - Italic: `*text*` or `_text_`
  - Strikethrough: `~~text~~`
  - Combined: `***text***` for bold+italic
- **Format Specifiers:**
  - Boolean formatters: `:checkbox`, `:yesno`, `:truefalse`, `:onoff`
  - Date/number formatting via standard .NET format strings
- **Architecture:**
  - Visitor pattern for extensible document processing
  - Multi-targeting support for .NET 6, 8, and 9
  - Zero dependencies (only DocumentFormat.OpenXml)
  - 100% test coverage with 109+ tests
- **Tools:**
  - TriasDev.Templify.Converter - CLI for migrating from OpenXMLTemplates
  - TriasDev.Templify.Gui - Cross-platform Avalonia GUI application
  - TriasDev.Templify.Demo - Example console application
  - Helper scripts for common operations
- **Documentation:**
  - Comprehensive README with examples
  - Architecture documentation
  - API reference
  - Tutorials and guides
  - Contributing guidelines
  - Security policy

### Performance
- Processes 1,000 placeholders in ~50ms
- Handles 100 loops in ~150ms
- Evaluates 500 conditionals in ~30ms
- Complex 50-page documents in ~500ms

### Compatibility
- Supports .NET 6.0, 8.0, and 9.0
- Works with Word 2007+ documents (.docx)
- Cross-platform: Windows, Linux, macOS
- No Microsoft Word installation required

[Unreleased]: https://github.com/TriasDev/templify/compare/v1.6.0...HEAD
[1.6.0]: https://github.com/TriasDev/templify/compare/v1.5.0...v1.6.0
[1.5.0]: https://github.com/TriasDev/templify/compare/v1.4.2...v1.5.0
[1.4.2]: https://github.com/TriasDev/templify/compare/v1.4.1...v1.4.2
[1.4.1]: https://github.com/TriasDev/templify/compare/v1.4.0...v1.4.1
[1.4.0]: https://github.com/TriasDev/templify/compare/v1.3.0...v1.4.0
[1.3.0]: https://github.com/TriasDev/templify/compare/v1.2.0...v1.3.0
[1.2.0]: https://github.com/TriasDev/templify/compare/v1.1.0...v1.2.0
[1.1.0]: https://github.com/TriasDev/templify/compare/v1.0.0...v1.1.0
[1.0.0]: https://github.com/TriasDev/templify/releases/tag/v1.0.0
