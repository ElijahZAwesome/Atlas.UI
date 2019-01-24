[![Build status](https://ci.appveyor.com/api/projects/status/sqyrd90lnrbfln2g?svg=true)](https://ci.appveyor.com/project/Ciastex/atlas-ui)

### Atlas.UI
Dark and elegant UI toolkit inspired by Visual Studio design for WPF. Tries to extend on the design by chipping in its own features.

### Installation instructions
1. Add a reference to the library in your project.
2. In your `App.xaml`, in `<Application.Resources />` tag, add this:
```
<ResourceDictionary>
    <ResourceDictionary.MergedDictionaries>
        <ResourceDictionary Source="pack://application:,,,/Atlas.UI;component/Themes/Atlas.xaml" />
    </ResourceDictionary.MergedDictionaries>
</ResourceDictionary>
```
This will override styles of `ScrollViewer`, `TextBlock`, `DataGrid` and a few other built-in controls that Atlas does not extend - because of that, the toolkit assumes you won't be using other (including the default) styles in other parts of your application.

The namespace for all controls is `Atlas.UI`. Whenever you want to use an extended control from the toolkit, add this to your namespace declarations: `xmlns:atlas="clr-namespace:Atlas.UI;assembly=Atlas.UI"`.
