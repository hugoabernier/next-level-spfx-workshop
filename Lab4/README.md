# Lab 4: Consuming Graph

## Exercise 1: Authorize the web part

1. If you're still running your web part, hit <kbd>CTRL</kbd>+<kbd>C</kbd> until prompted to stop.
1. In your `MyEventsWebPart.ts`, add the following line to pass the web part's context to the component:
    ```typescript
      MyEvents,
          {
            description: this.properties.description,
            // BEGIN: Add this line
            context: this.context
            // END
          }
    ```
2. Yes, you'll get some errors. That's fine.
1. Just above where you entered new code, look for `IMyEventsProps.ts` and <kbd>CTRL</kbd>-Click on it to open the definition
1. Just above the `export interface IMyEventsProps`, paste:
```typescript
import { WebPartContext } from '@microsoft/sp-webpart-base';
```
1. Below the `description: string;` add `context: WebPartContext`.

## Exercise 2: SPFx Fast Serve

1. From the terminal or your command prompt type `npm i -g spfx-fast-serve`
1. Once completed, type `spfx-fast-serve`
1. When prompted to do so, type `npm install`
1. Once completed, run `npm run serve`
