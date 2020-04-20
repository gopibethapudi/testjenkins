@Grab('org.yaml:snakeyaml:1.17')
import org.yaml.snakeyaml.Yaml
import org.yaml.snakeyaml.DumperOptions
import static org.yaml.snakeyaml.DumperOptions.FlowStyle.BLOCK
node
{
      checkout scm;
     
      
      datas = readFile file: "${env.WORKSPACE}/a.yaml"
    println datas.ami.nonprod;
}
