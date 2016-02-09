# Warp Core Technologies Order Processing System
This is a sample project for demonstrating various Windows Workflow Foundation techniques.

I’ve found that the best way to learn a technology is to just go build something with it. Over the next several posts we are going to be building a complete order processing system using Workflow Foundation and since we need a fake client to build it for we will be taking inspiration from the Star Trek universe.

Our client: Warp Core Technologies. WCT is the leading provider of warp cores and warp core parts throughout the Alpha Quadrant. While the products they sell are cutting edge, their order processing system is not. We will be building a new order processing system using Workflow Foundation and by the end you should see the value that WF provides.

* Order Validation
  * The Federation Council is always signing treaties or setting up blockades. We need to verify that the order is in compliance with   Federation law before we proceed.
* Inventory Check
  * Trade disputes mean we may not always have the requested parts on hand or there may be a delay.
* Currency Conversion
  * WCT deals in Federation Credits but we serve clients using everything from Gold Pressed Latinum to Klingon Talons. We need to convert it.
* Taxation
  * We need to cut taxes for the Federation and the destination planet.
* Invoicing
  * We will generate a PDF (yes, they still use PDFs in the 24th century) and an email invoice.
* Payment Processing
  * We need to take payment and notify our ERP system.

In addition to the basic requirements we also have some service requirements:

* Guaranteed delivery
  * We will be using MSMQ to fire and forget the order. If the order processing system is down we want to hold the message until it comes back up.
* Support for user modifiable workflows
  * We will be building a WPF application utilizing the rehosted designer functionality from WF to allow workflows to be modified on    the fly.
* Testable
  * We will be writing unit and integration tests to ensure compliance with business rules.

By the end of this series we should have a good overview of what Workflow Foundation can provide and how it will help our business.

You can view the entire tutorial at http://code-coverage.net/series/workflow-foundation-tutorial/
