### Class 09 Reading Notes

## HTTP Request Lifecycle

- Step 1 - Local Processing
  - the browser pulls out the relevant parts of the request
    - the protocol - `http` comes before `://`
    - the host - `www.example.com` follows `://`
    - an optional port - `:5000` can come after the host
    - the resource path - `/route/to/resource`
    - possible query strings - `?key1=val1&key2=val2`
  - the browser then attempts to resolve the ip address for the given host by looking through its cache of URLs as well as the operating system's cache, the router's cache, and the DNS cache
  - if it finds the target IP in a cache, then step 2, the search for a cache, can be skipped
- Step 2 - Resolving the IP
  - the browser sends out a DNS (Domain Name Service) server request using UDP (User Datagram Protocol)
    - the DNS request has your own target IP and DNS server included so the response can find its way back to you
  - each networking device the receives the request packet uses a routing table to decide where the packet should be sent next
  - DNS servers are made to pass these requests recursively to each other until one has a reference to the host given
  - once a DNS server (or possibly an authoritative nameserver) receives the packet and has the related IP address, it will respond with the host's IP address
  - note that if the host is not found, a response will hopefully come back with an error, but a browser is likely to timeout if the request takes to long to come back as well

[Return to table of contents](../README.md)
