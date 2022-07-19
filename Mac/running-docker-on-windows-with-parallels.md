# Running Docker on Windows with Parallels

In order for the Docker daemon service to run when using Windows through Parallels on a Mac, you need to "Allow Nested Hyperthreading". This option is in the Parallels' settings for the Windows VM.

Otherwise, you'll probably experience Docker Desktop crashing on start up, with no discerable error...

