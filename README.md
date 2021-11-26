# sealog

A libcluon-based example setup with microservices listening in on:
* NMEA2000, using a [YDEN-02](https://www.yachtd.com/products/ethernet_gateway.html) and [cluon-nmea2000](https://github.com/MO-RISE/cluon-nmea2000)
* NMEA0183, using a [YDEN-02](https://www.yachtd.com/products/ethernet_gateway.html) and [cluon-nmea0183](https://github.com/MO-RISE/cluon-nmea0183)
* LWE450, using [cluon-lwe450](https://github.com/MO-RISE/cluon-lwe450)

All using the [memo](https://github.com/MO-RISE/memo) message set.

And logging all traffic to disk using [cluon-record](https://github.com/chrberger/cluon-record)

# crowsnest

An example setup of an onboard crowsnest instance with example configuration of:
* Base crowsnest setup without auth (only suitable for a trusted network)
* Connector to N2k messages from the selog udp stream (https://github.com/MO-RISE/crowsnest-connector-cluon-n2k)
* Bridge to crowsnest.mo.ri.se (https://github.com/MO-RISE/crowsnest-bridge-mqtt)