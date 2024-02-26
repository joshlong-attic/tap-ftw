# Accelerator Log

## Options
```json
{
  "projectName" : "bootiful-demo",
  "workloadName" : "demo",
  "provideComponentDetails" : false,
  "gitUrl" : "git@github.com:joshlong-attic/tap-ftw.git",
  "gitBranch" : "main",
  "testScanPipelineEnabled" : true,
  "webWorkloadType" : true,
  "autoconfigureActuatorsEnabled" : true,
  "serviceBindingEnabled" : false,
  "nativeCompileEnabled" : true,
  "jvmVersion" : "21",
  "createPostgresDbEnabled" : false,
  "createRmqEnabled" : false,
  "createMongoDbEnabled" : false,
  "createKafkaEnabled" : false,
  "createMySqlDbEnabled" : false,
  "createRedisEnabled" : false,
  "createGitHubRepo" : false,
  "createTilefile" : true,
  "scaleToZeroEnabled" : false,
  "minimumInstanceCount" : "1",
  "kubeContextName" : "akslab4",
  "postgresDbName" : "postgres1",
  "partOf" : "demoapp",
  "lifecycle" : "production",
  "owner" : "default-org",
  "system" : "unknown"
}
```
## Log
```
┏ engine (Chain)
┃  Info Running Chain(GeneratorValidationTransform, UniquePath)
┃ ┏ ┏ engine.transformations[0].validated (Combo)
┃ ┃ ┃  Info Combo running as Chain
┃ ┃ ┃ engine.transformations[0].validated.delegate (Chain)
┃ ┃ ┃  Info Running Chain(Combo)
┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.transformations[0] (Combo)
┃ ┃ ┃ ┃  Info Combo running as Chain
┃ ┃ ┃ ┃ engine.transformations[0].validated.delegate.transformations[0].delegate (Chain)
┃ ┃ ┃ ┃  Info Running Chain(Merge, UniquePath)
┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.transformations[0].delegate.transformations[0] (Merge)
┃ ┃ ┃ ┃ ┃  Info Running Merge(Combo, Combo, Combo, Combo, Combo, Combo, Combo, Combo, Combo, Combo, Combo)
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.transformations[0].delegate.transformations[0].sources[0] (Combo)
┃ ┃ ┃ ┃ ┃ ┃  Info Combo running as Chain
┃ ┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.delegate.transformations[0].delegate.transformations[0].sources[0].delegate (Chain)
┃ ┃ ┃ ┃ ┃ ┃  Info Running Chain(Include, YTT, RewritePath)
┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.transformations[0].delegate.transformations[0].sources[0].delegate.transformations[0] (Include)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Will include [spring-workload.yaml]
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [spring-workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug Tiltfile didn't match [spring-workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug component-info.yaml didn't match [spring-workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug init-github-repo.sh didn't match [spring-workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug k8s-resource.yaml didn't match [spring-workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug kafka.yaml didn't match [spring-workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mongodb.yaml didn't match [spring-workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mysql.yaml didn't match [spring-workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug postgres.yaml didn't match [spring-workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug rabbitmq.yaml didn't match [spring-workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug redis.yaml didn't match [spring-workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug spring-native-workload.yaml didn't match [spring-workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug spring-workload.yaml matched [spring-workload.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┗ Debug .vscode/settings.json didn't match [spring-workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.transformations[0].delegate.transformations[0].sources[0].delegate.transformations[1] (YTT)
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug Wrote values file with json content:   {"createMySqlDbEnabled":false,"partOf":"demoapp","createMongoDbEnabled":false,"serviceBindingEnabled":false,"webWorkloadType":true,"createPostgresDbEnabled":false,"createKafkaEnabled":false,"scaleToZeroEnabled":false,"lifecycle":"production","nativeCompileEnabled":true,"createGitHubRepo":false,"artifactId":"bootiful-demo","testScanPipelineEnabled":true,"gitBranch":"main","autoconfigureActuatorsEnabled":true,"provideComponentDetails":false,"createRedisEnabled":false,"owner":"default-org","postgresDbName":"postgres1","artifactVersion":"0.0.1-beta","workloadName":"demo","minimumInstanceCount":"1","createRmqEnabled":false,"system":"unknown","jvmVersion":"21","createTilefile":true,"kubeContextName":"akslab4","projectName":"bootiful-demo","gitUrl":"git@github.com:joshlong-attic/tap-ftw.git"}
┃ ┃ ┃ ┃ ┃ ┃ ┗  Info Shelling out to YTT with args: [ytt, -f, /tmp/ytt-input12538380276798404544, --data-values-file, /tmp/accelerator-options14760808984627680844.json, --output-files, /tmp/ytt-output3094050581773980253]
┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.transformations[0].delegate.transformations[0].sources[0].delegate.transformations[2] (RewritePath)
┃ ┃ ┃ ┃ ┃ ┗ ┗ Debug Path 'spring-workload.yaml' matched 'spring-workload.yaml' with groups {g0=spring-workload.yaml} and was rewritten to 'demo-workload.yaml'
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.transformations[0].delegate.transformations[0].sources[1] (Combo)
┃ ┃ ┃ ┃ ┃ ┃  Info Combo running as Chain
┃ ┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.delegate.transformations[0].delegate.transformations[0].sources[1].delegate (Chain)
┃ ┃ ┃ ┃ ┃ ┃  Info Running Chain(Include, YTT)
┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.transformations[0].delegate.transformations[0].sources[1].delegate.transformations[0] (Include)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Will include [component-info.yaml]
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [component-info.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug Tiltfile didn't match [component-info.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug component-info.yaml matched [component-info.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug init-github-repo.sh didn't match [component-info.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug k8s-resource.yaml didn't match [component-info.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug kafka.yaml didn't match [component-info.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mongodb.yaml didn't match [component-info.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mysql.yaml didn't match [component-info.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug postgres.yaml didn't match [component-info.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug rabbitmq.yaml didn't match [component-info.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug redis.yaml didn't match [component-info.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug spring-native-workload.yaml didn't match [component-info.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug spring-workload.yaml didn't match [component-info.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┗ Debug .vscode/settings.json didn't match [component-info.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.transformations[0].delegate.transformations[0].sources[1].delegate.transformations[1] (YTT)
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug Wrote values file with json content:   {"createMySqlDbEnabled":false,"partOf":"demoapp","createMongoDbEnabled":false,"serviceBindingEnabled":false,"webWorkloadType":true,"createPostgresDbEnabled":false,"createKafkaEnabled":false,"scaleToZeroEnabled":false,"lifecycle":"production","nativeCompileEnabled":true,"createGitHubRepo":false,"artifactId":"bootiful-demo","testScanPipelineEnabled":true,"gitBranch":"main","autoconfigureActuatorsEnabled":true,"provideComponentDetails":false,"createRedisEnabled":false,"owner":"default-org","postgresDbName":"postgres1","artifactVersion":"0.0.1-beta","workloadName":"demo","minimumInstanceCount":"1","createRmqEnabled":false,"system":"unknown","jvmVersion":"21","createTilefile":true,"kubeContextName":"akslab4","projectName":"bootiful-demo","gitUrl":"git@github.com:joshlong-attic/tap-ftw.git"}
┃ ┃ ┃ ┃ ┃ ┗ ┗  Info Shelling out to YTT with args: [ytt, -f, /tmp/ytt-input4333484131481553211, --data-values-file, /tmp/accelerator-options16168480850602817103.json, --output-files, /tmp/ytt-output17487595091668395707]
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.transformations[0].delegate.transformations[0].sources[2] (Combo)
┃ ┃ ┃ ┃ ┃ ┃  Info Condition (#nativeCompileEnabled) evaluated to true
┃ ┃ ┃ ┃ ┃ ┃  Info Combo running as Chain
┃ ┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.delegate.transformations[0].delegate.transformations[0].sources[2].delegate (Chain)
┃ ┃ ┃ ┃ ┃ ┃  Info Running Chain(Include, YTT, RewritePath)
┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.transformations[0].delegate.transformations[0].sources[2].delegate.transformations[0] (Include)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Will include [spring-native-workload.yaml]
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [spring-native-workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug Tiltfile didn't match [spring-native-workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug component-info.yaml didn't match [spring-native-workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug init-github-repo.sh didn't match [spring-native-workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug k8s-resource.yaml didn't match [spring-native-workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug kafka.yaml didn't match [spring-native-workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mongodb.yaml didn't match [spring-native-workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mysql.yaml didn't match [spring-native-workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug postgres.yaml didn't match [spring-native-workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug rabbitmq.yaml didn't match [spring-native-workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug redis.yaml didn't match [spring-native-workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug spring-native-workload.yaml matched [spring-native-workload.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug spring-workload.yaml didn't match [spring-native-workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┗ Debug .vscode/settings.json didn't match [spring-native-workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.transformations[0].delegate.transformations[0].sources[2].delegate.transformations[1] (YTT)
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug Wrote values file with json content:   {"createMySqlDbEnabled":false,"partOf":"demoapp","createMongoDbEnabled":false,"serviceBindingEnabled":false,"webWorkloadType":true,"createPostgresDbEnabled":false,"createKafkaEnabled":false,"scaleToZeroEnabled":false,"lifecycle":"production","nativeCompileEnabled":true,"createGitHubRepo":false,"artifactId":"bootiful-demo","testScanPipelineEnabled":true,"gitBranch":"main","autoconfigureActuatorsEnabled":true,"provideComponentDetails":false,"createRedisEnabled":false,"owner":"default-org","postgresDbName":"postgres1","artifactVersion":"0.0.1-beta","workloadName":"demo","minimumInstanceCount":"1","createRmqEnabled":false,"system":"unknown","jvmVersion":"21","createTilefile":true,"kubeContextName":"akslab4","projectName":"bootiful-demo","gitUrl":"git@github.com:joshlong-attic/tap-ftw.git"}
┃ ┃ ┃ ┃ ┃ ┃ ┗  Info Shelling out to YTT with args: [ytt, -f, /tmp/ytt-input13226173754603191366, --data-values-file, /tmp/accelerator-options10464014948520591685.json, --output-files, /tmp/ytt-output16074049134122475931]
┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.transformations[0].delegate.transformations[0].sources[2].delegate.transformations[2] (RewritePath)
┃ ┃ ┃ ┃ ┃ ┗ ┗ Debug Path 'spring-native-workload.yaml' matched 'spring-native-workload.yaml' with groups {g0=spring-native-workload.yaml} and was rewritten to 'demo-native-workload.yaml'
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.transformations[0].delegate.transformations[0].sources[3] (Combo)
┃ ┃ ┃ ┃ ┃ ┃  Info Condition (#createPostgresDbEnabled) evaluated to false
┃ ┃ ┃ ┃ ┃ ┗ null ()
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.transformations[0].delegate.transformations[0].sources[4] (Combo)
┃ ┃ ┃ ┃ ┃ ┃  Info Condition (#createRmqEnabled) evaluated to false
┃ ┃ ┃ ┃ ┃ ┗ null ()
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.transformations[0].delegate.transformations[0].sources[5] (Combo)
┃ ┃ ┃ ┃ ┃ ┃  Info Condition (#createMongoDbEnabled) evaluated to false
┃ ┃ ┃ ┃ ┃ ┗ null ()
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.transformations[0].delegate.transformations[0].sources[6] (Combo)
┃ ┃ ┃ ┃ ┃ ┃  Info Condition (#createKafkaEnabled) evaluated to false
┃ ┃ ┃ ┃ ┃ ┗ null ()
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.transformations[0].delegate.transformations[0].sources[7] (Combo)
┃ ┃ ┃ ┃ ┃ ┃  Info Condition (#createMySqlDbEnabled) evaluated to false
┃ ┃ ┃ ┃ ┃ ┗ null ()
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.transformations[0].delegate.transformations[0].sources[8] (Combo)
┃ ┃ ┃ ┃ ┃ ┃  Info Condition (#createRedisEnabled) evaluated to false
┃ ┃ ┃ ┃ ┃ ┗ null ()
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.transformations[0].delegate.transformations[0].sources[9] (Combo)
┃ ┃ ┃ ┃ ┃ ┃  Info Condition (#createGitHubRepo) evaluated to false
┃ ┃ ┃ ┃ ┃ ┗ null ()
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.transformations[0].delegate.transformations[0].sources[10] (Combo)
┃ ┃ ┃ ┃ ┃ ┃  Info Condition (#createTilefile) evaluated to true
┃ ┃ ┃ ┃ ┃ ┃  Info Combo running as Chain
┃ ┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.delegate.transformations[0].delegate.transformations[0].sources[10].delegate (Chain)
┃ ┃ ┃ ┃ ┃ ┃  Info Running Chain(Include, ReplaceText)
┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.transformations[0].delegate.transformations[0].sources[10].delegate.transformations[0] (Include)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Will include [Tiltfile]
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [Tiltfile] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug Tiltfile matched [Tiltfile] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug component-info.yaml didn't match [Tiltfile] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug init-github-repo.sh didn't match [Tiltfile] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug k8s-resource.yaml didn't match [Tiltfile] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug kafka.yaml didn't match [Tiltfile] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mongodb.yaml didn't match [Tiltfile] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mysql.yaml didn't match [Tiltfile] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug postgres.yaml didn't match [Tiltfile] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug rabbitmq.yaml didn't match [Tiltfile] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug redis.yaml didn't match [Tiltfile] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug spring-native-workload.yaml didn't match [Tiltfile] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug spring-workload.yaml didn't match [Tiltfile] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┗ Debug .vscode/settings.json didn't match [Tiltfile] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.transformations[0].delegate.transformations[0].sources[10].delegate.transformations[1] (ReplaceText)
┃ ┃ ┃ ┃ ┗ ┗ ┗  Info Will replace [KUBE_CONTEXT->akslab4, WORKLOAD_FILENAME->demo-workload.yaml, APP_NAME->demo]
┃ ┗ ┗ ┗ ╺ engine.transformations[0].validated.delegate.transformations[0].delegate.transformations[1] (UniquePath)
┗ ╺ engine.transformations[1] (UniquePath)
```
