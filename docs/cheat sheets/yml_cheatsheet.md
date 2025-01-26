# YAML Indentation Cheat Sheet

YAML (YAML Ain't Markup Language) relies on consistent **spaces** for indentation. Proper indentation is critical for YAML to work correctly. This guide provides examples for all common structures.

---

## General Rules
1. **Use spaces, not tabs** for indentation.
2. **Consistency is key**: Choose 2 or 4 spaces per indentation level and stick with it.
3. Each new block (nested structure) is indented further.

---

## Examples

### 1. Key-Value Pairs
Basic key-value pairs are the simplest YAML structure:
```yaml
key1: value1
key2: value2
```

---

### 2. Nested Key-Value Pairs
Nested structures use consistent indentation:
```yaml
config:
  database:
    host: localhost
    port: 5432
  application:
    name: MyApp
    debug: true
```

---

### 3. Lists
Lists start with a dash (`-`) followed by a space:
```yaml
fruits:
  - apple
  - banana
  - cherry
```

#### Lists of Strings (Inline):
```yaml
colors: [red, blue, green]
```

---

### 4. Lists of Dictionaries
Lists can contain dictionaries, with each dictionary indented consistently:
```yaml
employees:
  - name: John
    age: 30
    role: Developer
  - name: Jane
    age: 25
    role: Designer
```

---

### 5. Multiline Strings
Use a **pipe (`|`)** for multiline strings:
```yaml
description: |
  This is a multiline string.
  Each line is indented to align with the pipe symbol.
  YAML will preserve these line breaks.
```

---

### 6. Nested Structures with Lists
You can combine dictionaries and lists for complex configurations:
```yaml
menu:
  breakfast:
    - item: pancakes
      price: 5.99
    - item: waffles
      price: 6.99
  lunch:
    - item: sandwich
      price: 7.99
    - item: salad
      price: 6.49
  dinner:
    main_course:
      - pasta
      - steak
    desserts:
      - cake
      - ice cream
```

---

### 7. Hierarchical Lists
Hierarchies can mix key-value pairs and nested lists:
```yaml
settings:
  version: 1.2.3
  features:
    enabled:
      - feature1
      - feature2
    disabled:
      - feature3
  users:
    - username: admin
      permissions:
        - read
        - write
        - execute
    - username: guest
      permissions:
        - read
```

---

## Common Errors and Fixes

### 1. Tabs vs. Spaces
**Wrong:**
```yaml
key:
	- value1  # Uses tabs (❌)
```

**Right:**
```yaml
key:
  - value1  # Uses spaces (✔️)
```

---

### 2. Inconsistent Indentation
**Wrong:**
```yaml
key:
    - value1  # 4 spaces
  - value2    # 2 spaces (❌)
```

**Right:**
```yaml
key:
  - value1
  - value2  # Consistent indentation (✔️)
```

---

### 3. Missing Space After Dash
**Wrong:**
```yaml
key:
  -value1  # Missing space after dash (❌)
```

**Right:**
```yaml
key:
  - value1  # Space after dash (✔️)
```

---

## Best Practices
1. **Use 2 spaces for indentation** (common YAML convention).
2. Validate your YAML with tools like [YAML Lint](https://www.yamllint.com/).
3. Use "show invisible characters" in your editor to spot tabs or extra spaces.
4. Avoid deeply nested structures for readability.

---

Good job! 🦖