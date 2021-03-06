People say, while a data scientist needs broad knowledge and skills, also needs deep knowledge in 1 area. 3 or 4 years later, when I look back, am I going to be able to say that, I am expertizing in Security Data Science? 


******************************************************

News and Notes

* <b>Google Project Zero</b> - they update newly founded attacks: https://googleprojectzero.blogspot.ca/
* 4 trends in Security data Science for 2017: https://www.oreilly.com/ideas/4-trends-in-security-data-science-for-2017?imm_mid=0ec217&cmp=em-data-na-na-newsltr_20170111
 * Adversarial Machine Learning looks very interesting to me, and here is more: http://www.kdnuggets.com/2015/07/deep-learning-adversarial-examples-misconceptions.html
 * Neural Network for unsupervised learning looks also interesting and here is details for Autoencoders: http://ufldl.stanford.edu/tutorial/unsupervised/Autoencoders/
* NuData Security Selected as Excellence Award: https://www.linkedin.com/pulse/nudata-security-selected-excellence-award-threat-sc-lisa-baergen-apr
* The Papers from NuData Security are really good: https://nudatasecurity.com/papers/

* Collection of Biometrics
  * Fingerprints breach: http://findbiometrics.com/opm-hack-5-6-million-fingerprints-29233/
  * GOOLIGAN Attack, call for non-traditional security detection methods: http://www.biocatch.com/blog/android-malware-compromises-google-accounts
  * Some BioMetrics mentioned by BioCatch: https://github.com/hanhanwu/Hanhan_Data_Science_Resources2/blob/master/BioCatch_WP_PREVENTING_FRAUD_IN_MOBILE_ERA.pdf
  * Biometrics Report (2017) from Aite Group: https://github.com/hanhanwu/Hanhan_Data_Science_Resources2/blob/master/Aite-Group_Biometrics_Report_NDS_2017.pdf
    * I really like this system/platform design recommended in this report. 
    * A layer of technology that can integrate various types of authentication and serve them based on risk, channel, and consumer preference.
    * Each individual flow may function reasonably well on its own. 
    * Multiple types of authentication can be deployed based on risk, cost, and customer preference and can be optimized by channel. It can also help enable a smooth multichannel experience for customers when they need to move from a self-service to an assisted channel
    * Authentication methods can be added, removed, and combined, and business logic for authentication can be consolidated and coordinated, and can evolve over time. With consistent integration and communication standards can lower costs and improve time to market when adding new authentication options and managing those in place.
  * Page 15, Physical BioMetrics: https://nudatasecurity.com/wp-content/uploads/2017/06/E-Book-The-Next-Evolution-of-Authentication-NuData-Security.pdf?utm_source=NuData+Security+Opt-in&utm_campaign=78cfccd098-Newsletter_June2017&utm_medium=email&utm_term=0_d94819affe-78cfccd098-218614237


* Collections of Attacks
  * 7 most commen RATs (remote access Trojans): http://www.darkreading.com/perimeter/the-7-most-common-rats-in-use-today-/a/d-id/1321965
  * Click Farm
    * http://vesselnews.io/look-inside-chinese-click-farm-fake-followers-fake-likes-fake-reviews/
    * http://m.essexlive.news/watch-how-these-bizarre-click-farms-in-china-are-able-to-offer-fake-social-media-likes-and-reviews/story-30352810-detail/story.html


******************************************************

How Others Do Security

MICROSOFT
* Azure Network Security: https://azure.microsoft.com/en-us/blog/azure-network-security/
* MSFT Cyber Security Blog: https://blogs.microsoft.com/microsoftsecure/category/cybersecurity/
* MSFT Security: https://www.microsoft.com/en-us/security/default.aspx
* BioCatch is working with Azure for their analysis now
* Azure Security Center (ASC) and Cyber Security (these in fact are interesting)
  * First of all, ASC added alerts to help threat investigation
    * https://azure.microsoft.com/en-us/blog/azure-security-center-adds-context-alerts-to-aid-threat-investigation/
    * It seems that, the basic steps is to check system data, including the time order of system events (any abnormal order, any abnormal event, etc); objects being created/downloaded/launched/etc.
    * Created scheduled task can also be suspective, since many attacks will schedule to happen repeatedly
  * Here is a very detailed SQL Brute Force Attack investigation process and prevention solution
    * https://azure.microsoft.com/en-us/blog/how-azure-security-center-helps-reveal-a-cyberattack/
    * It seems that their auto detection methods include not only machine learning methods, but also implemented investication process that is same as human investigation process
    * This is a very interesting article!
  * How ASC detects Bitcoin Mining Attack
    * https://azure.microsoft.com/en-us/blog/how-azure-security-center-detects-a-bitcoin-mining-attack/
    * <b>Bitcoin Miners</b> are a special class of software that use mining algorithms to generate or “mine” bitcoins, which are a form of digital currency. Mining software is often flagged as malicious because <b>it hijacks</b> system hardware resources like the Central Processing Unit (<b>CPU</b>) or Graphics Processing Unit (<b>GPU</b>) as well as <b>network bandwidth of an affected host</b>. Cryptonight is one such mining algorithm which relies specifically on the host’s CPU. 
    * In their investigations, they’ve seen bitcoin miners installed through a variety of techniques including <b>malicious downloads, emails with malicious links, attachments downloaded by already-installed malware, peer to peer file sharing networks, and through cracked installers/bundlers</b>.
* White Papers from Hexadite
  * When I was running the code, I checked cyber security news and saw this company has been bought by Microsoft recently. Out of curiosity, I started to check this company, and it does write pretty good white papers. I especially like the process it explains to you about how security analyst work and how intelligent security automation work in the same way but at machine speed
  * Security Automation Details (process, what to check, which vendor to use in different sitations, etc.): https://github.com/hanhanwu/Hanhan_Data_Science_Resources2/blob/master/What%20is%20Security%20Automation%20Whitepaper%20RC2.pdf
  * Alert Fatigue (like that real life example - Target 2013): https://github.com/hanhanwu/Hanhan_Data_Science_Resources2/blob/master/alert-fatigue-best-1.pdf


******************************************************

Data Science Applications 

Spam Detection
* SpamBayes is a tool to detect spams, it uses machine learning methods: http://spambayes.sourceforge.net/
* In this paper, it indicates the attacks that SpamBayes may not be able to find, Exploiting machine learning to subvert your spam filter: https://people.eecs.berkeley.edu/~tygar/papers/SML/Spam_filter.pdf


******************************************************

Simple Ideas Spark

* AI in Banking:https://www.analyticsvidhya.com/blog/2017/04/5-ai-applications-in-banking-to-look-out-for-in-next-5-years/?utm_source=feedburner&utm_medium=email&utm_campaign=Feed%3A+AnalyticsVidhya+%28Analytics+Vidhya%29
  * Most of these are not new to people, but it makes me think whether bots can be used to encourage more biometrics input and to collect more biometrics?
  
* Unsupervised learnining - Association Rules
  * Related behaviours - When detecting biometrics, would association rules related algorithms help? Because some behaviors are linked together. Meanwhile, the order of these behaviours are also important.
  * Predict behaviours - would a behaviour can be predicted based on the previous behaviour series, or order series?
  
* Unsupervised learning - PCA and Sparse PCA in shape data
  * Some biometrics can be shape data, such as sighed images. PCA is a popular tool applied to <b>shape data</b>, sometimes Sparsed PCA is more informative and saves reousrces than Standard PCA.
  * When preprocessing images, it is better to Align the predict target in the same position in the image. Scale or crop all images to the same size.
  * NOTE: if want to use neural network for image processing, <b>Convolutional Neural Network</b> would be better suited for image related problems because of its inherent nature for taking into account changes in nearby locations of an image


******************************************************

Research Papers

<b>Offense and Defense</b>

* Finding Vulnerabilities
 * [Driller: Augmenting Fuzzing Through Selective Symbolic Execution][1]
 

******************************************************

SFU Cyber Security Seminar

* [2017-1-24] Privacy as a Service
 * They created 3 cloud service protection to deal with powerful threats in Cloud, Networks and clients end
 * [uProxy, for Network][2]
 * [Radiatus, for Clients end][3]
 * Talek, deals with utrusted cloud
 
* [2017-1-25] Securing the Internet Routing Infrastructure
 * Routing prototypes glue the Internet communiation
 * BGP is an important protocol used to route between the network (intern network routing), but BGP is a distributed algorithm, which means routing decisions are the results made by all "peers", what if there is a mistake or attack, things can be a disaster.
 * Their project is to check whether routers are ok and try to analysis whether there is hijack attack. Checking routers are very complex, so they developed a structure called "Pop" which is a connection of of routers and other networking devices in a campus of that certain region.
 * With PoP, they built the GeoIP database, created PopGeo embeding and PoP Map
 * Their solution is important because, they cannot always expect thr router or data encryption could solve the problem, since encrypted data has just been proved that it is breakable
 * [Their solution][4]
 
 
[1]: https://github.com/hanhanwu/Hanhan_Data_Science_Resources2/blob/master/2016_NDSS_Driller.pdf
[2]: https://github.com/uProxy/uproxy
[3]: https://www.cs.washington.edu/education/grad/UW-CSE-13-11-01.PDF
[4]: http://www.bgprotect.com/
