# Menu

Each module can have its own menu.

A *runnable* project orchestrates menus from different modules, and adds its own menu if it needs one.

To manage the menu, go to your `Panel` project (for example `AdminPanel` or `ClientPanel`) and in the root of that directory create a file called `Menu.jsx`.

```
- AdminPanel
    - Menu.jsx
```

Inside `Menu.jsx` write this code:

```
import AirportShuttleIcon from '@mui/icons-material/AirportShuttle'

const menuItems = [
    {
        title: 'Parent menu item',
        icon: AirportShuttleIcon,
        children: [
            {
                title: 'Amazing submenu one',
                path: '/go-here'
            },
            {
                title: 'Amazing submenu two',
                path: '/go-there'
            }
        ]
    }
]

export default menuItems
```

The `Menu.jsx` file should have a default export and its default export should be a JavaScript array.

Parent menu items can have icons. Icons should be selected from [MUI icons](https://mui.com/material-ui/material-icons/).

You can also import module menus and use them:

```
import { BlogMenu } from 'Blog'

const menuItems = [
    ...BlogMenu
]

export default menuItems
```

The convention for naming exports of module menus is `ModuleMenu`. Here are some example:

- `import { BlogMenu } from 'Blog'`
- `import { ConfigurationMenu } from 'Configuration'`
- `import { AccountsMenu } from 'Accounts'`
- `import { GalleriesMenu } from 'Galleries'`

So, the convention is `import { ModuleMenu } from 'Module'`
