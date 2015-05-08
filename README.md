SoapUI client for ZETN

Identity configured, WSDLs pulled in.

Test suite Tests, test case Basic. Currently available:
* getImplementationVersion
* getDomainCapabilities
* getActiveSession
* getUserProfile

Other features:
* Added assertions to the requests flagging HTTP 500 responses.
* Added property transfers to handle test credentials and transport of a security token.

Before executing the test case, submit user credentials to the requests.

Known issues:
* WSDLs come with local hostname that will resolve over VPN only, to make the requests work outside VPN change the endpoint's hostname to the correct public IP. Note that access to this IP is restricted for general public.