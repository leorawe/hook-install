# hook-install
Use hook_install() to copy content value from one field to another (one example of how it can be used)

Module includes two files:  
- [yourmodulename].install file
- [yourmodulename].info.yml

In the lw_updater.install file, there is a function being used called hook_install().  
One replaces the word 'hook' with the name of the module.  
So in this case, the function gets named lw_updater_install.

In this case, a field called field_introduction was created as formatted text.  
The client wanted plain text instead, so the easiest way to achieve this is to create a new field and copy the old field value into
the new field value.  
