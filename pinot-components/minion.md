# Minion

Pinot Minion is a new component which leverages the [Helix Task Framework](https://engineering.linkedin.com/blog/2019/01/managing-distributed-tasks-with-helix-task-framework) . It can be attached to an existing Pinot cluster and then execute tasks as provided by the controller. It's a generic and single  place for running background jobs. They help offload computationally intensive tasks—such as adding indexes to segments and merging segments—from other components.

## Starting Minion

```text
bin/pinot-admin.sh StartMinion -clusterName pinot-quickstart -zkAddress localhost:2181 -configFileName ${PINOT_DIR}/config/pinot-minion.conf

**pinot-minion.conf**

pinot.minion.port=6000
pinot.minion.adminapi.port=6001
pinot.set.instance.id.to.hostname=true
dataDir=/minion-data-dir
instance.enable.split.commit=true
```

