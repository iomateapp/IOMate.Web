# Components

This directory contains Vue components that are used throughout the application. Each component is automatically imported and registered as a global component, allowing for easy usage across different parts of the app.

## Available Components

- **NavigationDrawer**: A sidebar navigation component that includes user information and navigational links.
- **TopBar**: A top navigation bar that includes an icon on the right with a dropdown menu for user actions, such as logging out.

## Usage

To use these components, simply include them in your Vue templates. For example:

```vue
<template>
  <div>
    <NavigationDrawer />
    <TopBar />
  </div>
</template>
```

## Adding New Components

To add a new component, create a new `.vue` file in this directory. The component will be automatically imported and available for use in your application.