## Cookie

Note:
My site uses a small cookie to determine whether or not the right assets have been loaded on the page. It stores a hash of the current CSS file, and if the hash is the current one— it will put the CSS link in the header as expected. If it does not match up, whether a new user or one who has an older version of CSS in their cache— then it will inline the CSS file while loading the normal CSS file asnycronously. This will ensure the second visit has the right file within the cache.
