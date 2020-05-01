
import groovy.json.JsonSlurper
def jenkinsParamValue(file,key)
{
      def data =  datas = readFile file: file
      def parser = new JsonSlurper()
      def json = parser.parseText(datas)
      def val = ''
      json.each {
            s -> if(s.ParameterKey == key)
            {
                 val=s.ParameterValue
            }
      }
      
      return val;
}
node
{
      checkout scm;
     
      
     println jenkinsParamValue("${env.WORKSPACE}/a.json","ecsAmi")
}
