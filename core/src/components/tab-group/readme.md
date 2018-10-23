# ion-tabs

Tabs are a top level navigation component for created multiple stacked navs.
The component is a container of individual [Tab](../Tab/) components.

`ion-tabs` is a styleless component that works as a router outlet in
order to handle navigation. When the user does not provide a `ion-tab-bar` in their markup, `ion-tabs`, by default provides one. Notice that `ion-tab-bar` is the UI component that can be used to switch between tabs.

In order to customize the style of the `ion-tab-bar`, it should be included in the user's markup as
direct children of `ion-tabs`, like this:

```html
<style>
  .my-custom-tabs {
    font-size: 20px;
  }
</style>
<ion-tabs>
  <ion-tab label="Indiana Jones"></ion-tab>
  <ion-tab label="Star Wars"></ion-tab>
  <ion-tab label="Jurassic Park"></ion-tab>

  <ion-tab-bar color="danger" layout="icon-start" placement="top"></ion-tab-bar>
</ion-tabs>
```

<!-- Auto Generated Below -->


## Properties

| Property    | Attribute    | Description                                                                     | Type                  |
| ----------- | ------------ | ------------------------------------------------------------------------------- | --------------------- |
| `name`      | `name`       | A unique name for the tabs.                                                     | `string \| undefined` |
| `useRouter` | `use-router` | If `true`, the tabs will use the router and `selectedTab` will not do anything. | `boolean`             |


## Events

| Event              | Detail                       | Description                                                                |
| ------------------ | ---------------------------- | -------------------------------------------------------------------------- |
| `ionChange`        | {tab: HTMLIonTabViewElement} | Emitted when the tab changes.                                              |
| `ionNavDidChange`  |                              | Emitted when the navigation has finished transitioning to a new component. |
| `ionNavWillChange` |                              | Emitted when the navigation is about to transition to a new component.     |
| `ionNavWillLoad`   |                              | Emitted when the navigation will load a component.                         |


## Methods

### `getRouteId() => Promise<RouteID | undefined>`



#### Returns

Type: `Promise<RouteID | undefined>`



### `getSelected() => Promise<HTMLIonTabViewElement | undefined>`

Get the currently selected tab

#### Returns

Type: `Promise<HTMLIonTabViewElement | undefined>`



### `getTab(tabOrIndex: string | number | HTMLIonTabViewElement) => Promise<HTMLIonTabViewElement | undefined>`

Get the tab at the given index

#### Parameters

| Name         | Type                                        | Description |
| ------------ | ------------------------------------------- | ----------- |
| `tabOrIndex` | `HTMLIonTabViewElement \| number \| string` |             |

#### Returns

Type: `Promise<HTMLIonTabViewElement | undefined>`



### `select(tabOrIndex: number | HTMLIonTabViewElement) => Promise<boolean>`

Index or the Tab instance, of the tab to select.

#### Parameters

| Name         | Type                              | Description |
| ------------ | --------------------------------- | ----------- |
| `tabOrIndex` | `HTMLIonTabViewElement \| number` |             |

#### Returns

Type: `Promise<boolean>`



### `setRouteId(id: string) => Promise<RouteWrite>`



#### Parameters

| Name | Type     | Description |
| ---- | -------- | ----------- |
| `id` | `string` |             |

#### Returns

Type: `Promise<RouteWrite>`




----------------------------------------------

*Built with [StencilJS](https://stenciljs.com/)*