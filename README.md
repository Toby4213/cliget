# cliget

Download login-protected files from the command line using curl, wget or aria2.

This addon will generate commands that emulate the request as though it was
coming from your browser by sending the same cookies, user agent string and
referrer. With this addon you can download email attachments, purchased
software/media, source code from a private repository to a remote server without
having to download the files locally first. If come across a website where
cliget doesn't work, please open an issue providing details to help reproduce
the problem.

*Windows users*: Enable the "Escape with double-quotes" option because Windows
doesn't support single quotes. If you use cygwin, however, you don't need to
enable this option.

**Please be aware** of potential security and privacy implications from cookies
being exposed in the download command.

## TODO
Improvement idea  
  - Add button that sends the curl command base64 encoded to a rest api server via http post
  - Server rest api endpoint, for example python flask or via php (good incentive to learn php)
  - Server returns short link to file, even before it's downloaded
  - placeholder html is copied to the short link location, will be replaced, once the file is downloaded
    - see https://stackoverflow.com/a/30568312
    - show progress of file download in placeholder html
    - indicate failed download in placeholder html, give option to restart download file (max 3 times)
    - remove link for failed download after 1 week
    - keep files for 2 weeks, give option to extend
    - via api key auth, indefinite file storage
