# beam_dataflow

1. Change the project name, datasetid, table id according to your need(both in BigQueryTornadoes.java and in mvn command)

2. export the service account json as credential 

3. run the mvn command inside beam_dataflow/bigquerytest  

4. command for my case :-
    mvn compile exec:java -Dexec.mainClass=org.apache.beam.examples.BigQueryTornadoes  -Dexec.args="--runner=DataflowRunner --project=bigquey --region=us-central1 --gcpTempLocation=gs://apbucket2/tmp --tempLocation=gs://apbucket2/tmp --input=foo.tornado --output=foo.tornado_res_2" -Pdataflow-runner


