# Introduction #

KREX is an acronym for Kettle Repository Export. It is a collection of Kettle (a.k.a. Pentaho Data Integration) jobs and transformations to export the contents of a Kettle database repository to individual .kjb and .ktr files.

# Details #

To get started:
  * Check out this project's sources and place them in a directory on the file system.
  * Download Kettle 3.2 (currently Milestone 1 release)
  * Start spoon and open "export\_repository\_to\_files.kjb". This is the main job.
  * Open the set\_source\_repo\_and\_target\_directory Transformation (1st entry after start)
    * Open "Set Source Repository", the first step in that transformation
    * Set appropriate variables for pdi\_repo\_to\_export, pdi\_repo\_user, pdi\_repo\_password and Save
  * run "export\_repository\_to\_files.kjb"

If all goes well, you should get a directory called pdi\_repo\_export in your home directory (/home/**username** on unix-based systems, and usually C:\Documents and Settings\**username** on windows and friends). In that dirextory you should find a subdirectory named after the repository name you specified. There you should also find the entire directory tree of the exported repository containing the jobs and transformations as .kjb and .ktr files respectively.

Note that this software is offered to you on an As-Is basis with no warranty. Yes, you disk may get corrupted. Your computer may burst into flames. Or perhaps it may just work and suit your needs.

Have fun!