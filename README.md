<html>

<head>
  <script>
    ! function() {
      var analytics = window.analytics = window.analytics || [];
      if (!analytics.initialize)
        if (analytics.invoked) window.console && console.error && console.error("Segment snippet included twice.");
        else {
          analytics.invoked = !0;
          analytics.methods = ["trackSubmit", "trackClick", "trackLink", "trackForm", "pageview", "identify", "reset", "group", "track", "ready", "alias", "debug", "page", "once", "off", "on", "addSourceMiddleware", "addIntegrationMiddleware", "setAnonymousId", "addDestinationMiddleware"];
          analytics.factory = function(e) {
            return function() {
              var t = Array.prototype.slice.call(arguments);
              t.unshift(e);
              analytics.push(t);
              return analytics
            }
          };
          for (var e = 0; e < analytics.methods.length; e++) {
            var key = analytics.methods[e];
            analytics[key] = analytics.factory(key)
          }
          analytics.load = function(key, e) {
            var t = document.createElement("script");
            t.type = "text/javascript";
            t.async = !0;
            t.src = "https://cdn.segment.com/analytics.js/v1/" + key + "/analytics.min.js";
            var n = document.getElementsByTagName("script")[0];
            n.parentNode.insertBefore(t, n);
            analytics._loadOptions = e
          };
          analytics.SNIPPET_VERSION = "4.13.1";
          analytics.load("AcKhZlx2vbyw6JSS66VMwE39pcbWeSSS");
          analytics.page('SE Challenge');
        }
    }();
  </script>
  <script src="script.js"></script>
  <link href="https://unpkg.com/tailwindcss@^1.0/dist/tailwind.min.css" rel="stylesheet">
</head>

<body>
  <div class="md:container md:mx-auto">
    <div class="text-4xl">NotNike Home Page</div>
    <ul>
      <li class="mt-2">
        <button class="bg-blue-500 rounded-full font-bold text-white px-4 py-2 transition duration-300 ease-in-out hover:bg-blue-600 mr-6" onclick="send('page')">Home Page</button>
      </li>
      <li class="mt-2">
        <button class="bg-blue-500 rounded-full font-bold text-white px-4 py-2 transition duration-300 ease-in-out hover:bg-blue-600 mr-6" onclick="send('track')">Adult Shoes</button>
      </li>
      <li class="mt-2">
        <button class="bg-blue-500 rounded-full font-bold text-white px-4 py-2 transition duration-300 ease-in-out hover:bg-blue-600 mr-6" onclick="send('track')">Kids Shoes</button>
      </li>
      <li class="mt-2">
        <button class="bg-blue-500 rounded-full font-bold text-white px-4 py-2 transition duration-300 ease-in-out hover:bg-blue-600 mr-6" onclick="send('identify')">Identify</button>
      </li>
      <li class="mt-2">
        <button class="bg-blue-500 rounded-full font-bold text-white px-4 py-2 transition duration-300 ease-in-out hover:bg-blue-600 mr-6" onclick="send('group')">Group</button>
      </li>
    </ul>
  </div>
</body>

</html>
