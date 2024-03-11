# MyProject

MyProject is a C# library that provides file upload and deletion functionalities for IFormFile extensions.

## Usage

### File Upload

```csharp
var formFile = // Get the IFormFile
var filePath = await formFile.UploadFileToAsync("uploads", "images");
Console.WriteLine("File uploaded. Path: " + filePath);
