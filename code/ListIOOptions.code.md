# ListIOOptions.groovy
**Source code:**
```groovy
import org.openscience.cdk.io.IChemObjectWriter;
import org.openscience.cdk.io.program.GaussianInputWriter;
import org.openscience.cdk.io.setting.IOSetting;

IChemObjectWriter writer = new GaussianInputWriter();
for (IOSetting setting : writer.getIOSettings()) {
  println "[" + setting.getName() + "]"
  println "Option: " + setting.getQuestion()
  println "Current value: " + setting.getSetting()
}
```
**Output:**
```plain
[OpenShell]
Option: Should the calculation be open shell?
Current value: false
[Comment]
Option: What comment should be put in the file?
Current value: Created with CDK (http://cdk.sf.n...
  et/)
[Memory]
Option: How much memory do you want to use?
Current value: unset
[Command]
Option: What kind of job do you want to perform?
Current value: energy calculation
[ProcessorCount]
Option: How many processors should be used by Ga...
  ussian?
Current value: 1
```