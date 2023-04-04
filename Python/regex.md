---
id: "regex"
aliases:
  - "Usage"
  - "Syntax"
tags:
  - "regex"
  - "python"
---

# Syntax
[regex101](https://regex101.com/)
[regexr](https://regexr.com/)

# Usage
## Use re
```python
re.sub(pattern,repl,str)
re.search(pattern, str)
re.findall(pattern,str)
```

## Use Pandas
```python
df['column_name'].str.contains('pattern')
df['column_name'].str.findall('pattern')
df['column_name'].str.replace('pattern', 'replacement')
```


