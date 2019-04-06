# HybridizationTypes.groovy
**Source code:**
```groovy
import org.openscience.cdk.interfaces.*;

IAtomType.Hybridization.each {
  println it
}
```
**Output:**
```plain
S
SP1
SP2
SP3
PLANAR3
SP3D1
SP3D2
SP3D3
SP3D4
SP3D5
```