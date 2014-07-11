node-statsd-client
==================

## This is a fork of https://github.com/msiebuhr/node-statsd-client

The patch was kind of hacked together. What it does differently:
 * It sends data over TCP instead of UDP.
 * It closes the connection after 10 intervals of not being used within
   'socketTimeout' instead of 1.
 * socketTimeout still means 'maximum time between when you say you want
   to emit some metrics and when those metrics actually end up getting
   sent'

Original documentation can be found on the parent this was forked from: [Original Fork](https://github.com/msiebuhr/node-statsd-client/).

LICENSE
-------

ISC - see
[LICENSE](https://github.com/msiebuhr/node-statsd-client/blob/master/LICENSE).
