# DotNetMapper

A simple object mapper for .NET which is a lightweight and fast. It provides a simple and easy-to-use API for mapping objects of one type to another.

## Installation

You can install DotNetMapper via NuGet Package Manager by searching for `DotNetMapper` or by running the following command in the Package Manager Console:

```bash
Install-Package DotNetMapper
```

## Usage

Using DotNetMapper is very easy. Here's an example of how to use it:

```cs
using DotNetMapper;

// Define input and output classes
public class InputClass
{
    public int Id { get; set; }
    public string Name { get; set; }
}

public class OutputClass
{
    public int Id { get; set; }
    public string Name { get; set; }
}

// Map input to output
var input = new InputClass { Id = 1, Name = "John" };
var output = Mapper.Map<InputClass, OutputClass>(input);

// Output will be a new instance of OutputClass with the same values as input
```

## Information

- DotNetMapper is licensed under the MIT License, so feel free to use it in your projects.
- Contributions to DotNetMapper are welcome! If you want to contribute, please fork the repository and submit a pull request.
- If you encounter any bugs or issues, please open an issue on the [GitHub repository](https://github.com/sanamhub/dotnet-mapper) so that they can be addressed.
- DotNetMapper is built with performance in mind. It uses a concurrent dictionary to cache the mapping functions, which ensures that they are only created once and can be used multiple times without being recreated.
