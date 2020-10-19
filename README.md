WORK IN PROGRESS, NO REASON TO INSTALL FOR NOW!


# Example Code
You can read from a file, string, or python dict.

```python
from json_search_lang import JsonSearcher


data = JsonSearcher.loads('{"abc": 123}')
data = JsonSearcher({"abc": 123})
with open("example.json") as f:
	data = JsonSearcher.load(f)
```


# Search String Exampels
## Simple path
**Json:**
```json
{
	"player": {
		"hp": 10
	}
}
```

**Search String:**
```
player/hp
```

**output:**
```
10
```

