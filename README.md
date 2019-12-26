# openapi2JSON

Script for converting OpenAPI and Swagger YAML specifications to json for use with development tools

```py
import json, sys
from prance import ResolvingParser
parser = ResolvingParser(sys.argv[1])
# parser.specification  # contains fully resolved specs as a dict
print(json.dumps(parser.specification))
```

RuntimeError: No validation backend available! Install one of "flex", "openapi-spec-validator" or "swagger-spec-validator".
