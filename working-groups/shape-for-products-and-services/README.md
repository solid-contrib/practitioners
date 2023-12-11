 # Shape for Products and Services

A working group for developing shapes and catalogs of the products and services offered by organizations and indviduals starting with the Solid Project ecosystem as an example.

### Motivation

There are a number of use cases which can be addressed by having a standard shape for the products and services that an individual or organization creates.  To list some of these use cases needed in the Solid community now, different people are currently trying to provide catalogs of :

* Solid Onboarding Resources
* Solid Developer Tools
* Solid Storage Providers
* Solid Identity Providers
* Solid Applications
* Solid Servers

While it is important to develop shapes specific to each of these kinds of things (for example to differentiate Applications or types of Onboarding Resources), it  would be useful to start with a shape common to all or most of the types of resources, which is what I propose in this repo.

A centralized catlog might store descriptors for an entire ecosystem's product and services.I suggest that we also think about these desriptors as a possible client-to-client spec for Organizations.  I would see this as triples in the WebID-Profile along the lines of `Orgainization provides ProductOrService`, pointing to a descriptor file as described here. If each organization kept its own catalog of descriptors of the products and services phrased in an interoperable way, centralized catalogs could be created by simply having pointers to the profiles.

It's possible that these descriptors might, in some cases belong in a WebID Profile of e.g. an application.  This gets into issues brought up by SAI and Inrupt's method of handling Client IDs.  Let's keep that in the back of our minds but not conflate it with developing a shape separate from the authentication concerns brought up by the Client ID issue.
