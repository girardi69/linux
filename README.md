# linux  
  
How to download a csv on a server  
curl -O -L https://github.com/girardi69/linux/raw/master/demo.csv  


curl -O -L https://github.com/linuxacademy/content-intro-to-databases-on-linux/raw/master/demo.csv

You can use the V3 API to get a raw file like this (you'll need an OAuth token):

curl -H 'Authorization: token INSERTACCESSTOKENHERE' -H 'Accept: application/vnd.github.v3.raw' -O -L https://api.github.com/repos/*owner*/*repo*/contents/*path*

All of this has to go on one line. The -O option saves the file in the current directory. You can use -o filename to specify a different filename.

To get the OAuth token follow the instructions here: https://help.github.com/articles/creating-an-access-token-for-command-line-use

I've written this up as a gist as well: https://gist.github.com/madrobby/9476733
