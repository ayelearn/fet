The following text has been accessed from https://en.wikipedia.org/wiki/Hypertext_Transfer_Protocol at Fri Aug 9 01:10:20 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















[Page_protected_with_pending_changes]
****** Hypertext Transfer Protocol ******
From Wikipedia, the free encyclopedia
This is the latest_accepted_revision, reviewed on 8 August 2019.
Jump_to_navigation Jump_to_search
Application protocol for distributed, collaborative, hypermedia information
systems
          Hypertext Transfer Protocol
International standard RFC 7230
Developed by           initially CERN; IETF, W3C
Introduced             1991; 28 years ago (1991)
Superseded by          HTTP/2
HTTP
    * Persistence
    * Compression
    * HTTPS
    * QUIC
Request_methods
    * OPTIONS
    * GET
    * HEAD
    * POST
    * PUT
    * DELETE
    * TRACE
    * CONNECT
    * PATCH
Header_fields
    * Cookie
    * ETag
    * Location
    * HTTP_referer
    * DNT
    * X-Forwarded-For
Status_codes
    * 301_Moved_Permanently
    * 302_Found
    * 303_See_Other
    * 403_Forbidden
    * 404_Not_Found
    * 451_Unavailable_For_Legal_Reasons
Security access control methods
    * Basic_access_authentication
    * Digest_access_authentication
    * v
    * t
    * e
Internet_protocol_suite
Application_layer
    * BGP
    * DHCP
    * DNS
    * FTP
    * HTTP
    * HTTPS
    * IMAP
    * LDAP
    * MGCP
    * MQTT
    * NNTP
    * NTP
    * POP
    * ONC/RPC
    * RTP
    * RTSP
    * RIP
    * SIP
    * SMTP
    * SNMP
    * SSH
    * Telnet
    * TLS/SSL
    * XMPP
    * more...
Transport_layer
    * TCP
    * UDP
    * DCCP
    * SCTP
    * RSVP
    * more...
Internet_layer
    * IP
          o IPv4
          o IPv6
    * ICMP
    * ICMPv6
    * ECN
    * IGMP
    * IPsec
    * more...
Link_layer
    * ARP
    * NDP
    * OSPF
    * Tunnels
          o L2TP
    * PPP
    * MAC
          o Ethernet
          o Wi-Fi
          o DSL
          o ISDN
          o FDDI
    * more...
    * v
    * t
    * e
The Hypertext Transfer Protocol (HTTP) is an application_protocol for
distributed, collaborative, hypermedia information systems.[1] HTTP is the
foundation of data communication for the World_Wide_Web, where hypertext
documents include hyperlinks to other resources that the user can easily
access, for example by a mouse click or by tapping the screen in a web_browser.
HTTP was developed to facilitate hypertext and the World Wide Web.
Development of HTTP was initiated by Tim_Berners-Lee at CERN in 1989.
Development of HTTP standards was a coordinated effort by the Internet
Engineering_Task_Force (IETF) and the World_Wide_Web_Consortium (W3C). The
efforts culminated into the publication of a series of Requests_for_Comments
(RFCs). The first definition of HTTP/1.1, the version of HTTP still in common
use, occurred in
RFC 2068 in 1997. This version was deprecated by
RFC 2616 in 1999 which was then also replaced by the
RFC 7230 family of RFCs in 2014.
A later version, HTTP/2, was standardized in 2015. HTTP/3 is the proposed
successor (Internet_Draft) that builds on HTTP/2[2][3] and is now supported by
major web servers and browsers over Transport_Layer_Security (TLS) using an
Application-Layer_Protocol_Negotiation (ALPN) extension[4] where TLS_1.2 or
newer is required.[5]
⁰
***** Contents *****
    * 1_Technical_overview
    * 2_History
    * 3_HTTP_session
          o 3.1_Persistent_connections
          o 3.2_HTTP_session_state
    * 4_HTTP_authentication
          o 4.1_Authentication_realms
    * 5_Message_format
          o 5.1_Request_message
                # 5.1.1_Request_methods
                      # 5.1.1.1_Safe_methods
                      # 5.1.1.2_Idempotent_methods_and_web_applications
                      # 5.1.1.3_Security
                      # 5.1.1.4_Summary_table
          o 5.2_Response_message
                # 5.2.1_Status_codes
    * 6_Encrypted_connections
    * 7_Example_session
          o 7.1_Client_request
          o 7.2_Server_response
    * 8_Similar_protocols
    * 9_See_also
    * 10_References
    * 11_External_links
***** Technical overview[edit] *****
URL beginning with the HTTP scheme and the WWW domain name label
HTTP functions as a requestâresponse protocol in the clientâserver
computing model. A web_browser, for example, may be the client and an
application running on a computer hosting a website may be the server. The
client submits an HTTP request message to the server. The server, which
provides resources such as HTML files and other content, or performs other
functions on behalf of the client, returns a response message to the client.
The response contains completion status information about the request and may
also contain requested content in its message body.
A web browser is an example of a user_agent (UA). Other types of user agent
include the indexing software used by search providers (web_crawlers), voice
browsers, mobile_apps, and other software that accesses, consumes, or displays
web content.
HTTP is designed to permit intermediate network elements to improve or enable
communications between clients and servers. High-traffic websites often benefit
from web_cache servers that deliver content on behalf of upstream_servers to
improve response time. Web browsers cache previously accessed web resources and
reuse them, when possible, to reduce network traffic. HTTP proxy_servers at
private_network boundaries can facilitate communication for clients without a
globally routable address, by relaying messages with external servers.
HTTP is an application_layer protocol designed within the framework of the
Internet_protocol_suite. Its definition presumes an underlying and reliable
transport_layer protocol,[6] and Transmission_Control_Protocol (TCP) is
commonly used. However, HTTP can be adapted to use unreliable protocols such as
the User_Datagram_Protocol (UDP), for example in HTTPU and Simple_Service
Discovery_Protocol (SSDP).
HTTP_resources are identified and located on the network by Uniform_Resource
Locators (URLs), using the Uniform_Resource_Identifiers (URI's) schemes http
and https. For example, including all optional components:
            userinfo          host        port
        âââââââââ´ââââââââ
ââââââ´âââââââââ ââ´â
 http://john.doe:password@www.example.com:123/forum/questions/
?tag=networking&order=newest#top
 âââ¬ââ
âââââââââââââ¬ââââââââââââââââââââââââââââ¬ââââââââââââââââââââââââ¬âââââââââââââââââââââ¬ââ
 scheme         authority                      path                  query
fragment
 URIs are encoded as hyperlinks in HTML documents, so as to form interlinked
hypertext documents.
HTTP/1.1 is a revision of the original HTTP (HTTP/1.0). In HTTP/1.0 a separate
connection to the same server is made for every resource request. HTTP/1.1 can
reuse a connection multiple times to download images, scripts, stylesheets, etc
after the page has been delivered. HTTP/1.1 communications therefore experience
less latency as the establishment of TCP connections presents considerable
overhead.
***** History[edit] *****
Tim_Berners-Lee
The term hypertext was coined by Ted_Nelson in 1965 in the Xanadu_Project,
which was in turn inspired by Vannevar_Bush's 1930s vision of the microfilm-
based information retrieval and management "memex" system described in his 1945
essay "As_We_May_Think". Tim_Berners-Lee and his team at CERN are credited with
inventing the original HTTP, along with HTML and the associated technology for
a web server and a text-based web browser. Berners-Lee first proposed the
"WorldWideWeb" project in 1989ânow known as the World_Wide_Web. The first
version of the protocol had only one method, namely GET, which would request a
page from a server.[7] The response from the server was always an HTML page.[8]
The first documented version of HTTP was HTTP_V0.9 (1991). Dave_Raggett led the
HTTP Working Group (HTTP WG) in 1995 and wanted to expand the protocol with
extended operations, extended negotiation, richer meta-information, tied with a
security protocol which became more efficient by adding additional methods and
header_fields.[9][10]
RFC 1945 officially introduced and recognized HTTP V1.0 in 1996.
The HTTP WG planned to publish new standards in December 1995[11] and the
support for pre-standard HTTP/1.1 based on the then developing
RFC 2068 (called HTTP-NG) was rapidly adopted by the major browser developers
in early 1996. By March that year, pre-standard HTTP/1.1 was supported in
Arena,[12] Netscape_2.0,[12] Netscape Navigator Gold 2.01,[12] Mosaic_2.7,
[citation_needed] Lynx_2.5,[citation_needed] and in Internet_Explorer_2.0.
[citation_needed] End-user adoption of the new browsers was rapid. In March
1996, one web hosting company reported that over 40% of browsers in use on the
Internet were HTTP 1.1 compliant.[citation_needed] That same web hosting
company reported that by June 1996, 65% of all browsers accessing their servers
were HTTP/1.1 compliant.[13] The HTTP/1.1 standard as defined in
RFC 2068 was officially released in January 1997. Improvements and updates to
the HTTP/1.1 standard were released under
RFC 2616 in June 1999.
In 2007, the HTTPbis_Working_Group was formed, in part, to revise and clarify
the HTTP/1.1 specification. In June 2014, the WG released an updated six-part
specification obsoleting
RFC 2616:
RFC 7230, HTTP/1.1: Message Syntax and Routing
RFC 7231, HTTP/1.1: Semantics and Content
RFC 7232, HTTP/1.1: Conditional Requests
RFC 7233, HTTP/1.1: Range Requests
RFC 7234, HTTP/1.1: Caching
RFC 7235, HTTP/1.1: Authentication
HTTP/2 was published as
RFC 7540 in May 2015.
Year HTTP Version
1991 0.9
1996 1.0
1997 1.1
2015 2.0
2018 3.0
***** HTTP session[edit] *****
An HTTP session is a sequence of network request-response transactions. An HTTP
client initiates a request by establishing a Transmission_Control_Protocol
(TCP) connection to a particular port on a server (typically port 80,
occasionally port 8080; see List_of_TCP_and_UDP_port_numbers). An HTTP server
listening on that port waits for a client's request message. Upon receiving the
request, the server sends back a status line, such as "HTTP/1.1 200 OK", and a
message of its own. The body of this message is typically the requested
resource, although an error message or other information may also be returned.
[1]
**** Persistent connections[edit] ****
Main article: HTTP_persistent_connection
In HTTP/0.9 and 1.0, the connection is closed after a single request/response
pair. In HTTP/1.1 a keep-alive-mechanism was introduced, where a connection
could be reused for more than one request. Such persistent connections reduce
request latency perceptibly, because the client does not need to re-negotiate
the TCP 3-Way-Handshake connection after the first request has been sent.
Another positive side effect is that, in general, the connection becomes faster
with time due to TCP's slow-start-mechanism.
Version 1.1 of the protocol also made bandwidth optimization improvements to
HTTP/1.0. For example, HTTP/1.1 introduced chunked_transfer_encoding to allow
content on persistent connections to be streamed rather than buffered. HTTP
pipelining further reduces lag time, allowing clients to send multiple requests
before waiting for each response. Another addition to the protocol was byte
serving, where a server transmits just the portion of a resource explicitly
requested by a client.
**** HTTP session state[edit] ****
HTTP is a stateless_protocol. A stateless protocol does not require the HTTP
server to retain information or status about each user for the duration of
multiple requests. However, some web_applications implement states or server
side_sessions using for instance HTTP_cookies or hidden variables within web
forms.
***** HTTP authentication[edit] *****
HTTP provides multiple authentication schemes such as basic_access
authentication and digest_access_authentication which operate via a challenge-
response mechanism whereby the server identifies and issues a challenge before
serving the requested content.
HTTP provides a general framework for access control and authentication, via an
extensible set of challenge-response authentication schemes, which can be used
by a server to challenge a client request and by a client to provide
authentication information.[14]
**** Authentication realms[edit] ****
The HTTP Authentication specification also provides an arbitrary,
implementation-specific construct for further dividing resources common to a
given root URI. The realm value string, if present, is combined with the
canonical root URI to form the protection space component of the challenge.
This in effect allows the server to define separate authentication scopes under
one root URI.[14]
***** Message format[edit] *****
See also: List_of_HTTP_header_fields
The client sends requests to the server and the server sends responses.
**** Request message[edit] ****
The request message consists of the following:
    * a request line (e.g., GET /images/logo.png HTTP/1.1, which requests a
      resource called /images/logo.png from the server.)
    * request_header_fields (e.g., Accept-Language: en).
    * an empty line
    * an optional message_body
The request line and other header fields must each end with <CR><LF> (that is,
a carriage_return character followed by a line_feed character). The empty line
must consist of only <CR><LF> and no other whitespace.[15] In the HTTP/1.1
protocol, all header fields except Host are optional.
A request line containing only the path name is accepted by servers to maintain
compatibility with HTTP clients before the HTTP/1.0 specification in
RFC 1945.[16]
*** Request methods[edit] ***
An HTTP 1.1 request made using telnet. The request message, response header
section, and response body are highlighted.
HTTP defines methods (sometimes referred to as verbs, but nowhere in the
specification does it mention verb, nor is OPTIONS or HEAD a verb) to indicate
the desired action to be performed on the identified resource. What this
resource represents, whether pre-existing data or data that is generated
dynamically, depends on the implementation of the server. Often, the resource
corresponds to a file or the output of an executable residing on the server.
The HTTP/1.0 specification[17] defined the GET, HEAD and POST methods and the
HTTP/1.1 specification[18] added five new methods: OPTIONS, PUT, DELETE, TRACE
and CONNECT. By being specified in these documents, their semantics are well-
known and can be depended on. Any client can use any method and the server can
be configured to support any combination of methods. If a method is unknown to
an intermediate, it will be treated as an unsafe and non-idempotent method.
There is no limit to the number of methods that can be defined and this allows
for future methods to be specified without breaking existing infrastructure.
For example, WebDAV defined 7 new methods and
RFC 5789 specified the PATCH method.
Method names are case sensitive.[19][20] This is in contrast to HTTP header
field names which are case-insensitive.[21]
  GET
      The GET method requests a representation of the specified resource.
      Requests using GET should only retrieve_data and should have no other
      effect. (This is also true of some other HTTP methods.)[1] The W3C has
      published guidance principles on this distinction, saying, "Web
      application design should be informed by the above principles, but also
      by the relevant limitations."[22] See safe_methods below.
  HEAD
      The HEAD method asks for a response identical to that of a GET request,
      but without the response body. This is useful for retrieving meta-
      information written in response headers, without having to transport the
      entire content.
  POST
      The POST_method requests that the server accept the entity enclosed in
      the request as a new subordinate of the web_resource identified by the
      URI. The data POSTed might be, for example, an annotation for existing
      resources; a message for a bulletin board, newsgroup, mailing list, or
      comment thread; a block of data that is the result of submitting a web
      form to a data-handling process; or an item to add to a database.[23]
  PUT
      The PUT method requests that the enclosed entity be stored under the
      supplied URI. If the URI refers to an already existing resource, it is
      modified; if the URI does not point to an existing resource, then the
      server can create the resource with that URI.[24]
  DELETE
      The DELETE method deletes the specified resource.
  TRACE
      The TRACE method echoes the received request so that a client can see
      what (if any) changes or additions have been made by intermediate
      servers.
  OPTIONS
      The OPTIONS method returns the HTTP methods that the server supports for
      the specified URL. This can be used to check the functionality of a web
      server by requesting '*' instead of a specific resource.
  CONNECT
      [25] The CONNECT method converts the request connection to a transparent
      TCP/IP_tunnel, usually to facilitate SSL-encrypted communication (HTTPS)
      through an unencrypted HTTP_proxy.[26][27] See HTTP_CONNECT_method.
  PATCH
      The PATCH method applies partial modifications to a resource.[28]
All general-purpose HTTP servers are required to implement at least the GET and
HEAD methods, and all other methods are considered optional by the
specification.[29]
** Safe methods[edit] **
Some of the methods (for example, GET, HEAD, OPTIONS and TRACE) are, by
convention, defined as safe, which means they are intended_only_for_information
retrieval and should not change the state of the server. In other words, they
should not have side_effects, beyond relatively harmless effects such as
logging, web caching, the serving of banner_advertisements or incrementing a
web_counter. Making arbitrary GET requests without regard to the context of the
application's state should therefore be considered safe. However, this is not
mandated by the standard, and it is explicitly acknowledged that it cannot be
guaranteed.
By contrast, methods such as POST, PUT, DELETE and PATCH are intended for
actions that may cause side effects either on the server, or external side
effects such as financial_transactions or transmission of email. Such methods
are therefore not usually used by conforming web_robots or web crawlers; some
that do not conform tend to make requests without regard to context or
consequences.
Despite the prescribed safety of GET requests, in practice their handling by
the server is not technically limited in any way. Therefore, careless or
deliberate programming can cause non-trivial changes on the server. This is
discouraged, because it can cause problems for web_caching, search_engines and
other automated agents, which can make unintended changes on the server. For
example, a website might allow deletion of a resource through a URL such as
http://example.com/article/1234/delete, which, if arbitrarily fetched, even
using GET, would simply delete the article.[30]
One example of this occurring in practice was during the short-lived Google_Web
Accelerator beta, which prefetched arbitrary URLs on the page a user was
viewing, causing records to be automatically altered or deleted en masse. The
beta was suspended only weeks after its first release, following widespread
criticism.[31][30]
** Idempotent methods and web applications[edit] **
Methods PUT and DELETE are defined to be idempotent, meaning that multiple
identical requests should have the same effect as a single request (note that
idempotence refers to the state of the system after the request has completed,
so while the action the server takes (e.g. deleting a record) or the response
code it returns may be different on subsequent requests, the system state will
be the same every time[citation_needed]). Methods GET, HEAD, OPTIONS and TRACE,
being prescribed as safe, should also be idempotent, as HTTP is a stateless
protocol.[1]
In contrast, the POST method is not necessarily idempotent, and therefore
sending an identical POST request multiple times may further affect state or
cause further side effects (such as financial_transactions). In some cases this
may be desirable, but in other cases this could be due to an accident, such as
when a user does not realize that their action will result in sending another
request, or they did not receive adequate feedback that their first request was
successful. While web_browsers may show alert_dialog_boxes to warn users in
some cases where reloading a page may re-submit a POST request, it is generally
up to the web application to handle cases where a POST request should not be
submitted more than once.
Note that whether a method is idempotent is not enforced by the protocol or web
server. It is perfectly possible to write a web application in which (for
example) a database insert or other non-idempotent action is triggered by a GET
or other request. Ignoring this recommendation, however, may result in
undesirable consequences, if a user_agent assumes that repeating the same
request is safe when it is not.
** Security[edit] **
The TRACE method can be used as part of a class of attacks known as cross-site
tracing; for that reason, common security advice is for it to be disabled in
the server configuration.[32] Microsoft IIS supports a proprietary "TRACK"
method, which behaves similarly, and which is likewise recommended to be
disabled.[32]
** Summary table[edit] **
HTTP method RFC      Request has Body Response has Safe Idempotent Cacheable
                                      Body
GET         RFC 7231Optional         Yes          Yes  Yes        Yes
HEAD        RFC 7231Optional         No           Yes  Yes        Yes
POST        RFC 7231Yes              Yes          No   No         Yes
PUT         RFC 7231Yes              Yes          No   Yes        No
DELETE      RFC 7231Optional         Yes          No   Yes        No
CONNECT     RFC 7231Optional         Yes          No   No         No
OPTIONS     RFC 7231Optional         Yes          Yes  Yes        No
TRACE       RFC 7231No               Yes          Yes  Yes        No
PATCH       RFC 5789Yes              Yes          No   No         No
**** Response message[edit] ****
The response message consists of the following:
    * a status line which includes the status_code and reason message (e.g.,
      HTTP/1.1 200 OK, which indicates that the client's request succeeded.)
    * response_header_fields (e.g., Content-Type: text/html)
    * an empty line
    * an optional message_body
The status line and other header fields must all end with <CR><LF>. The empty
line must consist of only <CR><LF> and no other whitespace.[15] This strict
requirement for <CR><LF> is relaxed somewhat within message bodies for
consistent use of other system linebreaks such as <CR> or <LF> alone.[33]
*** Status codes[edit] ***
See also: List_of_HTTP_status_codes
In HTTP/1.0 and since, the first line of the HTTP response is called the status
line and includes a numeric status code (such as "404") and a textual reason
phrase (such as "Not Found"). The way the user_agent handles the response
depends primarily on the code, and secondarily on the other response_header
fields. Custom status codes can be used, for if the user agent encounters a
code it does not recognize, it can use the first digit of the code to determine
the general class of the response.[34]
The standard reason phrases are only recommendations, and can be replaced with
"local equivalents" at the web_developer's discretion. If the status code
indicated a problem, the user agent might display the reason phrase to the user
to provide further information about the nature of the problem. The standard
also allows the user agent to attempt to interpret the reason phrase, though
this might be unwise since the standard explicitly specifies that status codes
are machine-readable and reason phrases are human-readable. HTTP status code is
primarily divided into five groups for better explanation of request and
responses between client and server as named:
    * Informational 1XX
    * Successful 2XX
    * Redirection 3XX
    * Client Error 4XX
    * Server Error 5XX
***** Encrypted connections[edit] *****
The most popular way of establishing an encrypted HTTP connection is HTTPS.[35]
Two other methods for establishing an encrypted HTTP connection also exist:
Secure_Hypertext_Transfer_Protocol, and using the HTTP/1.1_Upgrade_header to
specify an upgrade to TLS. Browser support for these two is, however, nearly
non-existent.[36][37][38]
***** Example session[edit] *****
Below is a sample conversation between an HTTP client and an HTTP server
running on www.example.com, port 80.
**** Client request[edit] ****
GET / HTTP/1.1
Host: www.example.com
A client request (consisting in this case of the request line and only one
header field) is followed by a blank line, so that the request ends with a
double newline, each in the form of a carriage_return followed by a line_feed.
The "Host" field distinguishes between various DNS names sharing a single IP
address, allowing name-based virtual_hosting. While optional in HTTP/1.0, it is
mandatory in HTTP/1.1. (The "/" means /index.html if there is one.)
**** Server response[edit] ****
HTTP/1.1 200 OK
Date: Mon, 23 May 2005 22:38:34 GMT
Content-Type: text/html; charset=UTF-8
Content-Length: 138
Last-Modified: Wed, 08 Jan 2003 23:11:55 GMT
Server: Apache/1.3.3.7 (Unix) (Red-Hat/Linux)
ETag: "3f80f-1b6-3e1cb03b"
Accept-Ranges: bytes
Connection: close

<html>
  <head>
    <title>An Example Page</title>
  </head>
  <body>
    <p>Hello World, this is a very simple HTML document.</p>
  </body>
</html>
The ETag (entity tag) header field is used to determine if a cached version of
the requested resource is identical to the current version of the resource on
the server. Content-Type specifies the Internet_media_type of the data conveyed
by the HTTP message, while Content-Length indicates its length in bytes. The
HTTP/1.1 webserver publishes its ability to respond to requests for certain
byte ranges of the document by setting the field Accept-Ranges: bytes. This is
useful, if the client needs to have only certain portions[39] of a resource
sent by the server, which is called byte_serving. When Connection: close is
sent, it means that the web_server will close the TCP connection immediately
after the transfer of this response.
Most of the header lines are optional. When Content-Length is missing the
length is determined in other ways. Chunked transfer encoding uses a chunk size
of 0 to mark the end of the content. Identity encoding without Content-Length
reads content until the socket is closed.
A Content-Encoding like gzip can be used to compress the transmitted data.
***** Similar protocols[edit] *****
The Gopher_protocol is a content delivery protocol that was displaced by HTTP
in the early 1990s. The SPDY protocol is an alternative to HTTP developed at
Google, it is superseded by the new HTTP protocol, HTTP/2.
***** See also[edit] *****
HTTP
    * Persistence
    * Compression
    * HTTPS
    * QUIC
Request_methods
    * OPTIONS
    * GET
    * HEAD
    * POST
    * PUT
    * DELETE
    * TRACE
    * CONNECT
    * PATCH
Header_fields
    * Cookie
    * ETag
    * Location
    * HTTP_referer
    * DNT
    * X-Forwarded-For
Status_codes
    * 301_Moved_Permanently
    * 302_Found
    * 303_See_Other
    * 403_Forbidden
    * 404_Not_Found
    * 451_Unavailable_For_Legal_Reasons
Security access control methods
    * Basic_access_authentication
    * Digest_access_authentication
    * v
    * t
    * e
    * Comparison_of_file_transfer_protocols
    * Constrained_Application_Protocol â a semantically similar protocol to
      HTTP but used UDP or UDP-like messages targeted for devices with limited
      processing capability; re-uses HTTP and other internet concepts like
      Internet_media_type and web linking (RFC 5988)[40]
    * Content_negotiation
    * Curl-loader â HTTP/S loading and testing open-source software
    * Digest_access_authentication
    * Fiddler_(software)
    * HTTP_compression
    * HTTP/2 â developed by the IETF's Hypertext Transfer Protocol Bis
      (httpbis) working group[41]
    * HTTP-MPLEX â A backwards compatible enhancement to HTTP to improve page
      and web object retrieval time in congested networks proposed by Robert
      Mattson
    * List_of_HTTP_header_fields
    * List_of_HTTP_status_codes
    * Representational_state_transfer (REST)
    * Variant_object
    * Web_cache
    * WebSocket
    * Wireshark
***** References[edit] *****
   1. ^ a b c dFielding, Roy T.; Gettys, James; Mogul, Jeffrey C.; Nielsen,
      Henrik Frystyk; Masinter, Larry; Leach, Paul J.; Berners-Lee, Tim (June
      1999). Hypertext_Transfer_Protocol_â_HTTP/1.1. IETF. doi:10.17487/
      RFC2616. RFC 2616.
   2. ^Bishop, Mike. "Hypertext_Transfer_Protocol_(HTTP)_over_QUIC".
      tools.ietf.org. Retrieved 2018-11-19.
   3. ^Cimpanu, Catalin. "HTTP-over-QUIC_to_be_renamed_HTTP/3_|_ZDNet". ZDNet.
      Retrieved 2018-11-19.
   4. ^"Transport_Layer_Security_(TLS)_Application-Layer_Protocol_Negotiation
      Extension". IETF. July 2014. RFC 7301.
   5. ^Belshe, M.; Peon, R.; Thomson, M. "Hypertext_Transfer_Protocol_Version
      2,_Use_of_TLS_Features". Retrieved 2015-02-10.
   6. ^"Overall_Operation". RFC_2616. p. 12. sec. 1.4. doi:10.17487/RFC2616.
      RFC_2616.
   7. ^Berners-Lee, Tim. "HyperText_Transfer_Protocol". World_Wide_Web
      Consortium. Retrieved 31 August 2010.
   8. ^Tim_Berners-Lee. "The_Original_HTTP_as_defined_in_1991". World Wide Web
      Consortium. Retrieved 24 July 2010.
   9. ^Raggett, Dave. "Dave_Raggett's_Bio". World Wide Web Consortium.
      Retrieved 11 June 2010.
  10. ^Raggett, Dave; Berners-Lee, Tim. "Hypertext_Transfer_Protocol_Working
      Group". World Wide Web Consortium. Retrieved 29 September 2010.
  11. ^Raggett, Dave. "HTTP_WG_Plans". World Wide Web Consortium. Retrieved 29
      September 2010.
  12. ^ a b cSimon Spero. "Progress_on_HTTP-NG". World Wide Web Consortium.
      Retrieved 11 June 2010.
  13. ^"HTTP/1.1". Webcom.com Glossary entry. Archived from the_original on
      2001-11-21. Retrieved 2009-05-29.
  14. ^ a bFielding, Roy T.; Reschke, Julian F. (June 2014). Hypertext_Transfer
      Protocol_(HTTP/1.1):_Authentication. IETF. doi:10.17487/RFC7235. RFC
      7235.
  15. ^ a b"HTTP_Message". RFC_2616. p. 31. sec. 4. doi:10.17487/RFC2616. RFC
      2616.
  16. ^"Apache_Week._HTTP/1.1".
  17.  090502 apacheweek.com
  18. ^Berners-Lee, Tim; Fielding, Roy T.; Nielsen, Henrik Frystyk. "Method
      Definitions". Hypertext_Transfer_Protocol_â_HTTP/1.0. IETF.
      pp. 30â32. sec. 8. doi:10.17487/RFC1945. RFC 1945.
  19. ^"Method_Definitions". RFC_2616. pp. 51â57. sec. 9. doi:10.17487/
      RFC2616. RFC_2616.
  20. ^"RFC-7210_section_3.1.1". Tools.ietf.org. Retrieved 2019-06-26.
  21. ^"RFC-7231_section_4.1". Tools.ietf.org. Retrieved 2019-06-26.
  22. ^"RFC-7230_section_3.2". Tools.ietf.org. Retrieved 2019-06-26.
  23. ^Jacobs, Ian (2004). "URIs,_Addressability,_and_the_use_of_HTTP_GET_and
      POST". Technical Architecture Group finding. W3C. Retrieved 26 September
      2010.
  24. ^"POST". RFC_2616. p. 54. sec. 9.5. doi:10.17487/RFC2616. RFC_2616.
  25. ^"PUT". RFC_2616. p. 55. sec. 9.6. doi:10.17487/RFC2616. RFC_2616.
  26. ^"CONNECT". Hypertext_Transfer_Protocol_â_HTTP/1.1. IETF. June 1999.
      p. 57. sec. 9.9. doi:10.17487/RFC2616. RFC 2616. Retrieved 23 February
      2014.
  27. ^Khare, Rohit; Lawrence, Scott (May 2000). Upgrading_to_TLS_Within_HTTP/
      1.1. IETF. doi:10.17487/RFC2817. RFC 2817.
  28. ^"Vulnerability_Note_VU#150227:_HTTP_proxy_default_configurations_allow
      arbitrary_TCP_connections". US-CERT. 2002-05-17. Retrieved 2007-05-10.
  29. ^Dusseault, Lisa; Snell, James M. (March 2010). PATCH_Method_for_HTTP.
      IETF. doi:10.17487/RFC5789. RFC 5789.
  30. ^"Method". RFC_2616. p. 36. sec. 5.1.1. doi:10.17487/RFC2616. RFC_2616.
  31. ^ a bEdiger, Brad (2007-12-21). Advanced_Rails:_Building_Industrial-
      Strength_Web_Apps_in_Record_Time. O'Reilly Media, Inc. p. 188. ISBN 978-
      0596519728. A common mistake is to use GET for an action that updates a
      resource. [...] This problem came into the Rails public eye in 2005, when
      the Google Web Accelerator was released.
  32. ^Cantrell, Christian (2005-06-01). "What_Have_We_Learned_From_the_Google
      Web_Accelerator?". Adobe Blogs. Adobe. Archived from the_original on
      2017-08-19.
  33. ^ a b"Cross_Site_Tracing". OWASP. Retrieved 2016-06-22.
  34. ^"Canonicalization_and_Text_Defaults". RFC_2616. sec. 3.7.1. doi:
      10.17487/RFC2616. RFC_2616.
  35. ^"Status-Line". RFC_2616. p. 39. sec. 6.1. doi:10.17487/RFC2616. RFC
      2616.
  36. ^Canavan, John (2001). Fundamentals of Networking Security. Norwood, MA:
      Artech House. pp. 82â83. ISBN 9781580531764.
  37. ^Zalewski, Michal. "Browser_Security_Handbook". Retrieved 30 April 2015.
  38. ^"Chromium_Issue_4527:_implement_RFC_2817:_Upgrading_to_TLS_Within_HTTP/
      1.1". Retrieved 30 April 2015.
  39. ^"Mozilla_Bug_276813_â_[RFE]_Support_RFC_2817_/_TLS_Upgrade_for_HTTP
      1.1". Retrieved 30 April 2015.
  40. ^Luotonen, Ari; Franks, John (February 22, 1996). Byte_Range_Retrieval
      Extension_to_HTTP. IETF. I-D draft-ietf-http-range-retrieval-00.
  41. ^Nottingham, Mark (October 2010). Web_Linking. IETF. doi:10.17487/
      RFC5988. RFC 5988.
  42. ^"Hypertext_Transfer_Protocol_Bis_(httpbis)_â_Charter". IETF. 2012.

***** External links[edit] *****
 Wikimedia Commons has media related to Hypertext_Transfer_Protocol.
    * "Change_History_for_HTTP". W3.org. Retrieved 2010-08-01.
 A detailed technical history of HTTP.
"Design_Issues_for_HTTP". W3.org. Retrieved 2010-08-01.
 Design Issues by Berners-Lee when he was designing the protocol.
"Classic_HTTP_Documents". W3.org. 1998-05-14. Retrieved 2010-08-01.
 list of other classic documents recounting the early protocol history
HTTP_0.9_â_As_Implemented_in_1991
HTTP/2_Website_Online_Tester
    * v
    * t
    * e
Web_browsers
Features · standards · protocols
                  * Bookmarks
Features          * Extensions
                  * Privacy_mode
                  * Sync
                  * HTML
                        o v5
                  * CSS
                  * DOM
Web standards     * JavaScript
                        o IndexedDB
                        o Web_storage
                        o WebAssembly
                        o WebGL
                  * HTTP
                        o v2
                        o v3
Protocols               o Cookies
                        o Encryption
                  * OCSP
                  * WebRTC
                  * WebSocket
Active
                 * Avast_Secure_Browser
                 * Blisk
                 * Brave
                 * Chrome
                 * Chromium
                 * Coc_Coc
                 * Dragon
                 * Epic
                 * Falkon
                 * Kinza
                 * Maxthon
                 * Opera
Blink-based      * Otter
                 * Puffin
                 * SalamWeb
                 * Samsung_Internet
                 * Silk
                 * Sleipnir
                 * Sputnik
                 * SRWare
                 * Torch
                 * UC
                 * Vivaldi
                 * Whale
                 * Yandex
                 * Firefox
                 * GNU_IceCat
                 * IceDragon
                 * K-Meleon
Gecko-based      * PirateBrowser
                 * SeaMonkey
                 * TenFourFox
                 * Tor
                 * Waterfox
                 * Dolphin
                 * Dooble
                 * GNOME_Web
                 * iCab
WebKit-based     * Konqueror
                 * Midori
                 * OmniWeb
                 * Safari
                 * surf
                 * 360
                 * Avant
                 * Basilisk
                 * Beaker
                 * CM_Browser
                 * Edge
                 * eww
                 * Internet_Explorer
Other            * Links
                 * Lunascape
                 * Lynx
                 * NetFront
                 * NetSurf
                 * Pale_Moon
                 * QQ_browser
                 * qutebrowser
                 * SlimBrowser
                 * w3m
Discontinued
                  * Beonex_Communicator
                  * Camino
                  * Classilla
                  * Conkeror
                  * Galeon
                  * Ghostzilla
                  * Kazehakase
                  * Kylo
Gecko-based       * Lotus
                  * MicroB
                  * Minimo
                  * Mozilla_suite
                  * Pogo
                  * Strata
                  * Swiftfox
                  * Swiftweasel
                  * Timberwolf
                  * xB
                  * AOL
                  * Deepnet
                  * GreenBrowser
                  * MediaBrowser
                  * MenuBox
Trident-based     * NeoPlanet
                  * NetCaptor
                  * SpaceTime
                  * UltraBrowser
                  * WebbIE
                  * ZAC
                  * Arora
                  * BOLT
                  * Opera_Coast
                  * Flock
                  * Fluid
                  * Google_TV
                  * Iris
                  * Mercury
WebKit-based      * Origyn
                  * QtWeb
                  * rekonq
                  * Rockmelt
                  * Shiira
                  * Steel
                  * Browser_for_Symbian
                  * Uzbl
                  * WebPositive
                  * xombrero
                  * abaco
                  * Amaya
                  * Arachne
                  * Arena
                  * Blazer
                  * Charon
                  * Deepfish
                  * Dillo
                  * ELinks
                  * Gazelle
                  * HotJava
                  * IBM_Home_Page
                    Reader
                  * IBM_WebExplorer
Other             * IBrowse
                  * KidZui
                  * Line_Mode
                  * Mosaic
                  * MSN_TV
                  * NetPositive
                  * Netscape
                  * Skweezer
                  * Skyfire
                  * Teashark
                  * The_world_browser
                  * ThunderHawk
                  * Vision
                  * WinWAP
                  * WorldWideWeb
    * Category
    * Comparisons
    * List
    * v
    * t
    * e
Semantic_Web
                   * Databases
                   * Hypertext
                   * Internet
Background         * Ontologies
                   * Semantics
                   * Semantic_networks
                   * World_Wide_Web
                   * Dataspaces
Sub-topics         * Hyperdata
                   * Linked_data
                   * Rule-based_systems
                   * Semantic_analytics
                   * Semantic_broker
                   * Semantic_computing
                   * Semantic_mapper
Applications       * Semantic_matching
                   * Semantic_publishing
                   * Semantic_reasoner
                   * Semantic_search
                   * Semantic_service-oriented_architecture
                   * Semantic_wiki
                   * Collective_intelligence
                   * Description_logic
                   * Folksonomy
                   * Geotagging
                   * Information_architecture
                   * Knowledge_extraction
                   * Knowledge_management
                   * Knowledge_representation_and_reasoning
Related topics     * Library_2.0
                   * Digital_library
                   * Digital_humanities
                   * Metadata
                   * References
                   * Topic_map
                   * Web_2.0
                   * Web_engineering
                   * Web_Science_Trust
                                                 * HTTP
                                                 * IRI
                                                       o URI
                                                 * RDF
                                                       o triples
                                                       o RDF/XML
                                                       o JSON-LD
               Syntax and supporting                   o Turtle
               technologies                            o TriG
                                                       o Notation3
                                                       o N-Triples
                                                       o TriX (no W3C standard)
                                                 * RRID
                                                 * SPARQL
                                                 * XML
                                                 * Semantic_HTML
                                                 * Common_Logic
                                                 * OWL
                                                 * RDFS
               Schemas, ontologies and rules     * Rule_Interchange_Format
                                                 * Semantic_Web_Rule_Language
Standards                                        * ALPS
                                                 * SHACL
                                                 * eRDF
                                                 * GRDDL
                                                 * Microdata
               Semantic annotation               * Microformats
                                                 * RDFa
                                                 * SAWSDL
                                                 * Facebook_Platform
                                                 * DOAP
                                                 * Dublin_Core
               Common vocabularies               * FOAF
                                                 * Schema.org
                                                 * SIOC
                                                 * SKOS
                                                 * hAtom
                                                 * hCalendar
                                                 * hCard
               Microformat vocabularies          * hProduct
                                                 * hRecipe
                                                 * hResume
                                                 * hReview
    * v
    * t
    * e
Uniform_Resource_Identifier (URI) schemes
               * about
               * acct
               * crid
               * data
               * file
               * ftp
               * geo
               * gopher
               * http
               * https
               * info
Official       * ldap
               * mailto
               * nfs
               * nntp
               * sip_/_sips
               * tag
               * tel
               * telnet
               * urn
               * view-source
               * ws_/_wss
               * xmpp
               * coffee
               * ed2k
               * feed
               * finger
Unofficial     * irc_/_irc6_/_ircs
               * ldaps
               * magnet
               * rsync
               * ymsgr
Protocol_list
    * v
    * t
    * e
Web_interfaces
                               * HTTP
                               * CGI
                               * SCGI
            Protocols          * FCGI
                               * AJP
                               * WSRP
                               * WebSocket
                               * C_NSAPI
                               * C_ASAPI
                               * C_ISAPI
                               * COM_ASP
                               * Java_servlet
                                     o container
                               * CLI_OWIN
            Server_APIs        * ASP.NET_Handler
                               * Python_WSGI
                               * Ruby_Rack
                               * JavaScript_JSGI
                               * Perl_PSGI
Server-side                    * Lua_WSAPI
                               * Portlet
                                     o container
                               * mod_include
                               * mod_jk
                               * mod_lisp
                               * mod_mono
                               * mod_parrot
            Apache_modules     * mod_perl
                               * mod_php
                               * mod_proxy
                               * mod_python
                               * mod_wsgi
                               * mod_ruby
                               * Phusion_Passenger
                               * Web_resource vs. Web_service
                               * Open_API
            Topics             * Webhook
                               * Application_server
                                     o comparison
                               * Scripting
                             * C_NPAPI
                                   o LiveConnect
                                   o XPConnect
                             * C_NPRuntime
            Browser_APIs     * C_PPAPI
                                   o NaCl
                             * ActiveX
                             * BHO
                             * XBAP
                                     * Audio
                                     * Canvas
                                     * CORS
                                     * DOM
                                     * DOM_events
                                     * EME
                                     * File
                                     * Geolocation
                                     * IndexedDB
                                     * MSE
Client-side              W3C         * SSE
                                     * SVG
            Web_APIs                 * Video
                                     * WebAuthn
                                     * WebRTC
                                     * WebSocket
                                     * Web_messaging
                                     * Web_storage
                                     * Web_worker
                                     * XMLHttpRequest
                                     * WebAssembly
                         Khronos     * WebCL
                                     * WebGL
                                     * Gears
                         Others      * Web_SQL_Database (formerly W3C)
                                     * WebUSB
                             * Ajax and Remote_scripting vs. DHTML
            Topics           * Mashup
                             * Web_IDL
                             * Scripting
                * Dynamic_web_page
                * Web_standards
Topics          * Rich_web_application
                * Web_API_security
                * Web_application
                * Web_framework
                                              * BNF: cb12556450f (data)
Authority_control [Edit_this_at_Wikidata]     * GND: 4479982-2
                                              * LCCN: sh97000529

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Hypertext_Transfer_Protocol&oldid=909952475"
Categories:
    * Hypertext_Transfer_Protocol
    * Application_layer_protocols
    * Internet_protocols
    * Network_protocols
    * World_Wide_Web
    * World_Wide_Web_Consortium_standards
    * Computer-related_introductions_in_1991
Hidden categories:
    * Articles_with_short_description
    * Wikipedia_pending_changes_protected_pages
    * All_articles_with_unsourced_statements
    * Articles_with_unsourced_statements_from_September_2010
    * Articles_with_unsourced_statements_from_August_2010
    * Articles_with_unsourced_statements_from_October_2016
    * Commons_category_link_is_on_Wikidata
    * Wikipedia_articles_with_BNF_identifiers
    * Wikipedia_articles_with_GND_identifiers
    * Wikipedia_articles_with_LCCN_identifiers
***** Navigation menu *****
**** Personal tools ****
    * Not logged in
    * Talk
    * Contributions
    * Create_account
    * Log_in
**** Namespaces ****
    * Article
    * Talk
⁰
**** Variants ****
**** Views ****
    * Read
    * Edit
    * View_history
⁰
**** More ****
**** Search ****
[Unknown INPUT type][Search][Go]
**** Navigation ****
    * Main_page
    * Contents
    * Featured_content
    * Current_events
    * Random_article
    * Donate_to_Wikipedia
    * Wikipedia_store
**** Interaction ****
    * Help
    * About_Wikipedia
    * Community_portal
    * Recent_changes
    * Contact_page
**** Tools ****
    * What_links_here
    * Related_changes
    * Upload_file
    * Special_pages
    * Permanent_link
    * Page_information
    * Wikidata_item
    * Cite_this_page
**** In other projects ****
    * Wikimedia_Commons
    * Wikibooks
**** Print/export ****
    * Create_a_book
    * Download_as_PDF
    * Printable_version
**** Languages ****
    * Afrikaans
    * Ø§ÙØ¹Ø±Ø¨ÙØ©
    * Asturianu
    * AzÉrbaycanca
    * ØªÛØ±Ú©Ø¬Ù
    * à¦¬à¦¾à¦à¦²à¦¾
    * BÃ¢n-lÃ¢m-gÃº
    * ÐÐµÐ»Ð°ÑÑÑÐºÐ°Ñ
    * ÐÐµÐ»Ð°ÑÑÑÐºÐ°Ñ_(ÑÐ°ÑÐ°ÑÐºÐµÐ²ÑÑÐ°)â
    * ÐÑÐ»Ð³Ð°ÑÑÐºÐ¸
    * Bosanski
    * CatalÃ 
    * ÄeÅ¡tina
    * Cymraeg
    * Dansk
    * Deutsch
    * Eesti
    * ÎÎ»Î»Î·Î½Î¹ÎºÎ¬
    * EspaÃ±ol
    * Esperanto
    * Euskara
    * ÙØ§Ø±Ø³Û
    * FÃ¸royskt
    * FranÃ§ais
    * Gaeilge
    * Galego
    * àªà«àªàª°àª¾àª¤à«
    * íêµ­ì´
    * ÕÕ¡ÕµÕ¥ÖÕ¥Õ¶
    * à¤¹à¤¿à¤¨à¥à¤¦à¥
    * Hrvatski
    * Bahasa_Indonesia
    * Ãslenska
    * Italiano
    * ×¢××¨××ª
    * ÒÐ°Ð·Ð°ÒÑÐ°
    * LatvieÅ¡u
    * LÃ«tzebuergesch
    * LietuviÅ³
    * Magyar
    * ÐÐ°ÐºÐµÐ´Ð¾Ð½ÑÐºÐ¸
    * à´®à´²à´¯à´¾à´³à´
    * à¤®à¤°à¤¾à¤ à¥
    * Bahasa_Melayu
    * ÐÐ¾Ð½Ð³Ð¾Ð»
    * Nederlands
    * à¤¨à¥à¤ªà¤¾à¤²_à¤­à¤¾à¤·à¤¾
    * æ¥æ¬èª
    * Norsk
    * Norsk_nynorsk
    * ÐÐ»ÑÐº_Ð¼Ð°ÑÐ¸Ð¹
    * à¨ªà©°à¨à¨¾à¨¬à©
    * Polski
    * PortuguÃªs
    * RomÃ¢nÄ
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Scots
    * Shqip
    * Simple_English
    * SlovenÄina
    * SlovenÅ¡Äina
    * Ð¡ÑÐ¿ÑÐºÐ¸_/_srpski
    * Srpskohrvatski_/_ÑÑÐ¿ÑÐºÐ¾ÑÑÐ²Ð°ÑÑÐºÐ¸
    * Suomi
    * Svenska
    * Tagalog
    * à®¤à®®à®¿à®´à¯
    * à°¤à±à°²à±à°à±
    * à¹à¸à¸¢
    * Ð¢Ð¾Ò·Ð¸ÐºÓ£
    * TÃ¼rkÃ§e
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * Tiáº¿ng_Viá»t
    * VÃµro
    * Winaray
    * å´è¯­
    * YorÃ¹bÃ¡
    * ç²µèª
    * Zazaki
    * ä¸­æ
Edit_links
    * This page was last edited on 8 August 2019, at 18:05 (UTC).
    * Text is available under the Creative_Commons_Attribution-ShareAlike
      License; additional terms may apply. By using this site, you agree to the
      Terms_of_Use and Privacy_Policy. WikipediaÂ® is a registered trademark of
      the Wikimedia_Foundation,_Inc., a non-profit organization.
    * Privacy_policy
    * About_Wikipedia
    * Disclaimers
    * Contact_Wikipedia
    * Developers
    * Cookie_statement
    * Mobile_view
    * [Wikimedia_Foundation]
    * [Powered_by_MediaWiki]
