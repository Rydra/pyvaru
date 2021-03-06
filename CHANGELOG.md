# Pyvaru Changelog

## v0.3.0

### Added:

- RuleGroup (which allows the sequential execution of multiple rules)
- [experimental] Bitwise rule negation using "~" (which inverts the rule validation logic)

### Improvements:

- ValidationResult and ValidationException now implement __str__ in order to provide a meaningful representation
- Improved and simplified error handling in apply() method

## v0.2.0

### Improvements:
- ValidationRule's apply_to parameter can now be passed as a lambda expression

### Fixes:
- UniqueItemsRule now works properly with dictionaries by checking values uniqueness

## v0.1.1

### Improvements:
- Attribute/Key/Index errors that may occur in the Validator's get_rules() method are now catched in validate()
implementation and the error properly reported in the ValidationResult

## v0.1.0
### Added:

- Core API (ValidationRule, Validator, ValidationResult, ValidationException)
- Common validation rules
