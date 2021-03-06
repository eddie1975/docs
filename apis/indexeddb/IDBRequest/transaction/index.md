---
title: 'transaction'
attributions:
  - 'Mozilla Developer Network [![cc-by-sa-small-wpd.svg](/assets/thumb/8/8c/cc-by-sa-small-wpd.svg/120px-cc-by-sa-small-wpd.svg.png)](http://creativecommons.org/licenses/by-sa/3.0/us/): [Article](https://developer.mozilla.org/en-US/docs/IndexedDB/IDBRequest)'
  - 'Microsoft Developer Network: [[Windows Internet Explorer API reference](http://msdn.microsoft.com/en-us/library/ie/hh828809%28v=vs.85%29.aspx) Article]'
notes:
  - 'Needs example, spec reference'
readiness: 'In Progress'
relationships:
  applies_to:
    predicate: 'Property of '
    value: apis/indexeddb/IDBRequest
    href: /apis/indexeddb/IDBRequest
standardization_status: 'W3C Proposed Recommendation'
summary: 'The transaction for the request. This property can be null for certain requests, such as for request returned from IDBFactory.open (You''re just connecting to a database, so there is no transaction to return).'
tags:
  - API_Object_Properties
  - API
  - IndexedDB
  - Needs_Examples
uri: apis/indexeddb/IDBRequest/transaction

---
## Summary

The transaction for the request. This property can be null for certain requests, such as for request returned from IDBFactory.open (You're just connecting to a database, so there is no transaction to return).

Property of [apis/indexeddb/IDBRequest](/apis/indexeddb/IDBRequest)[apis/indexeddb/IDBRequest](/apis/indexeddb/IDBRequest)

## Syntax

**Note**: This property is read-only.

``` js
var result = element.transaction;
```

### Syntax

### Standards information

-   [Indexed Database API](http://go.microsoft.com/fwlink/p/?LinkId=224519)
