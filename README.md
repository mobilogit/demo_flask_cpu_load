# CPU Load caused by Flask App
## Purpose
- Run the application
- In the form enter number of seconds and submit
- The script will loop the given number of seconds
- To call 20 cpu loading CPU for 10 seconds from powershell run:

```powershell
 1..20 | % {start-job {curl.exe  http://127.0.0.1:5000/loop/10}}
```

- To remove the background jobs run

```powershell
Get-Job | Remove-Job
```
