# CMD

- Kill process by port
Find ``PID`` by ``port``, e.g. ``3000``
````
netstat -ano | findstr 3000
taskkill /F /PID <PID>
````