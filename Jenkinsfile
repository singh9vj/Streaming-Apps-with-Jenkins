@Library('codeutils@vishwajeet')

def codeUtils = new org.emirates.java.scalaCodePipeline()

node{
  codeUtils.call()
}

script {
publishCoverage adapters: [coberturaAdapter('target/site/cobertura/coverage.xml')], sourceFileResolver: sourceFiles('NEVER_STORE')
}
