# AMQ Streams Operator

Any `Kafka` CR from [alm-examples](./alm-examples.yaml) can be used.
If the cluster has FIPS enabled, the flow will fail with the error described in the `status` of [CR shown here](./cr.yaml).

Applying the [workaround described here][fips-jvm] on the controller, will allow the CR to succeed and the Kafka cluster to be created.

[fips-jvm]: https://access.redhat.com/documentation/en-us/red_hat_amq_streams/2.3/html-single/configuring_amq_streams_on_openshift/index#proc-configuring-fips-mode-cluster-operator-str 
