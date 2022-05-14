# Eliminate render blocking resource js


### using Defer
```
<script defer src="sitewide.js"></script>
<script defer src="jquery.min.js"></script>
<script defer src="page-specific.js"></script>
```

### using Async 

```
<script async src="sitewide.js"></script>
<script async src="jquery.min.js"></script>
<script async src="page-specific.js"></script>
```
