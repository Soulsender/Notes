PART 2. [TOOLING](https://www.reddit.com/r/OSINT/comments/e7a4ke/part_2_tooling/?utm_source=share&utm_medium=ios_app&utm_name=iossmf)

# (OSINT TOOLS)  - LIST AND MORE 

#  ▬▬ι═══════ﺤ 

Assuming you have seen ..

[PART 1. Introduction to Osint](https://www.reddit.com/r/OSINT/comments/e78he1/osint_for_beginners_part_1_introduction/?utm_source=share&utm_medium=web2x)

Part 2 . Tooling <-- you are here

[Part 3. case management and methodology](https://www.reddit.com/r/OSINT/comments/e9276y/osint_guide_part_3_case_management_and_methodology/)

# DISCLAIMER

**- Before going any further, I would be remiss not to mention that while performing OSINT is legal, using the OSINT tools and techniques outlined here are intended to be used in a legal an ethical manner. You have been warned! and again like part 1. This is not my work i have linked all the sources. This is Just what i have learned on my journey in to OSINT hope it helps.**

========----------------=================---------------==========-------

WE are now ready to move on and take a look at some of the tools we use in OS-INT investigation's and how we can use these tools effectively.

There are a plethora of OSINT tools available, some of which are free and others can cost a pretty penny. While it is outside the scope of this chapter to cover every single OSINT tool, we will cover a few of the more popular tools that you may find useful for Red Team ops. Performing OSINT is about taking the little bits and pieces of information that you are able to extrapolate about a particular person or entity and pulling the thread on it by running that information through OSINT tools to see what more can be discovered.

STUDY OF OPEN SOURCE INTELLIGENCE TOOLS

This chapter introduces and demonstrates OSINT tools for gathering intelligence from open sources. The set of selected tools presented here is a good example of how OSINT tools differ from each other. The solutions represent different types of OSINT applications, providing a wider view on the scale of available OSINT solutions. The range of OSINT solutions is generally very broad – solutions may be designed to focus only on single queries, whereas more powerful OSINT solutions have an ability to perform inquiries of a much larger scale (11). Many of the larger scale OSINT solutions are custom made and designed with huge budgets for governments and giant companies, and accessible naturally only by the owner of the solutions. These solutions are powerful with automated processes, with artificial intelligence and advanced filtering Technics (1). Consequently, the access to such solutions is restricted. However, the number of tools and resources generally accessible by public is also remarkable allowing for powerful searches.

\---------------  (¯\`·.\_.··¸.-\~\*´¨¯¨\`\*·\~(  ([2019-OSINT-GUIDE](https://www.randhome.io/blog/2019/01/05/2019-osint-guide/))  )\~\*´¨¯¨\`\*·\~-.¸··.\_.·´¯) 

S**earch Engines**

Depending on the context, you may want to use a different search engine during an investigation. I mostly rely on Google and Bing (for Europe or North America), Baidu (for Asia) and Yandex (for Russia and Eastern Europe).

Of course, the first investigation tool is search operators. You will find a complete list of these operators for Google [here](http://www.googleguide.com/advanced_operators_reference.html), here is an extract of the most interesting one:

We have found the search with quotation marks to be extremely valuable when searching the following:

* Email address
* Phone number
* User name
* Pin Code 

You can use the following Boolean logical operators to combine queries: AND, OR, + and -

* filetype:allows to search for specific file extensions
* site:will filter on a specific website
* intitle:and inurl:will filter on the title or the url
* link:: find webpages having a link to a specific url (deprecated in 2017, but still partially work)

Some examples

* NAME + CV + filetype:pdfcan help you find someone CV
* DOMAIN - site:DOMAINmay help you find subdomains of a website
* SENTENCE - site:ORIGINDOMAINmay help you find website that plagiarized or copied an article
* site:example.com/folder: If one knows a site’s basic architecture, this combination can drill down the site. E.g, site:amazon.com/India
* site:sub.example.com: Helps drill down into specific sub-domains. E.g, site:local.amazon.com
* site:example.com inurl:abc: The “site:” operator combined with “inurl:” operator can find the sub-domains. More so, because the "inurl:" is much more flexible than putting the sub-domain directly into the main query. E.g, site:amazon.com inurl:local.
* site:example.com inurl:https: This combination helps find any secure pages that the Google has indexed. E.g, site:amazon.com

Additional readings:

* [https://booleanstrings.com/tools/](https://booleanstrings.com/tools/)
* [Mastering Google Search Operators in 67 Easy Steps](https://moz.com/blog/mastering-google-search-operators-in-67-steps)
* [Google Hacking Database](https://www.exploit-db.com/google-hacking-database)

Images

For images, there are two things you want to know: how to find any additional information on an image and how to find similar images.

To find additional information, the first step is to look at  [https://exifdata.com/](https://exifdata.com/)  Exif data are data embedded into an image when the image is created and it often contains interesting information on the creation date, the camera used, sometimes GPS data etc. To check it, I like using the command line [ExifTool](https://exiftool.org/) but the Exif Viewer extension (for [Chrome](https://chrome.google.com/webstore/detail/exif-viewer/nafpfdcmppffipmhcpkbplhkoiekndck) and [Firefox](https://addons.mozilla.org/en-US/firefox/addon/exif-viewer/)) is also really handy. Additionally, you can use this amazing [**Photo Forensic website**](https://29a.ch/photo-forensics/) that has many interesting features. (Other alternatives are [exif.regex.info](http://exif.regex.info/exif.cgi) and [Foto Forensics](https://fotoforensics.com/)).

To find similar images, you can use either [Google Images](https://images.google.com/?hl=fr), [Bing Images](https://www.bing.com/images/), [Yandex Images](https://yandex.com/images/) or [TinyEye](https://tineye.com/). TinyEye has a useful API (see [here](http://www.automatingosint.com/blog/2015/11/osint-youtube-tineye-reverse-image-search/) how to use it) and Bing has a very useful feature letting you search for a [specific part of an image](https://www.cnet.com/news/bing-visual-search-within-images/). To get better results, it can be helpful to remove the background of the image, [remove.bg](https://www.remove.bg/) is an interesting tool for that.

There is no easy way to analyse the content of an image and find its location for instance. You will have to look for specific items in the image that let you guess in which country it can be, and then do online research and compare with Satelite images. I would suggest to read some good investigations by Bellingcat to learn more about it, like [this one](https://www.bellingcat.com/resources/case-studies/2015/03/03/stunt-geolocation-verifying-the-unverifiable/) or [this one](https://www.bellingcat.com/resources/case-studies/2014/07/18/identifying-the-location-of-the-mh17-linked-missile-launcher-from-one-photograph/).

Additional readings:

* [Metadata: MetaUseful & MetaCreepy](https://www.bellingcat.com/resources/how-tos/2015/04/24/metadata-metauseful-metacreepy/) by Bellingcat
* [The Visual Verification Guide](https://firstdraftnews.org/wp-content/uploads/2017/03/FDN_verificationguide_photos.pdf?x40896) by First Draft news

Social Networks

For social network, there are many tools available, but they are strongly platform dependent. Here is a short extract of interesting tools and tricks:

* **Twitter:** the API gives you the exact creation time and tool used to publish tweets. x0rz’ [tweets\_analyzer](https://github.com/x0rz/tweets_analyzer) is a great way to have an overview of the activity of an account. There are ways to find a Twitter id from an email address but they are [a bit tricky](https://booleanstrings.com/2018/05/02/how-to-find-the-twitter-id-from-an-email-address/).
* **Facebook:** the best resource for Facebook investigation is [Michael Bazzell’s website](https://inteltechniques.com/), especially his [custom FB tool’s page](https://inteltechniques.com/osint/facebook.html)
* **LinkedIn:** the most useful trick I have found in LinkedIn is how to find a [LinkedIn profile based on an email address](https://inteltechniques.com/blog/2018/04/25/linkedin-profiles-by-email/).

[**Tinfoleak.com**](https://tinfoleak.com/) / say hello to a website where you can get detailed information about any Twitter user. It is a web interface OSINT tool, authored by Vicente Aguilera Diaz (16). is fully web-based and does not require any installations by the user. Tinfoleak is a good example of a web-based OSINT solution for this thesis demonstrating how easily one can have access to OSINT queries.

To fetch user related data from Twitter with Tinfoleak, only a Twitter username of the user of interest is required, and that is public information. As a result of a query, Tinfoleak provides a detailed report on the Twitter user. The report provides basic information (e.g. name, picture, location, followers) of the user and information on devices, operating systems, applications and social networks used by the Twitter user, place and geolocation coordinates of locations visited by the Twitter user, allowing to download all pictures from a Twitter user, showing also all hashtags, and topics used by the Twitter user (with date and time), and also who the Twitter user has mentioned in their. tweets. Tinfoleak also utilizes the geo information from tweets and images locating the places where the user has been tweeting.

\----------------------------------------------------------------------------------------

I have done my best to vet/ all links within the links below just encase you are skeptical or wise here is a sandbox to test them

[https://www.joesandbox.com/](https://www.joesandbox.com/) and a multi - [https://www.hybrid-analysis.com/](https://www.hybrid-analysis.com/)

(¯\`·.\_.··¸.-\~\*´¨¯¨\`\*·\~ ^(▬▬ι═══════ﺤ)  OSINT - WAREHOUSE  ^(▬▬ι═══════ﺤ) )\~\*´¨¯¨\`\*·\~-.¸ 

* [https://osint.link/](https://osint.link/)
* [Bellingcat toolbox](https://docs.google.com/document/d/1BfLPJpRtyq4RFtHJoNpvWQjmGnyVkfE2HYoICKOGguA/edit)
* [tracelabs tookit](https://www.tracelabs.org/resources/tools/)
* [https://osintframework.com/](https://osintframework.com/)
* [http://researchclinic.net/links.html#Social\_media\_tools](http://researchclinic.net/links.html#Social_media_tools)
* [https://cyber-cops.com/investigation-tools/welcome-to-osirt](https://cyber-cops.com/investigation-tools/welcome-to-osirt)
* [https://www.einvestigator.com/open-source-intelligence-tools/](https://www.einvestigator.com/open-source-intelligence-tools/)
* [https://300m.com/osint/](https://300m.com/osint/)
* [https://start.me/p/wMdQMQ/tools](https://start.me/p/wMdQMQ/tools)
* [https://securitytrails.com/blog/what-is-osint-how-can-i-make-use-of-it](https://securitytrails.com/blog/what-is-osint-how-can-i-make-use-of-it)
* [https://www.toddington.com/resources/tii-free-resources-knowledge-base/](https://www.toddington.com/resources/tii-free-resources-knowledge-base/)
* [OSINT\_Handbook](https://www.i-intelligence.eu/wp-content/uploads/2018/06/OSINT_Handbook_June-2018_Final.pdf)
* [http://rr.reuser.biz/](http://rr.reuser.biz/)
* [https://www.aware-online.com/en/osint-tools/](https://www.aware-online.com/en/osint-tools/)
* [Maltego](https://www.paterva.com/)
* [Hunchly](https://www.hunch.ly/)
* [/recon-ng](https://tools.kali.org/information-gathering/recon-ng)
* [https://netbootcamp.org/osinttools/](https://netbootcamp.org/osinttools/)
* [https://booleanstrings.com/tools/](https://booleanstrings.com/tools/)
* [https://www.coreysdigs.com/take-action/must-have-tools-for-digging-videos-podcasts/](https://www.coreysdigs.com/take-action/must-have-tools-for-digging-videos-podcasts/)
* [https://github.com/smicallef/spiderfoot](https://github.com/smicallef/spiderfoot)
* [https://github.com/tzkuat/Ressources/blob/master/OSINT.md](https://github.com/tzkuat/Ressources/blob/master/OSINT.md)
* [https://github.com/jivoi/awesome-osint](https://github.com/jivoi/awesome-osint)
* [https://leak-lookup.com/](https://leak-lookup.com/)
* [https://www.osinttechniques.com/osint-tools.html](https://www.osinttechniques.com/osint-tools.html)
* [https://github.com/jmortega/osint\_tools\_security\_auditing](https://github.com/jmortega/osint_tools_security_auditing)
* [https://github.com/search?q=OSINT+TOOLS](https://github.com/search?q=OSINT+TOOLS)

============  ----------------✺ ▬▬ι═══════ﺤ ✺-------------- =============

The question of tool's is always a curious one in info-sec, So let me say it clearly: **tools do not matter, it is what you do with tools that matter**. If you don’t know what you are doing, tools won’t help you, they will just give you a long list of data that you won’t be able to understand or assess. Test tools, read their code, create your own tools etc, but be sure that you understand what they do.. The best toolkit is the one you know, like and master.