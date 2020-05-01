
import groovy.json.JsonSlurper
node
{
      checkout scm;
     
      
      datas = readFile file: "${env.WORKSPACE}/a.json"
          def parser = new JsonSlurper()
def json = parser.parseText(datas)
      json.each {
            s -> if(s.ParameterKey == "ecsAmi")
            {
                  println s.ParameterValue
            }
      }
}
