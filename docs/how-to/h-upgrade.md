# Upgrade

In-place upgrades/rollbacks are not possible for major versions.

[note type="caution"]
Due to a bug in mysql-router-k8s charm, refreshing from revision prior to 814 to newer revision cannot happen in a rolling fashion, causing some downtime.
All units will be refreshed at once and the `resume` step is skipped.

Technical details can be found in the [Pull Request #106](https://github.com/canonical/mysql-router-operators/pull/106). 

[/note]


For instructions on carrying out **minor version upgrades**, see the following guides:
* [Minor upgrade](/t/12238), e.g. MySQL Router 8.0.33 -> MySQL Router 8.0.34<br/>
(including charm revision bump 99 -> 102).
* [Minor rollback](/t/12239), e.g. MySQL Router 8.0.34 -> MySQL Router 8.0.33<br/>
(including charm revision return 102 -> 99).