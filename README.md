# FileUploadExtensionForIFormFileNP


MyProject is a C# library that provides file upload and deletion functionalities for IFormFile extensions.

## Usage

```
dotnet add package FileUploadExtensionForIFormFileNP
```

### File Upload

```csharp
var formFile = // Get the IFormFile
var filePath = await formFile.UploadFileToAsync("uploads", "images");
Console.WriteLine("File uploaded. Path: " + filePath);
```

### File Delete

```csharp
var filePath = // Get the path of file
var filePath = await IFormFileExtension.DeleteFileAsync(filePath);
Console.WriteLine("File uploaded. Path: " + filePath);
