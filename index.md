---
layout: page
---

# Open Source Chips for Europe

## Open Letter on the Urgency of Access to Open Source Chip Manufacturing

**To Whom It May Concern**

*March 31, 2025*

The European Chips Act has set ambitious goals and its implementation is a significant pan-european effort. From an academic perspective, last year we published an [open letter emphasizing the critical importance of open-source EDA for academia in Europe](https://open-source-eda-letter.eu). We were excited and grateful to see that this initiative triggered the definition of a [European roadmap in this area](https://fossi-foundation.org/resources/eu-roadmap), and a matching [Chips JU call for project funding](https://www.chips-ju.europa.eu/CallDetails/?id=a9b6319a-bee3-ef11-8eea-6045bde08093). We believe that the projects funded by this call will have a significant impact. Moreover, we already see rising interest from many EU stakeholders, with increasing investments into open-source chip design, especially in open source IP development (e.g. RISC-V cores), and open source EDA tools.

One additional critical barrier remains toward the end-goal of building real open-source chips, especially for prototyping and education: namely, **streamlining the access to open source chip production facilities (foundries) is essential**. Programs like [ChipIgnite](https://web.archive.org/web/20250302154132/https://efabless.com/chipignite), [Tiny Tapeout](https://tinytapeout.com/) and [IHP’s open source program](https://www.ihp-microelectronics.com/services/research-and-prototyping-service/fast-design-enablement/open-source-pdk) have become “guiding stars” that demonstrate that everyone with a computer can build chips. We believe that having low-cost, regular and easy access to chip production is critical to create excitement and build up expertise, widening the pool of chip designers with tape-out experience: a true **silicon democratization** and a further **de-mystification of chip design**‚. 

Currently, academia and companies can get affordable access to chip manufacturing via [EUROPRACTICE-IC](https://europractice-ic.com/), which has been instrumental in supporting IC design in Europe and has so far enabled hundreds of designs to be manufactured. Each silicon manufacturer (foundry) provides a set of rules and configurations that help designers ensure that their ICs can be reliably manufactured, achieving  satisfactory performance. These so-called Process Design Kits (PDKs) have long been proprietary and were made available under non-disclosure agreements. Anyone that wishes to manufacture an IC has to sign an NDA to get access to PDK allowing the design to be completed. 

Up until recently, signing such an NDA (besides a legal complication) did not have that much of a detrimental effect. IC design was only practiced by larger entities and required the use of commercial IP and EDA tools that brought additional restrictions. With the wider adoption of open-source EDA tools and IPs, one by one these restrictions have fallen wayside: **higher quality open-source IP and open-source EDA tools have removed barriers**, leaving the NDAs for technology PDKs one of the few remaining obstacles that limit open collaboration, and the democratization of IC design.

In the past few years, thanks to private financial support, [Skywater 130nm](https://github.com/google/skywater-pdk) and [Globalfoundries 180MCU](https://github.com/google/gf180mcu-pdk) technologies have been released as open PDKs. They were followed by [IHP 130nm](https://github.com/IHP-GmbH/IHP-Open-PDK) technology, released thanks to [German government funding](https://elektronikforschung.de/projekte/ihp-open130-g2). These open PDKs have already enabled the tapeout and fabrication of hundreds of open-source ICs through Tiny Tapeout. We applaud these initiatives: Giving **open, NDA-free access** to **mature technology nodes** is in our view the perfect way to remove the last remaining technical and legal obstacles to open-source silicon fabrication.

However, even the Open PDKs still require professional support, as the process of completing a design that can be reliably manufactured requires skill and experience, and in some instances the OpenPDKs still do not contain the same level of information that is available in the closed PDKs. For this reason companies, such as [Efabless](https://efabless.com/), have been founded to provide a vital service, acting as an intermediary, a broker, between the open source hardware community and the foundries providing the technologies, ensuring that designs could be manufactured reliably. Unfortunately, the US-based startup Efabless went out of business abruptly, leaving a momentary gap in this much needed service. More importantly, this event demonstrates the **urgency of supporting the development of multiple open PDKs**, as well as **funding service centers** for managing and brokering IC manufacturing based on open PDKs  in Europe: resiliency and sovereignty on the entire path to silicon is essential for the EU to finalize the process of silicon democratization!

We therefore *strongly* recommend **two short-term actions** aiming at democratizing silicon access, growing the community of European students and practitioners with tape-out experience from hundreds to thousands:

- **Fund entities** that create and maintain open source PDKs on mature nodes, ideally cooperating with large scale commercial foundries (for example with proxy PDKs) and provide brokerage service for open-source silicon fabrication access. 
- **Make free open source chip fabrication possible for every student in Europe** through public funding for several runs of chip production. Access to these publicly funded runs could be organized through competitions, hackathons and similar activities aimed at increasing the size of the IC design community, enabling not only large universities, but also smaller educational institutions, and even individuals to access silicon manufacturing.

With those two actions we expect a significant impact on further talent development and the European chip design community.

Thank you for your consideration.

Sincerely,
the signatories

<a class="button" href="https://forms.gle/KmGccDJgLCXnoHUy9">Sign (please note: delay until added below)</a>

*(responsible authors: Stefan Wallentowitz, Frank K. Gürkaynak, Luca Benini; supported by [FOSSi Foundation](https://fossi-foundation.org))*

### Signatories ({{ site.data.signatories.size }})

{% assign signatories = site.data.signatories %}
{% for sign in signatories %}
**{{ sign.name }}** - <i>{{ sign.affiliation }} - {{ sign.country }}</i>
{% endfor %}

