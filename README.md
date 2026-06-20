# UnrealSharp-Cropout

Welcome to the UnrealSharp-Cropout repository! 

This project is an ongoing effort to convert [Cropout](https://www.unrealengine.com/en-US/blog/cropout-casual-rts-game-sample-project), originally created in Blueprints, into C# using [UnrealSharp](https://github.com/UnrealSharp/UnrealSharp). This project will serve as a learning material to help developers getting started with UnrealSharp!

The C# code is a 1:1 copy of the BPs created by Epic Games.

## Requirements

- **Engine Version**: Unreal Engine 5.8
- **.NET SDK**: 10.0.201 or newer
- **UnrealSharp**: the current `main` branch (supports UE 5.6–5.8)

## Installation

To get started with UnrealSharp-Cropout, follow these steps:

1. **Clone the Repository**

2. **Set Up UnrealSharp**:
    - Clone the UnrealSharp repository into the `Plugins/UnrealSharp` folder located in the project root.

3. **Generate and build**:
    - Right-click `CropoutSampleProject.uproject` and select **Generate Visual Studio project files**, or use UnrealBuildTool: `dotnet "D:\\Program Files\\UE_5.8\\Engine\\Binaries\\DotNET\\UnrealBuildTool\\UnrealBuildTool.dll" -projectfiles -project="I:\\UEProjects\\UnrealSharp-Cropout\\CropoutSampleProject.uproject" -game -engine`.
    - Build the `CropoutSampleProjectEditor` target for `Development Editor | Win64`, then open the `.uproject` in Unreal Editor.

### UE 5.8 compatibility note

This local setup uses UnrealSharp `main` at `a2d2cd4` (the UE 5.8 fixes merge). It includes a small local fix in `UnrealFunctionBase.cs` so zero-argument `UInterface` functions receive a native function pointer. Keep that plugin change when updating UnrealSharp until it is available upstream.

3. **Build and Run the Project**:
    - Open the C++ solution file (`.sln`) located in the project directory.
    - Build and run the project from this solution.

## Getting Started

After installation, you can dive into the C# scripts to see how Blueprint is now implemented using C#.

## Support and Community

If you need help or wish to discuss UnrealSharp, join our community on Discord:

[Discord community](https://discord.gg/HQuJUYFxeV)

## Contributing
I accept pull requests and any contributions you make are **greatly appreciated**.

## License
Distributed under the MIT License. See `LICENSE` for more information.
