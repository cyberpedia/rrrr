# Social Media Mining for Open-Source Intelligence (OSINT) in Cyber Threat Detection

## Introduction

Open-Source Intelligence (OSINT) leverages publicly available data to enhance cyber threat detection and situational awareness. Social media mining—extracting actionable intelligence from social networks—has become crucial for identifying vulnerabilities, threat actors, and cyber attack patterns. This report provides a structured review of key tools, including Shodan, Maltego, Gephi, and similar platforms, focusing on their capabilities, use cases, advantages, disadvantages, pricing models, and applicability to cyber defense.

---

## 1. Tool Overview

### 1.1 Shodan

**Description:**  
Shodan is a search engine for internet-connected devices. It indexes information about devices (servers, routers, IoT) via banners, services, and vulnerabilities [[1]](https://www.shodan.io/about).

**Capabilities:**
- Scans the internet for open ports, services, and device metadata [[1]](https://www.shodan.io/about).
- Identifies vulnerable systems using known CVEs [[2]](https://help.shodan.io/the-basics/vulnerability-search.html).
- Provides threat intelligence feeds and real-time alerts [[3]](https://help.shodan.io/enterprise/alerting.html).
- Supports filtering by geography, organization, device type, etc. [[1]](https://www.shodan.io/about).

**Use Cases:**
- Discovering exposed/vulnerable assets [[4]](https://www.shodan.io/explore).
- Tracking IoT device security [[5]](https://www.shodan.io/search?query=iot).
- Mapping external attack surfaces [[6]](https://blog.shodan.io/exposed-internet-assets/).
- Investigating suspicious infrastructure used by threat actors [[7]](https://unit42.paloaltonetworks.com/shodan-cyber-threat-intelligence/).

**Cyber Defense Support:**
- Early warning for exposed assets [[8]](https://www.sans.org/blog/using-shodan-for-defense/).
- Rapid identification of misconfigurations [[9]](https://www.csoonline.com/article/3434751/how-to-use-shodan-to-discover-vulnerable-devices.html).
- Supports vulnerability management and incident response [[10]](https://www.recordedfuture.com/shodan-security-intelligence).

**Pricing:**
- **Free:** Limited search and filters [[11]](https://account.shodan.io/register).
- **Membership ($59/month, $299/year):** Increased query limits, advanced filters, and premium features [[12]](https://www.shodan.io/store/member).
- **Enterprise (custom pricing):** API access, full datasets, and organizational features [[13]](https://www.shodan.io/enterprise).
- **Advantages:**  
  - Pay-as-you-grow model, suitable for individuals and enterprises.
  - Free tier supports basic research and testing.
  - API access enables automation and integration into SOC workflows.
  - Global, real-time visibility into internet-exposed assets.
- **Disadvantages:**  
  - Limited depth: Only sees what is exposed to the public internet.
  - May generate false positives due to banner misidentification [[14]](https://www.sans.org/blog/using-shodan-for-defense/).
  - Premium features and API access can be costly for smaller organizations.
  - Data freshness may vary; scans are periodic, not continuous [[15]](https://www.shodan.io/api).
  - Use may raise compliance/privacy concerns for some organizations [[16]](https://www.ncsc.gov.uk/collection/top-tips-for-staying-secure-online/shodan).

---

### 1.2 Maltego

**Description:**  
Maltego is a visual link analysis tool for mapping relationships between entities (people, domains, IPs, social media accounts) [[17]](https://www.maltego.com/solutions/cyber-threat-intelligence/).

**Capabilities:**
- Aggregates data from open sources, social media, DNS, WHOIS, and more [[18]](https://docs.maltego.com/support/solutions/articles/15000019111-what-is-a-transform-).
- Visualizes complex relationships (graphs/networks) [[19]](https://www.maltego.com/solutions/link-analysis-software/).
- Supports OSINT through “Transforms”—automated data-enrichment modules [[20]](https://www.maltego.com/transform-hub/).
- Integrates with third-party data providers [[21]](https://www.maltego.com/partners/).

**Use Cases:**
- Mapping threat actor infrastructure (C2 servers, associated domains) [[22]](https://www.maltego.com/solutions/threat-investigations/).
- Uncovering social networks of threat actors or insiders [[23]](https://www.maltego.com/solutions/insider-threat-detection/).
- Investigating phishing campaigns and email spoofing [[24]](https://www.maltego.com/blog/analyzing-phishing-campaigns-using-maltego/).
- Profiling potential targets and their online footprint [[25]](https://www.maltego.com/solutions/social-engineering/).

**Cyber Defense Support:**
- Enables threat actor attribution [[26]](https://www.maltego.com/solutions/threat-actor-attribution/).
- Supports risk assessments and digital footprint analysis [[27]](https://www.maltego.com/solutions/digital-footprint/).
- Useful for fraud detection, insider threat analysis, and incident investigations [[28]](https://www.maltego.com/solutions/fraud-detection/).

**Pricing:**
- **Community Edition (Free):** Limited features, graph size, and transforms [[29]](https://www.maltego.com/downloads/).
- **Maltego Pro ($999/year):** Full graphing, automation, and premium transforms [[30]](https://www.maltego.com/pricing/).
- **Enterprise (custom pricing):** Multi-user features, on-prem deployments, advanced integrations [[30]](https://www.maltego.com/pricing/).

**Advantages:**  
- Free tier for students, researchers, and initial exploration.
- Professional/Enterprise tiers justify pricing with advanced analytics, collaboration, and automation.
- Powerful data enrichment and visualization for complex investigations.
- Wide range of integration options with external data sources.
**Disadvantages:**  
- Steep learning curve for advanced analysis [[31]](https://www.peerspot.com/products/maltego-pro-reviews).
- Free version is limited in scale and capability.
- Pro/Enterprise versions are expensive for small teams or individuals.
- Transform quality varies and some integrations require separate licenses [[32]](https://www.peerspot.com/products/maltego-pro-reviews).
- May generate information overload without careful scoping.

---

### 1.3 Gephi

**Description:**  
Gephi is an open-source network visualization and analysis software, popular for social network analysis [[33]](https://gephi.org/features/).

**Capabilities:**
- Import and visualize large network datasets [[34]](https://gephi.org/users/).
- Analyze communities, clusters, and central nodes (influencers) [[35]](https://gephi.org/features/).
- Supports dynamic/temporal graph analysis [[36]](https://gephi.org/features/).
- Extensible via plugins for custom data import and metrics [[37]](https://marketplace.gephi.org/).

**Use Cases:**
- Analyzing social media networks for influence operations [[38]](https://gephi.org/users/).
- Identifying key nodes in cyber threat actor networks [[39]](https://www.peerspot.com/products/gephi-reviews).
- Visualizing relationships between malware samples, domains, and IPs [[40]](https://www.peerspot.com/products/gephi-reviews).
- Supporting law enforcement or threat intelligence investigations [[41]](https://www.researchgate.net/publication/312724169_A_Network_Analysis_Tool_for_Open_Source_Intelligence_OSINT).

**Cyber Defense Support:**
- Helps uncover hidden relationships in threat actor infrastructure [[42]](https://www.sciencedirect.com/science/article/pii/S1877050919316345).
- Supports pattern analysis in attack campaigns [[43]](https://gephi.org/features/).
- Assists in mapping propagation of malicious content.

**Pricing:**
- **Free/Open Source.** [[33]](https://gephi.org/)

**Advantages:**  
- No cost, suitable for academic, research, and operational use.
- Highly extensible and scriptable [[37]](https://marketplace.gephi.org/).
- Cost-effective for organizations with technical expertise.
- Handles large, complex network data sets.
**Disadvantages:**  
- Lacks built-in data collection; requires external data preparation [[44]](https://www.peerspot.com/products/gephi-reviews).
- No direct integrations with OSINT data sources.
- Steep learning curve for non-technical users.
- Limited support and documentation compared to commercial tools.
- Not tailored specifically for cyber threat intelligence.

---

### 1.4 Similar Platforms

| Tool         | Description                                      | Pricing             | Key Advantages                                           | Key Disadvantages                                         | Reference |
|--------------|--------------------------------------------------|---------------------|---------------------------------------------------------|-----------------------------------------------------------|-----------|
| SpiderFoot   | Automated OSINT tool for threat surface mapping  | Free/Open Source, $149/year (Cloud) | Automation, extensibility, self-hosted option           | Cloud version limited; on-prem setup can be complex        | [[45]](https://www.spiderfoot.net/) |
| OSINT Framework | Curated resource directory for OSINT         | Free                | Comprehensive starting point for OSINT investigations   | Only a directory—no automation or analytics                | [[46]](https://osintframework.com/) |
| Paliscope    | OSINT investigation platform                    | Starts ~$1,000/year | Workflow automation, reporting, enterprise features     | Expensive, closed-source, steeper learning curve           | [[47]](https://www.paliscope.com/) |
| Social-Searcher | Social media search and monitoring            | Free, $9.49+/month  | Real-time monitoring, multi-platform coverage           | Limited analytics, restrictions on free/cheaper tiers      | [[48]](https://www.social-searcher.com/) |

---
### 1.4 Similar Platforms (Detailed)

#### SpiderFoot

**Description:**  
SpiderFoot is an automated OSINT reconnaissance tool that performs extensive intelligence gathering about IPs, domains, emails, usernames, and more [[45]](https://www.spiderfoot.net/). It integrates with numerous open-source and commercial data sources, and can be run as a web application or command line tool.

**Capabilities:**
- Automated collection of OSINT from 200+ sources, including social media, threat intelligence feeds, and public datasets.
- Discovery of associated domains, subdomains, emails, usernames, IP addresses, data leaks, breaches, and more.
- Integration with APIs for data enrichment (Shodan, VirusTotal, HaveIBeenPwned, etc.).
- Flexible scanning modules and custom automation workflows.
- Web-based UI for visualization, exploration, and reporting.
- Self-hosted and cloud-based deployment options.

**Use Cases:**
- Mapping an organization’s external threat surface.
- Collecting intelligence on threat actors via usernames, emails, and social media.
- Identifying exposed credentials and data breaches.
- Automating discovery of infrastructure assets for red/blue team exercises.
- Enriching incident response with context on indicators.

**Cyber Defense Support:**
- Increases speed and automation of OSINT collection for security teams.
- Highlights unknown assets and exposures.
- Supports threat hunting, vulnerability management, and adversary tracking.

**Pricing:**
- **Free/Open Source (self-hosted):** Full feature set, unlimited scans, open code.
- **Cloud ($149/year and up):** Hosted, managed, includes premium modules and API credits.

**Advantages:**
- Highly automated, scalable, and scriptable.
- Self-hosting for privacy and customizability.
- Wide integration with OSINT sources.

**Disadvantages:**
- Cloud version limits heavy usage unless higher tiers purchased.
- Some integrations require separate API keys or paid services.
- Initial configuration and self-hosting can be complex for beginners.

---

#### OSINT Framework

**Description:**  
OSINT Framework is not a tool, but a curated directory of online resources for open-source intelligence investigations [[46]](https://osintframework.com/). It organizes links to hundreds of OSINT tools, search engines, and data sources into a hierarchical, easy-to-navigate structure.

**Capabilities:**
- Comprehensive directory of categorized OSINT resources for social media, people, usernames, domains, IPs, dark web, and more.
- Continuously updated and community-driven.
- Serves as a launchpad for focused OSINT activities.

**Use Cases:**
- Quickly finding specialized OSINT tools or databases relevant to a specific investigation.
- Guiding beginners and professionals through available OSINT options.
- Building custom OSINT workflows by selecting relevant resources.

**Cyber Defense Support:**
- Accelerates tool discovery and research for security teams.
- Helps investigators find niche or emerging OSINT resources.

**Pricing:**
- **Free.** Entirely web-based and open to all users.

**Advantages:**
- No cost, no registration required.
- Extremely comprehensive and regularly updated.
- Simple interface for rapid navigation.

**Disadvantages:**
- Does not perform analysis, automation, or data collection itself.
- Resource links may occasionally become outdated or broken.
- No built-in reporting, analytics, or integration features.

---

#### Paliscope

**Description:**  
Paliscope is a commercial OSINT investigation platform designed for law enforcement, enterprise, and cyber security professionals [[47]](https://www.paliscope.com/). It provides end-to-end workflows for online investigations, including data collection, analysis, visualization, and reporting.

**Capabilities:**
- Automated and manual data collection from social media, forums, dark web, and open sources.
- Advanced link analysis, timeline construction, and mapping.
- Case management features: evidence storage, annotation, collaboration, and chain-of-custody.
- Integrations with Maltego, i2 Analyst’s Notebook, and third-party data providers.
- Automated reporting and export for legal proceedings.

**Use Cases:**
- Investigating cybercrime, fraud, and organized crime.
- Profiling threat actors and mapping their online presence.
- Collecting and preserving social media evidence.
- Supporting law enforcement or corporate investigations.

**Cyber Defense Support:**
- Enables deep-dive investigations into threat actors, phishing, and fraud.
- Supports cross-team and multi-case management for SOCs and fusion centers.

**Pricing:**
- **Commercial, starts at ~$1,000/year per user (varies by features and deployment).**
- Free trials and custom enterprise packages available on request.

**Advantages:**
- Full investigation lifecycle support in one platform.
- Robust reporting, collaboration, and chain-of-custody features.
- Integration with other analysis tools.

**Disadvantages:**
- Costly compared to open-source alternatives.
- Closed source; less customizable than open tools.
- Learning curve for advanced features.

---

#### Social-Searcher

**Description:**  
Social-Searcher is an online platform for searching and monitoring social media content across multiple platforms in real-time [[48]](https://www.social-searcher.com/). It provides both free and paid services for keyword-based social media search, analytics, and alerting.

**Capabilities:**
- Real-time search of posts, mentions, and hashtags from sources like Twitter, Facebook, Instagram, YouTube, TikTok, Reddit, and more.
- Sentiment analysis, keyword trends, and user analytics.
- Alerts for new mentions or relevant posts.
- Export of search results to CSV, RSS, and other formats.
- API access for integration and automation (premium).

**Use Cases:**
- Monitoring for mentions of brands, organizations, or key terms.
- Detecting social engineering campaigns, phishing, or brand impersonation.
- Gathering intelligence on threat actor chatter and emerging threats.
- Supporting incident response with real-time social media monitoring.

**Cyber Defense Support:**
- Early warning for social media-based phishing or scam campaigns.
- Brand and executive protection monitoring.
- Provides context for social engineering and information operations.

**Pricing:**
- **Free:** Limited daily searches and restricted analytics.
- **Premium ($9.49/month and up):** More searches, advanced analytics, and API.

**Advantages:**
- Rapid, multi-platform social media monitoring.
- Easy to use and accessible via web interface.
- Affordable for small teams or individuals.

**Disadvantages:**
- Analytics and data retention limited on free tier.
- Some platforms (e.g., Facebook, Instagram) limited by API access policies.
- Not purpose-built for cyber threat intelligence—focuses on social monitoring.

---

## 2. Applicability to Cyber Threat Detection

### 2.1 Identifying Vulnerabilities
- **Shodan**: Finds exposed endpoints and devices with known vulnerabilities (CVE-based) [[2]](https://help.shodan.io/the-basics/vulnerability-search.html).
- **Maltego**: Maps infrastructure and relationships to uncover associated vulnerabilities [[22]](https://www.maltego.com/solutions/threat-investigations/).
- **Gephi**: Visualizes links between assets and vulnerable nodes [[39]](https://www.peerspot.com/products/gephi-reviews).
- **SpiderFoot**: Automated scanning for exposed services, vulnerabilities, and leaks.
- **Paliscope**: Supports vulnerability and threat actor investigations via multi-source data collection.
- **Social-Searcher**: Detects public discussion of vulnerabilities and exploits.
- **OSINT Framework**: Directory for discovering specialized vulnerability and exposure search tools.

### 2.2 Identifying Threat Actors
- **Maltego**: Correlates social media, domain, and email data to build threat actor profiles [[26]](https://www.maltego.com/solutions/threat-actor-attribution/).
- **Gephi**: Reveals key influencers or nodes in cybercriminal networks [[39]](https://www.peerspot.com/products/gephi-reviews).
- **SpiderFoot**: Automates collection and enrichment of threat actor indicators [[45]](https://www.spiderfoot.net/).
- **Paliscope**: Advanced profiling and case management capabilities for threat actors.
- **Social-Searcher**: Monitors social media for threat actor communication or impersonation.
- **Shodan**: Infrastructure mapping sometimes assists in actor attribution.
- **OSINT Framework**: Resource hub for actor identification techniques and tools.

### 2.3 Discovering Cyber Attack Patterns
- **Gephi**: Detects clusters and attack propagation paths [[42]](https://www.sciencedirect.com/science/article/pii/S1877050919316345).
- **Maltego**: Maps relationships between incidents, infrastructure, and actors [[22]](https://www.maltego.com/solutions/threat-investigations/).
- **Shodan**: Identifies attack trends based on device/service exposures [[8]](https://www.sans.org/blog/using-shodan-for-defense/).
- **SpiderFoot**: Aggregates incident indicators to reveal larger attack patterns.
- **Paliscope**: Timeline and event analysis for tracking cyber attacks.
- **Social-Searcher**: Detects emerging campaigns or trends via social chatter.
- **OSINT Framework**: Catalogs tools for pattern analysis and campaign tracking.

---
## 3. Summary Table

| Tool      | Key Capabilities          | Use Cases                       | Pricing                | Advantages                 | Disadvantages            | Reference |
|-----------|--------------------------|----------------------------------|------------------------|----------------------------|--------------------------|-----------|
| Shodan    | Device/service search, CVE mapping, alerting | Attack surface mapping, vulnerability discovery | Free, $59/mo+, Enterprise | Real-time, API, global coverage | Limited depth, possible false positives, cost for API, privacy concerns | [[1]](https://www.shodan.io/) |
| Maltego   | Graph analysis, data enrichment, entity linking | Threat actor profiling, infrastructure analysis | Free, $999/yr+, Enterprise | Visual analysis, transforms, integrations | Expensive, learning curve, info overload, transform costs | [[17]](https://www.maltego.com/) |
| Gephi     | Large-scale network visualization/analysis | Social network and incident mapping | Free (Open Source)     | Extensible, cost-effective | Data prep required, no OSINT integrations, learning curve | [[33]](https://gephi.org/) |
| SpiderFoot| Automated OSINT, threat mapping | Asset discovery, intelligence automation | Free, $149/yr (Cloud)  | Self-hosted, automated     | Cloud feature limits, complex setup | [[45]](https://www.spiderfoot.net/) |


| Tool         | Key Capabilities                                                                 | Use Cases                                    | Pricing                         | Advantages                                     | Disadvantages                                   | Reference |

| SpiderFoot   | Automated OSINT, 200+ sources, enrichment, self-hosted/cloud, API                | Threat surface mapping, asset discovery      | Free, $149/yr (Cloud)           | Automated, extensible, privacy via self-hosting | Cloud limits, setup complexity                  | [[45]](https://www.spiderfoot.net/) |
| OSINT Framework | Curated OSINT resource directory, topical navigation                         | Tool discovery, workflow building            | Free                            | Comprehensive, easy to use, updated             | No automation, only links                       | [[46]](https://osintframework.com/) |
| Paliscope    | Automated/manual collection, link analysis, case management, reporting           | Cybercrime, fraud, threat actor investigations | ~$1,000/yr per user (varies)   | Full investigation workflow, reporting, collaboration | Expensive, closed-source, learning curve         | [[47]](https://www.paliscope.com/) |
| Social-Searcher | Multi-platform real-time social search, sentiment, alerts, analytics         | Brand protection, phishing, social monitoring | Free, $9.49/mo+ (Premium)      | Easy, affordable, real-time monitoring          | Free tier limited, some API/platform restrictions | [[48]](https://www.social-searcher.com/) |

---
## 3. Comprehensive Summary Table

| Tool             | Key Capabilities                                                                | Use Cases                                     | Pricing                          | Advantages                                       | Disadvantages                                      | Reference                               |
|------------------|--------------------------------------------------------------------------------|-----------------------------------------------|-----------------------------------|--------------------------------------------------|----------------------------------------------------|------------------------------------------|
| **Shodan**       | Search for internet-connected devices, ports, banners, CVE mapping, alerts, API | Attack surface mapping, vulnerability discovery| Free, $59/mo+, custom Enterprise | Real-time, global, API, integrates with many tools| Limited depth, false positives, cost, privacy      | [1](https://www.shodan.io/)             |
| **Maltego**      | Visual link analysis, transforms, graphing, data enrichment, integrations       | Threat actor profiling, infra mapping, OSINT   | Free CE, $999/yr+ Pro/Enterprise | Deep analysis, rich visuals, extensible           | Expensive, learning curve, info overload           | [17](https://www.maltego.com/)          |
| **Gephi**        | Open-source network visualization and analysis, plugins, large data handling    | Social/infra network analysis, campaign mapping| Free (Open Source)               | Cost-effective, extensible, large network support | Data prep needed, no direct OSINT, learning curve  | [33](https://gephi.org/)                |
| **SpiderFoot**   | Automated OSINT, 200+ data sources, enrichment, self-hosted/cloud, API          | Threat surface mapping, asset discovery        | Free (self-hosted), $149/yr+ Cloud| Automated, extensible, privacy via self-hosting   | Cloud limits, setup/config complexity              | [45](https://www.spiderfoot.net/)       |
| **OSINT Framework** | Curated directory of OSINT tools, categorized navigation                     | Tool/resource discovery, workflow building     | Free                             | Comprehensive, easy to use, regularly updated     | No automation, only external links                 | [46](https://osintframework.com/)       |
| **Paliscope**    | Automated/manual collection, link analysis, case management, reporting          | Cybercrime, fraud, threat actor investigations | ~$1,000/yr/user+ (varies)        | Full investigation workflow, robust reporting     | Expensive, closed-source, learning curve           | [47](https://www.paliscope.com/)        |
| **Social-Searcher** | Multi-platform real-time social search, sentiment, alerts, analytics         | Brand protection, phishing, social monitoring  | Free, $9.49/mo+ Premium          | Easy, affordable, real-time, multi-platform       | Free tier limited, API/plat. restrictions, basic   | [48](https://www.social-searcher.com/)  |

---

## 4. Conclusion

Social media mining, via open-source tools like Shodan, Maltego, and Gephi, significantly enhances cyber threat detection by:
- Identifying exposed and vulnerable assets.
- Profiling threat actors and their networks.
- Revealing cyber attack patterns and propagation paths.
- Supporting proactive defense, incident response, and strategic intelligence.

**However, challenges remain:**
- Cost and complexity can be significant for organizations with limited resources.
- Learning curves and required technical skills are non-trivial.
- Some tools lack integration or automation features.
- Data privacy, compliance, and the risk of false positives must be carefully managed.

Organizations should choose tools based on investigation depth, automation needs, technical capacity, and budget. Free/open-source options provide a low-barrier entry, while paid platforms offer deeper analytics, automation, and enterprise-ready features.

---

## 5. References

1. [Shodan - About](https://www.shodan.io/about)
2. [Shodan - Vulnerability Search](https://help.shodan.io/the-basics/vulnerability-search.html)
3. [Shodan - Alerting](https://help.shodan.io/enterprise/alerting.html)
4. [Shodan - Explore](https://www.shodan.io/explore)
5. [Shodan - IoT Search](https://www.shodan.io/search?query=iot)
6. [Shodan Blog - Exposed Internet Assets](https://blog.shodan.io/exposed-internet-assets/)
7. [Unit42 - Shodan in Threat Intel](https://unit42.paloaltonetworks.com/shodan-cyber-threat-intelligence/)
8. [SANS - Using Shodan for Defense](https://www.sans.org/blog/using-shodan-for-defense/)
9. [CSO Online - Vulnerable Devices with Shodan](https://www.csoonline.com/article/3434751/how-to-use-shodan-to-discover-vulnerable-devices.html)
10. [Recorded Future - Shodan Security Intelligence](https://www.recordedfuture.com/shodan-security-intelligence)
11. [Shodan - Register](https://account.shodan.io/register)
12. [Shodan - Membership Store](https://www.shodan.io/store/member)
13. [Shodan - Enterprise](https://www.shodan.io/enterprise)
14. [SANS - Shodan False Positives](https://www.sans.org/blog/using-shodan-for-defense/)
15. [Shodan - API](https://www.shodan.io/api)
16. [NCSC UK - Shodan](https://www.ncsc.gov.uk/collection/top-tips-for-staying-secure-online/shodan)
17. [Maltego - Cyber Threat Intelligence](https://www.maltego.com/solutions/cyber-threat-intelligence/)
18. [Maltego Docs - What is a Transform](https://docs.maltego.com/support/solutions/articles/15000019111-what-is-a-transform-)
19. [Maltego - Link Analysis Software](https://www.maltego.com/solutions/link-analysis-software/)
20. [Maltego - Transform Hub](https://www.maltego.com/transform-hub/)
21. [Maltego - Partners](https://www.maltego.com/partners/)
22. [Maltego - Threat Investigations](https://www.maltego.com/solutions/threat-investigations/)
23. [Maltego - Insider Threat Detection](https://www.maltego.com/solutions/insider-threat-detection/)
24. [Maltego Blog - Phishing Campaign Analysis](https://www.maltego.com/blog/analyzing-phishing-campaigns-using-maltego/)
25. [Maltego - Social Engineering](https://www.maltego.com/solutions/social-engineering/)
26. [Maltego - Threat Actor Attribution](https://www.maltego.com/solutions/threat-actor-attribution/)
27. [Maltego - Digital Footprint](https://www.maltego.com/solutions/digital-footprint/)
28. [Maltego - Fraud Detection](https://www.maltego.com/solutions/fraud-detection/)
29. [Maltego Download](https://www.maltego.com/downloads/)
30. [Maltego Pricing](https://www.maltego.com/pricing/)
31. [PeerSpot - Maltego Reviews](https://www.peerspot.com/products/maltego-pro-reviews)
32. [PeerSpot - Maltego Transforms](https://www.peerspot.com/products/maltego-pro-reviews)
33. [Gephi - Features](https://gephi.org/features/)
34. [Gephi - Users](https://gephi.org/users/)
35. [Gephi - Features](https://gephi.org/features/)
36. [Gephi - Features](https://gephi.org/features/)
37. [Gephi - Plugins Marketplace](https://marketplace.gephi.org/)
38. [Gephi - Users](https://gephi.org/users/)
39. [PeerSpot - Gephi Reviews](https://www.peerspot.com/products/gephi-reviews)
40. [PeerSpot - Gephi Reviews](https://www.peerspot.com/products/gephi-reviews)
41. [ResearchGate - OSINT Network Analysis Tool](https://www.researchgate.net/publication/312724169_A_Network_Analysis_Tool_for_Open_Source_Intelligence_OSINT)
42. [ScienceDirect - Gephi for OSINT](https://www.sciencedirect.com/science/article/pii/S1877050919316345)
43. [Gephi - Features](https://gephi.org/features/)
44. [PeerSpot - Gephi Data Preparation](https://www.peerspot.com/products/gephi-reviews)
45. [SpiderFoot](https://www.spiderfoot.net/)
46. [OSINT Framework](https://osintframework.com/)
47. [Paliscope](https://www.paliscope.com/)
48. [Social-Searcher](https://www.social-searcher.com/)
