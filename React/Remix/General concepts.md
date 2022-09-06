# Root
`app/root.tsx` is the main "layout" of the application, everything is wrapped within it. Nested content from routes are rendered into the `<Outlet />` component.

# Links
Each route has a links function that exports an array of links (stylesheets, etc.) that should be applied to that route;

```javascript
export function links() {
	return [{ rel: "stylesheet", href: styles }]
}
```

