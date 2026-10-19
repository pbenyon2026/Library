Home Library: a version that runs entirely on your own device

Files
  index.html            the whole app (works on its own)
  sw.js                 lets the app open without internet once installed
  manifest.webmanifest  name and icon for "Add to Home Screen"
  icon-192.png, icon-512.png

On a computer
  Double-click index.html. It opens in your browser and saves your catalog there.

On a phone
  Phones won't run a page straight from a file, so put this folder on any free
  static web host (for example GitHub Pages or Netlify), open the address on your
  phone, then use "Add to Home Screen". The host only delivers the app; your
  catalog and photos are saved on the phone, not on the host.

Where the data lives
  In your browser's storage on that device (IndexedDB). Each device and browser
  has its own separate catalog. Use "Back up to a file" regularly, and
  "Restore from a file" to move your catalog to another device.

When the internet is used
  Each time you scan a book, its ISBN is looked up on Open Library (and Google
  Books if Open Library doesn't have it). The details and cover are shown so you
  can check them, correct anything that's wrong, and tap "Add to library".
  Nothing is saved until you do. Whatever you save, including the cover image,
  is stored on your device, so the app never needs the internet to show your
  catalog. If you're offline, you can add the book with just its ISBN and use
  "Get details online" later.
