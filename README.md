FaultSight
-----------

FaultSight is a web-based visualization tool meant to be used together with [FlipIt](https://github.com/aperson40/FlipIt). FlipIt is an LLVM Based Fault Injector for HPC applications. FaultSight performs analysis upon the injection data from FlipIt, and provides concrete data regarding an application's fault tolerance capabilities. Graphs are generated using D3.js to visualize the fault injection campaign. 

Such graphs include:

- Classification of injections based on instruction type
- Percent of injections based on function (includes type information
- Signals generated
- Trials with detection (includes bit locations and types)
- Latency of detection
- Trials that unexpectedly terminate (includes bit locations and types)

Users can also produce custom graphs by imposing multiple custom constraints through the tool, in addition to extending existing visualization scripts by defining new custom functions.

This program depends on:

- sqlite3
- Flask
- numpy

[Libraries included in FaultSight](https://github.com/einarhorn/FaultSight/wiki/Libraries-used-in-FlipIt)

Usage
-----

These scripts depend on 'numpy', 'matplotlib', and 'sqlite3'.

To use this tool:

1.) Run an injection campaign via FlipIt.

2.) Place the `src` directory and `web.py` within the `analysis` directory in FlipIt.

3.) Run the following command:
    
```
python web.py
```

4.) Navigate to the following url:
    
```
http://127.0.0.1:5000/
```

Need more help?
-----
Please use the [wiki](https://github.com/einarhorn/FaultSight/wiki) for now. More detailed documentation will be uploaded shortly.



