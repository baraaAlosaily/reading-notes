# Local Storage

### Window.localStorage

The localStorage read-only property of the window interface allows you to access a Storage object for the Document's origin; the stored data is saved across browser sessions

- Syntax
  `myStorage = window.localStorage;`

Value:A Storage object which can be used to access the current origin's local storage space.

Exceptions:
SecurityError
The request violates a policy decision, or the origin is not a valid scheme/host/port tuple (this can happen if the origin uses the file: or data: schemes, for example). For example, the user may have their browser configured to deny permission to persist data for the specified origin.

Description
The keys and the values stored with localStorage are always in the UTF-16 DOMString format, which uses two bytes per character. As with objects, integer keys are automatically converted to strings.

localStorage data is specific to the protocol of the document. In particular, for a site loaded over HTTP (e.g., http://example.com), localStorage returns a different object than localStorage for the corresponding site loaded over HTTPS (e.g., https://example.com).

For documents loaded from file: URLs (that is, files opened in the browser directly from the user’s local filesystem, rather than being served from a web server) the requirements for localStorage behavior are undefined and may vary among different browsers.

In all current browsers, localStorage seems to return a different object for each file: URL. In other words, each file: URL seems to have its own unique local-storage area. But there are no guarantees about that behavior, so you shouldn’t rely on it because, as mentioned above, the requirements for file: URLs remains undefined. So it’s possible that browsers may change their file: URL handling for localStorage at any time. In fact some browsers have changed their handling for it over time.

Example

The following snippet accesses the current domain's local Storage object and adds a data item to it using `Storage.setItem().`

`localStorage.setItem('myCat', 'Tom');`
The syntax for reading the localStorage item is as follows:

`const cat = localStorage.getItem('myCat');`
The syntax for removing the localStorage item is as follows:

`localStorage.removeItem('myCat');`
The syntax for removing all the localStorage items is as follows:

`localStorage.clear();`
