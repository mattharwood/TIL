# Detecting if in a docker container with Dotnet

Set an environment variable on the container e.g. INDOCKER to true.

Then decide upon the value of that environment variable for example:
if (Environment.GetEnvironmentVariable("INDOCKER") == "true")