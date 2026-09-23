# TodoApp

A minimal WPF desktop application for jotting down a simple todo list.

## Features

- Add a new todo item by typing text into the input box and clicking **Create TODO**.
- Added items appear in a scrollable list below the input box.
- Blank or whitespace-only input is ignored.
- The input box is automatically cleared after an item is added.

## Limitations

This is an early-stage app. Currently, todo items:

- Are not persisted (the list resets each time the app is restarted).
- Cannot be edited, marked complete, or removed.

## Requirements

- [.NET 10 SDK](https://dotnet.microsoft.com/download)
- Windows (the app uses WPF, which is Windows-only)
- Visual Studio 2022/2026 (recommended) or the `dotnet` CLI

## Build and Run

### Using Visual Studio

1. Open `TodoApp.slnx` in Visual Studio.
2. Press `F5` (or `Ctrl+F5`) to build and run the app.

### Using the .NET CLI

```powershell
cd TodoApp
dotnet run
```

## Project Structure

- `TodoApp/MainWindow.xaml` - Defines the main window's UI: the input textbox, the "Create TODO" button, and the scrollable list of todo items.
- `TodoApp/MainWindow.xaml.cs` - Code-behind that handles adding new todo items to the list.