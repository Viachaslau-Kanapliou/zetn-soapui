SoapUI client for ZETN

Development environment: Full Identity configured, WSDLs pulled in. RSI Preferences and Search configured, WSDLs pulled in.

Project file: dev-soapui-project.xml

Test suite Tests, test case Basic. Currently available:
* getImplementationVersion
* getDomainCapabilities
* getActiveSession
* getUserProfile
* getPreferences
* searchAllContent

Other features:
* Added assertions to the requests flagging HTTP 500 responses.
* Added property transfers to handle test credentials and transport of a security token.
* Added both local (VPN-only) and public (IP-restricted) endpoints.

Before executing the test case, submit user credentials to the requests.

Known issues:
* WSDLs come with local hostname that will resolve over VPN only, to make the requests work outside VPN change the endpoint's hostname to the correct public IP. Note that access to this IP is restricted for general public.
* RSI endpoint is not reachable from the BW VPN.