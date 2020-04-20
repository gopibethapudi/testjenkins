node
{
      checkout scm;
      
      
      sh """

ls -ltrh;

"""
      
      datas = readFile file: "${env.WORKSPACE}/a.yml"
    println datas;
}
