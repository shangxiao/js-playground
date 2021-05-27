Notes:

* Browsers don't interpret directory imports as index.js, they simply forward
  the request as-is and the server returns whatever for that request, perhaps a
  directory listing? This means that popular structuring of components in their
  own dirs with index.js won't work.
* Component names must have at least one hyphen (-). Reason being that it helps
  with future proofing the HTML standard.
* Components are not self-closing. Failure to do so will not create error
  messages rather will silently embed siblings as children.
