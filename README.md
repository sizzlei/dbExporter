# dbExporter
## Description
dbExporter 스크립트는 Prometheus를 사용하는 환경에서 각 서버에 Exporter를 설치하고 Prometheus에 Config을 등록하고 재시작하는 번거로움을 없에기 위해 작성된 스크립트입니다. 

사용 정보는 아래와 같습니다. 
<code>
<pre>
Usage: ./dbExporter [Option]

Bash profile:
Note: Account Bash_profile add.
"  alias dbExporter=${base}/dbExporter"

This is Simple MySQL/MariaDB Monitoring Script with Prometheus Exporter.

Version:
  mysqld_exporter 0.10.0
  node_exporter   0.12.0rc3

Usage Port:
  Target -> Monitor   9090    Prometheus Port
  Target -> Monitor   22 SSH Port
  Monitor -> Target   9104    mysqld_exporter
  Monitor -> Target   9100    node_exporter

Option:
  add|ADD    Make mysqld_exporter Config or Monitor server enrollment.
  start|STARTmysqld_exporter and node_exporter Service Start.
  stop|STOP  mysqld_exporter and node_exporter Service Stop.
  status|STATUS   mysqld_exporter and node_exporter Service Status Print.
  help|HELP  This Script Option Print

add Options:
  mysql|MYSQLMake mysqld_exporter Config.
  monitor|MONITOR Monitor server enrollment.
</pre>
</code>
