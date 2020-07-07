# DistributedSystemInGO
Basic Multi Client Server Distributed Application

1. Create a folder inside your goPath/src named DS
2. cd DS, Clone the repository inside it.
3. To build the package: cd .. && go install DS
4. Go the GoPath: Run Following commands in different terminals.

Node 1 
$ ./bin/DS --makeMasterOnError

Node 2
$ ./bin/DS --myport 8002 --clusterip 127.0.0.1:8001

Node 3
$ ./bin/DS --myport 8004 --clusterip 127.0.0.1:8001

Node 4
$ ./bin/DS --myport 8003 --clusterip 127.0.0.1:8002
