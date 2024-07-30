Sure, here is the content formatted using the ```code``` block in Markdown:

```markdown
# Cache Maintenance Instructions

## 1. Clear the Server HTTP Cache
```code
Go to transaction SMICM.
Navigate to Goto -> HTTP Plugin -> Server Cache -> Invalidate Locally and Globally.
```

## 2. Clear Metadata Cache


```code
For Gateway (oData cache clearing): Use transaction /IWFND/CACHE_CLEANUP.
For Backend and Gateway (oData cache clearing): Use transaction /IWBEP/CACHE_CLEANUP.
```

## 3. Synchronize Chip Cache

```code
/UI2/CHIP_SYNCHRONIZE_CACHE
```


```code
/UI2/DELETE_CACHE_AFTER_IMP
```

```code
/UI2/DELETE_CACHE
```


## 4. Run Cache Buster

```code
/UI5/APP_INDEX_CALCULATE
```

## 5. Clear Local Browser Cache
To avoid views and resources being displayed from the local browser cache or to implement cache buster:

```code
/UI2/INVALIDATE_GLOBAL_CACHES
```

## 6. Gateway Cache Cleaning
```code
/n/IWFND/CACHE_CLEANUP 
```

```code
/n/IWBEP/CACHE_CLEANUP
```


### FE Cache
```code
/UI2/INVALIDATE_GLOBAL_CACHES
```


```code
/UI2/INVALIDATE_CLIENT_CACHES
```

```code
/UI2/DELETE_CACHE
```

```code
/UI2/DELETE_CACHE_AFTER_IMP
```

