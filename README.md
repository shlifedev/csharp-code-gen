# chsarp code gen
  very simple code-gen for chsarp language.
  
## Example

```cs
    CodeGenerator generator = new CodeGenerator();
    generator.UsingNamespace("System.Collections.Generic"); 
    generator.CreateClass("Game.Test", "ClassNameTest"); 
    generator.AddField("int", "userId");
    generator.AddField("int", "userId2");
    generator.AddField("int", "userId3"); 
    generator.AddMethod("void", "GetUsers", "//code"); 
    var code = generator.GenerateCode();
```

## Result

```cs
using System.Collections.Generic;
namespace Game.Test {
public class ClassNameTest{
public int userId;  
public int userId2;  
public int userId3;  
public void GetUsers()
{
 //code 
}
}
}

```
