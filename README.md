ASCIIMath2TeX.Net
-----------------

This is a direct port of [the official PHP implementation of the ASCIIMath2TeX converter](https://github.com/asciimath/asciimathml/blob/master/asciimath-based/ASCIIMath2TeX.php), using the [Peachpie compiler](https://www.peachpie.io).

Please refer to the original source code for details.

[Install via NuGet](https://www.nuget.org/packages/ASCIIMath2TeX.Net/)

## Example

F# example (from https://github.com/cannorin/FsNote)

```f#
let am2tex (code: string) =
  let am2t = new AMtoTeX()
  am2t.convert(PhpValue.Create(code)).ToString()
```

C# example:
```c#
var am2t = new AMtoTeX();
Console.Write(am2t.convert("3^f-4").ToString());
```
