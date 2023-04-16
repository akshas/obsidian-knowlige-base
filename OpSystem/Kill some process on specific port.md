
## Find process

``` powershell
netstat -aon | findstr 8080
```

## Get name of process

``` powershell
tasklist | findstr 11748
```


## Kill the process

``` powershell
taskkill /F /PID 11748
```
