## SinjulMSBH \\ Performance Of String Concatenation In C# And .NET Core


BenchmarkDotNet=v0.12.0, OS=Windows 10.0.18363
Intel Core i7-4710HQ CPU 2.50GHz (Haswell), 1 CPU, 8 logical and 4 physical cores
.NET Core SDK=3.1.200-preview-014883BUG 

### SingleLineJoin
| Method | Mean |
|---|---|
| Interpolation | 250.9 ns | 
| PlusOperator | 246.9 ns |
| StringConcatenate | 246.9 ns |
| StringJoin | 229.6 ns |
| StringFormat | 590.7 ns | 
| StringBuilderAppend | 184.5 ns |

### StringJoinComparison
| Method | Mean |
|---|---|
| StringJoin | 135.7 ns | 
| StringJoinList | 221.4 ns |

### OperatorTest  
| Method | Mean |
|---|---|
| PlusOperatorWithResult | 344.6 ns | 
| PlusOperator | 304.9 ns |