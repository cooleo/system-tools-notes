# How does DNS worked?

How DNS Works. When a user types a human-readable address into the browser, 
the operating system's DNS client will check for information in a local cache. ... 
When the local DNS server receives the query, and the requested domain name is found, it will return the result.

https://cloudacademy.com/blog/how-dns-works/


# What's happen typing Google.com

When a user enters a query to Google (such as www.google.com/search?q=ieee+society), the user’s browser first performs a domain name sys- tem (DNS) lookup to map www.google.com to a particular IP address. To provide sufficient capacity to handle query traffic, our service con- sists of multiple clusters distributed worldwide. Each cluster has around a few thousand machines, and the geographically distributed setup protects us against catastrophic data cen- ter failures (like those arising from earthquakes and large-scale power failures). A DNS-based load-balancing system selects a cluster by accounting for the user’s geographic proximity to each physical cluster. The load-balancing sys- tem minimizes round-trip time for the user’s request, while also considering the available capacity at the various clusters.
The user’s browser then sends a hypertext transport protocol (HTTP) request to one of these clusters, and thereafter, the processing of that query is entirely local to that cluster. A hardware-based load balancer in each clus- ter monitors the available set of Google Web servers (GWSs) and performs local load bal- ancing of requests across a set of them. After receiving a query, a GWS machine coordi- nates the query execution and formats the results into a Hypertext Markup Language (HTML) response to the user’s browser. Fig- ure 1 illustrates these steps.

http://research.google.com/archive/googlecluster.html



