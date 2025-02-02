# Using Globus
[Globus](http://www.globus.org/) addresses the challenges faced by researchers in moving, sharing, and archiving large volumes of data among distributed sites. With Globus, you hand off data movement tasks to a hosted service that manages the entire operation. It monitors performance and errors, retries failed transfers, corrects problems automatically whenever possible, and reports status to keep you informed and keep you focused on your research. Command line and Web-based interfaces are available. The command line interface, which requires only ssh to be installed on the client, is the method of choice for script-based workflows. Globus also provides a [REST-style transfer API](https://docs.globus.org/api/transfer/) for advanced-use cases that require scripting and automation.

## Getting Started
Basic documentation for getting started with Globus can be found at the following URL:
[https://docs.globus.org/how-to/](https://docs.globus.org/how-to/)

## Data Transfer Node
A total of 13 data transfer nodes (DTNs) for /home, theta-fs0, and Grand (6 of these DTNs are also used for HPSS) and 4 DTNs for Eagle are available to ALCF users, allowing users to perform wide and local area data transfers. Access to the DTNs is provided via the following Globus endpoints:

## ALCF Globus Endpoints
The Globus endpoint and the path to use depends on where your data resides. If your data is on:

* /home which is where your home directory resides: alcf#dtn_theta. Use the path /home/<username\>
* theta-fs0 filesystem: alcf#dtn_theta. Use /projects/<project name\>
* HPSS: alcf#dtn_hpss
* Grand filesystem: alcf#dtn_theta. Use the path /grand/<project name\>
* Eagle filesystem: alcf#dtn_eagle. Use the path /<project name\>

After [registering](https://app.globus.org/), simply use the appropriate ALCF endpoint, as well as other sources or destinations. Use your ALCF credentials (your OTP generated by the CryptoCARD token with PIN or Mobilepass app) to activate the ALCF endpoint.

[Globus Connect Personal](https://www.globus.org/globus-connect-personal) allows users to add laptops or desktops as an endpoint to Globus, in just a few steps. After you set up Globus Connect Personal, Globus can be used to transfer files to and from your computer.

## References
[Research Data Management with Globus](https://www.alcf.anl.gov/support-center/training-assets/research-data-management-globus)
<iframe width="560" height="315" src="https://www.youtube.com/embed/1nCfWslDrf8" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
  
