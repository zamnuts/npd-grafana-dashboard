# npd-grafana-dashboard

This is a forked and patched version of the [Node Problem Detector Grafana
dashboard by kaszpir](https://grafana.com/grafana/dashboards/15549) diverging
from [Revision 1](https://grafana.com/api/dashboards/15549/revisions/1/download).
This dashboard is complementary to the
[kubernetes/node-problem-detector](https://github.com/kubernetes/node-problem-detector)
configured  with the Prometheus exporter.

Sometimes importing doesn't work in newer versions of Grafana
(tested on v8.4.5, but >5.0.0) due to a missing templating datasource;
see [grafana/grafana#10786](https://github.com/grafana/grafana/issues/10786).
This dashboard adds what is missing as depicted in the included minimal
[patch against rev1](node-problem-detector.patch).

No upstream repository was found, so no contribution back to the original is possible.
While the original work does not explicitly have a license, the [Grafana Labs CLA
permits this derivative work](https://github.com/grafana/grafana/blob/99156b40bd142f46349fb1f1d751f6feee9f87ff/docs/sources/developers/cla.md?plain=1#L55-L62)
as part of a [Grafana Labs dashboard contribution
(publishing)](https://github.com/grafana/grafana/blob/99156b40bd142f46349fb1f1d751f6feee9f87ff/CONTRIBUTING.md?plain=1#L9-L13),
and is republished/redistributed under the same clause.
Thanks for the original work [_KaszpiR_](https://github.com/nvtkaszpir)! (Please include
a link to the repo and an accompanying license next time. 🙂)
