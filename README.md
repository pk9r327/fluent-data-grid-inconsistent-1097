# fluent-data-grid-inconsistent-1097

For testing convenience I suggest you create a codespace.

After the codespace has finished initializing, run the following commands.

```bash
# Make sure you are using .net 8
dotnet --list-sdks
```

```bash
# Watch project
dotnet watch
```

Click on the Grid page on NavMenu, the first time everything displays normally. Please click on Grid page on NavMenu again, the grid on the page will not display correctly. (see video below)

<video src="media/20231214-1503-35.9238629.mp4" controls title="Title"></video>

> This only happens when using static SSR, try going to `Pages/Grid.razor` and uncomment line 2 ( `@* @rendermode InteractiveServer *@` ) then test again.