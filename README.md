# Quick Start

    docker run -p 8888:8080 -d phylor/piggydb

PiggyDB is then reachable on `http://localhost:8888`. Default user is `owner` and password is `owner`.

# Use a Data Container

    docker run --name piggydb-data -v /srv/piggydb busybox true
    docker run --name piggydb --volumes-from piggydb-data -p 8888:8080 piggydb
