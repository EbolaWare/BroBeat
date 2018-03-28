# BroBeat
## Sending static Bro logs directly to ElasticSearch in an ELK environment

General idea here is to read bro logs from file, interpret their mapping, and create elasticCompliant output based on your bro logs. All in a neat, tidy, _open_ package.

I ran into the problem while decending into a rabbit-hole of previously captured logs and pcaps. Beats were a good jumping point, but fell short when it came to trying to find an original timestamp for the log/pcap. After seeing how poorly packetbeat performed, with its limited protocol abilities, I decided to start this project for my after work.

I am still unfamiliar with GoLang, so this will be a python file. At the moment, I have two directions that it may go:
* Directly read Bro logs and ship them.
* Read Bro logs and create/update modules for FileBeat
