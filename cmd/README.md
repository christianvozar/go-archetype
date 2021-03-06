# `/cmd`

Application binary main files.

The directory name for each application should match the name of the executable you want to have (e.g., `/cmd/myapp`).

Keep code in application to a minimum. All code that can be imported and used in other projects should live in `/pkg`. If code is not sharable then it should live in `/internal`.

It's common to have a small `main` function that imports and invokes the code from the `/internal` and `/pkg` directories and nothing else.

Examples:

* https://github.com/heptio/ark/tree/master/cmd (just a really small `main` function with everything else in packages)
* https://github.com/moby/moby/tree/master/cmd
* https://github.com/prometheus/prometheus/tree/master/cmd
* https://github.com/influxdata/influxdb/tree/master/cmd
* https://github.com/kubernetes/kubernetes/tree/master/cmd
* https://github.com/satellity/satellity/tree/master/cmd/satellity
* https://github.com/dapr/dapr/tree/master/cmd

