---
title: Hbase Upgrade
keywords: hbase, ���׷��̵�
last_updated: Mar 8, 2019
sidebar: mydoc_sidebar
permalink: hbaseupgrade.html
disqus: false
---

## ������Ʈ���� Hbase 2.x ������ ����ϰ� �����Ű���?

���� ������ ������ �⺻ ������ Hbase 1.x �����Դϴ�.

������Ʈ �����ͺ��̽����� Hbase 2.x ������ ����ϰ� �ʹٸ�,
������Ʈ�� �ٽ� �������ؾ� �մϴ�. `hbase-shaded-client` ���̺귯���� ������ 2.x �� ����Ǿ� �մϴ�.
(v2.1.1 ����, �׽�Ʈ��)

`hbase2` �������� �߰��ϸ鼭 ���������� �Ϸ���

���� ����̳�

`mvn clean install -P hbase2,release -DskipTests=true`

���� ��� (���� ����)

`mvn clean install -Dhbase.shaded.client.version=2.1.1 -DskipTests=true`
 
�Ǵ� pom.xml ���Ͽ��� ���� ������ �ٲ� �� ���� ����� ����� �� �ֽ��ϴ�.

```java
<!-- hbase -->
<hbase.shaded.client.version>1.2.6.1</hbase.shaded.client.version>
```
