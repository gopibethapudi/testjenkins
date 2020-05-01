
import groovy.json.JsonSlurper
node
{
      checkout scm;
     
      
      datas = readFile file: "${env.WORKSPACE}/a.json"
          def parser = new JsonSlurper()
def json = parser.parseText(datas)
      println json.environment
}
