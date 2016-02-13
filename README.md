# ZeroHedgeWS
ZeroHedge Mobile + WEB API implemented in Websharper

This is a ZeroHedge 3 types WEB API and user interfaces:

1. Retrieve give page stories: GET /api/page/{num : integer}. Response will contain JSON array with stories for the current page
2. Retrieve given story based on it's base64 URL, received from the page request above: GET /api/story/{URL: base64 string}
3. Post full text search to the site: POST /api/search/{search keys: URLEncoded string} - will return JSON object conytaining first search page stories for the given keys
4. Retrieve given search page stories: GET /api/search/{keys}/{pagenum : integer}
