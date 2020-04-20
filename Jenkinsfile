
import groovy.json.JsonSlurper
node
{
      checkout scm;
     
      
      datas = readFile file: "${env.WORKSPACE}/a.yaml"
          def parser = new JsonSlurper()
def json = parser.parseText(datas)
      println json
}
