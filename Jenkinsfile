
import groovy.json.JsonSlurper
def jenkinsParamValue(file,key)
{
      def json = readJSON file: file
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
