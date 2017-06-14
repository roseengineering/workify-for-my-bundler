
If you use the bundler program in my bundler repo, 
a bundled module can be run as a web worker using the following call:

     import workify from 'workify';
     let w = workify('./app');

The function returns a web worker.  The workify function in effect
rebundles the modules so the named module is the first to be executed
instead of the original entry point.  The resulting blob is passed 
to Worker() as the url which returns the web worker.

Copyright 2017 roseengineering

