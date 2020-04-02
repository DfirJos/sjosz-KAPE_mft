# MFTEcmd CSV to Elasticsearch
Logstash config that uploads CSV file containing parsed MFT with MFTEcmd to Elasticsearch. 
Set pipeline workers to 1, otherwise it might result in vague results - either with the parameter: `--pipeline.worker 1` or in the pipelines.yml)
```
 - pipeline.id: MFT
   pipeline.workers: 1
   path.config: "../config/MFT.conf"
```
This config was tested on Logstash 7.6.1
