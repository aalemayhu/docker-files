# [Hound][0]

> Hound is an extremely fast source code search engine.

To get started create  a config like the following:

    {
        "max-concurrent-indexers" : 2,
        "dbpath" : "data",
        "repos" : {
            "swift" : {
                "url" : "https://github.com/apple/swift.git"
            }
        }
    }

and then run `docker run -it --rm -p 6080:6080 --name houndd -v $(pwd):/hound etsy/hound`.

This file is based on the [README][1] from hound.


[0]: https://github.com/etsy/hound
[1]: https://github.com/etsy/hound/blob/master/README.md


