Red Siege has created a Windows client (thanks to the massive help of Matt Grandy (@Matt_Grandy_) with the stability fixes). All you need to do is build it locally (or check the releases), and then provide a path to a file containing the URLs you want scanned! SharpWitness will generate the report within your "AppData\Roaming" directory. The latest version of the C# SharpWitness supports parsing and taking screenshots of Internet Explorer and Chrome bookmarks without having to supply a list of URLs. This version is also small enough to be delivered through Cobalt Strike's execute-assembly.

### Setup:
1. Navigate into the CS directory 
2. Load SharpWitness.sln into Visual Studio
3. Go to Build at the top and then Build Solution if no modifications are wanted

### Usage:
```bash
SharpWitness.exe --help
SharpWitness.exe --bookmarks
SharpWitness.exe -f C:\Path\to\urls.txt
SharpWitness.exe --file C:\Path\to\urls.txt --delay [timeout in seconds] --compress
```

