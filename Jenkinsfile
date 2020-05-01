
import groovy.json.JsonSlurper
def jekinsParamValue(file,key)
{
      def data =  datas = readFile file: file
      def parser = new JsonSlurper()
def json = parser.parseText(datas)
      json.each {
            s -> if(s.ParameterKey == key)
            {
                  return s.ParameterValue
            }
      }
}
node
{
      checkout scm;
     
      
     println jenkinsParamValue("${env.WORKSPACE}/a.json","ecsAmi")
}
