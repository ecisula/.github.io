```markdown
# gylkam.github.io Development Patterns

> Auto-generated skill from repository analysis

## Overview
This skill teaches you the core development patterns and workflows used in the `gylkam.github.io` repository. The project is written in Python without a specific framework, and emphasizes clear documentation, consistent code style, and a straightforward process for updating project documentation. You'll learn file naming conventions, import/export styles, commit message patterns, and how to contribute effectively to the documentation.

## Coding Conventions

### File Naming
- Use **camelCase** for file names.
  - Example: `myModule.py`, `dataProcessor.py`

### Import Style
- Use **relative imports** within modules.
  - Example:
    ```python
    from .utils import helperFunction
    ```

### Export Style
- Use **named exports** (explicitly define what is exported).
  - Example:
    ```python
    def processData(data):
        # processing logic
        return result

    __all__ = ['processData']
    ```

### Commit Messages
- Use the `feat` prefix for new features.
- Commit messages are concise, averaging around 63 characters.
  - Example:
    ```
    feat: add data normalization to preprocessing pipeline
    ```

## Workflows

### Update README Documentation
**Trigger:** When you need to add, clarify, or update documentation or plans in the README.
**Command:** `/update-readme`

1. Open `README.md` in your editor.
2. Add or clarify the necessary information.
3. Save your changes.
4. Commit your changes with a descriptive message, such as:
    ```
    feat: update README with new setup instructions
    ```
5. Push your changes to the repository.

## Testing Patterns

- **Test File Naming:** Test files follow the `*.test.*` pattern.
  - Example: `utils.test.py`
- **Testing Framework:** Not explicitly specified; check individual test files for framework usage.
- **Typical Test Structure:**
  ```python
  def test_someFunction():
      assert someFunction(2) == 4
  ```

## Commands

| Command         | Purpose                                         |
|-----------------|-------------------------------------------------|
| /update-readme  | Update or clarify project documentation in README|

```