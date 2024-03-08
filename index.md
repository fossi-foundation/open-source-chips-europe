---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: page
---

# Importance of Open-Source EDA Tools for Academia

## Open Letter on European Strategic and Funding Directions

**To Whom It May Concern**

*March 8, 2024*

The recent semiconductor shortage and shifts in global political relations have changed the European roadmap on semiconductors and chip design significantly. A mix of incentives for new fabrication facilities for advanced technologies and the ambitious goals to (re)-build leading-edge chip design capabilities in Europe are key cornerstones of the European Chips Act. Under this impulse, various funding actions have been successfully launched, for instance in the area of the creation of IP based on the RISC-V instruction set.

Universities have to be an integral part of Europe’s ambitions and are heavily involved in research activities on various levels. This is crucial for two reasons: First, they are incubators of innovative ideas. Second, and equally important, they are of key importance to educating future generations of chip designers and related jobs. The high demand for an increased workforce can only be satisfied with tight coordination and the best support of universities. In these efforts, we believe that open source is a key success factor. The availability of open-source RISC-V IPs developed in Europe has, for example, been of seminal importance for a significant ramp-up of research activities and the rapid build-up of a vibrant research community and innovation ecosystem around RISC-V hardware and software. This has led to new groups getting involved with computer architecture and an increase in innovative research that is currently funded to get commercialized at higher technology readiness levels.

A key next step is to turn innovation in computer architecture for the European market into chip designs that utilize the fabrication facilities and skilled workers that create those designs. In this trajectory, it is our strong belief that **open-source chip design tools (Electronic Design Automation -EDA- tools) are essential for the European renaissance in chip design education and innovation**:

1. Open-source EDA tools lower the barrier of entry significantly for students and researchers willing to engage in chip design.  As such, we believe that early initiatives based on open-source EDA have already driven a significant amount of fresh talent into the semiconductor community. In addition to the current university-focused EUROPRACTICE program for access to proprietary tools and closed process design kits (PDKs), open-source EDA tools and PDKs are a great complementary offer, as they can be offered for free and under very liberal licensing terms.
1. Open-source EDA tools allow researchers and designers to collaborate easily, without the complexities and delays of three-way NDAs or similar legal agreements. Researchers and collaborators can easily share designs, ideas, and materials. This makes it much easier to engage new people from diverse fields like computer science, where open-source development is often the norm.
1. Open-source EDA tools are, for themselves, interesting for innovations, research, and development. They allow educators to let students inspect hands-on the functionality of various steps in the design automation process. Students and researchers can change the code, explore their own ideas, and gain a more profound understanding of the inner workings of a chip design process. The knowledge gained by these people will be extremely valuable for increasing Europe’s footprint in the commercial EDA ecosystem.

Based on the considerations above, we would like to express a strong recommendation to the European and national funding agencies:

1. Open-source EDA tools must be a first-class citizen of the ambitions to foster chip design capabilities in Europe. A focus on proprietary EDA tools alone is not sufficient when the goal is to democratize chip design in Europe.
1. Open-source EDA tools are often suited to be complementary to proprietary tools, but design platforms that focus on open-source EDA are an important goal. We value the products of proprietary EDA tool vendors for bleeding-edge chip designs (which are frequently not the focus of education and academic research). Choice and independent design platforms, commercial and alternatively open source, are indispensable.
1. Funding agencies should identify gaps in the open-source EDA tool chain and support the community in closing those gaps and further developing the open-source tools. End-to-end design flows based on open-source EDA tools must be available and will ensure a very low entrance barrier to newcomers.

We thank you in advance for considering our input. We are at your availability for a more in-depth discussion on this topic.

Sincerely,

### Initial Signatories

<div class="container">
{% for sign in site.data.initial %}
<div class="initial" markdown="1">
**{{ sign.name }}**

{{ sign.affiliation }}

*{{ sign.fame }}*
</div>
{% endfor %}
</div>

### Signatories ({{ site.data.signatories.size }})

*We kindly ask educators and researchers from European academic institutions to
co-sign this open letter. To co-sign, please send a mail from your university
mailing address to
[stefan.wallentowitz@hm.edu](mailto:stefan.wallentowitz@hm.edu) and include your
affiliation and ideally include a link to your profile.*

<div class="container">
{% assign signatories = site.data.signatories | sort: "name" %}
{% for sign in signatories %}
<div class="signatory" markdown="1">
**{{ sign.name }}**

{{ sign.affiliation }}
</div>
{% endfor %}
</div>

<div id ="map" style = "width:800px; height:600px;"></div>

 <script src="https://unpkg.com/leaflet@1.9.4/dist/leaflet.js"
     integrity="sha256-20nQCchB9co0qIjJZRGuk2/Z9VM+kNiyxNV1lvTlZBo="
     crossorigin=""></script>
<script>
    // Creating map options
    var mapOptions = {
    center: [52.2657, 10.5227],
    zoom: 4,
    zoomControl: false,
    doubleClickZoom: false,
    boxZoom: false,
    scrollWheelZoom: false,
    keyboard: false,
    dragging: false
    }
    
    // Creating a map object
    var map = new L.map('map', mapOptions);
    
    // Creating a Layer object
    var layer = new L.TileLayer('https://{s}.tile.openstreetmap.org/{z}/{x}/{y}.png');
    
    // Adding layer to the map
    map.addLayer(layer);

{% for sign in site.data.initial %}
    {% if sign.map %}
    L.marker({{ sign.map}}).addTo(map)
    {% endif %}
{% endfor %}
{% for sign in site.data.signatories %}
    {% if sign.map %}
    L.marker({{ sign.map}}).addTo(map)
    {% endif %}
{% endfor %}
</script>