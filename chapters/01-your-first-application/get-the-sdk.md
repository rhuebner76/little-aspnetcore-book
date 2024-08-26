## Get the SDK
Search for "download .net core" and follow the instructions on Microsoft's download page to get the .NET Core SDK. After the SDK has finished installing, open up the Terminal (or PowerShell on Windows) and use the `dotnet` command line tool (also called a **CLI**) to make sure everything is working:

```
dotnet --version

8.0.108
```

You can get more information about your platform with the `--info` flag:

```
dotnet --info

.NET SDK:
 Version:           8.0.108
 Commit:            665a05cea7
 Workload version:  8.0.100-manifests.b6724b7a

Runtime Environment:
 OS Name:     Windows
 OS Version:  10.0.22631
 OS Platform: Windows
 RID:         win-x64
 Base Path:   C:\Program Files\dotnet\sdk\8.0.108\

.NET workloads installed:
 Workload version: 8.0.100-manifests.b6724b7a
There are no installed workloads to display.

Host:
  Version:      8.0.8
  Architecture: x64
  Commit:       08338fcaa5

.NET SDKs installed:
  8.0.108 [C:\Program Files\dotnet\sdk]

.NET runtimes installed:
  Microsoft.AspNetCore.App 8.0.8 [C:\Program Files\dotnet\shared\Microsoft.AspNetCore.App]
  Microsoft.NETCore.App 8.0.8 [C:\Program Files\dotnet\shared\Microsoft.NETCore.App]

(more details...)
```

If you see output like the above, you're ready to go!
