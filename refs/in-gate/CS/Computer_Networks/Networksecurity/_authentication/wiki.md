The following text has been accessed from https://en.wikipedia.org/wiki/Authentication at Fri Aug 9 01:10:36 IST 2019
Creative_Commons_Attribution-ShareAlike_License





















****** Authentication ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
For other uses of the terms "authentic" and "authenticity", see Authenticity.
Not to be confused with authorization.
ATM user authenticating himself
Authentication (from Greek: Î±á½Î¸ÎµÎ½ÏÎ¹ÎºÏÏ authentikos, "real, genuine",
from Î±á½Î¸Î­Î½ÏÎ·Ï authentes, "author") is the act of proving an assertion,
such as the identity of a computer system user. In contrast with
identification, the act of indicating a person or thing's identity,
authentication is the process of verifying that identity. It might involve
validating personal identity_documents, verifying the authenticity of a website
with a digital_certificate,[1] determining the age of an artifact by carbon
dating, or ensuring that a product or document is not counterfeit.
⁰
***** Contents *****
    * 1_Methods
    * 2_Authentication_factors
          o 2.1_Single-factor_authentication
          o 2.2_Multi-factor_authentication
    * 3_Authentication_types
          o 3.1_Strong_authentication
          o 3.2_Continuous_authentication
          o 3.3_Digital_authentication
          o 3.4_Product_authentication
                # 3.4.1_Packaging
    * 4_Information_content
          o 4.1_Literacy_and_literature_authentication
    * 5_History_and_state-of-the-art
    * 6_Authorization
    * 7_Access_control
    * 8_See_also
    * 9_References
    * 10_External_links
***** Methods[edit] *****
Main article: Provenance
Authentication is relevant to multiple fields. In art, antiques and
anthropology, a common problem is verifying that a given artifact was produced
by a certain person or in a certain place or period of history. In computer
science, verifying a user's identity is often required to allow access to
confidential data or systems.[2]
Authentication can be considered to be of three types:
The first type of authentication is accepting proof of identity given by a
credible person who has first-hand evidence that the identity is genuine. When
authentication is required of art or physical objects, this proof could be a
friend, family member or colleague attesting to the item's provenance, perhaps
by having witnessed the item in its creator's possession. With autographed
sports memorabilia, this could involve someone attesting that they witnessed
the object being signed. A vendor selling branded items implies authenticity,
while he or she may not have evidence that every step in the supply chain was
authenticated. Centralized authority-based trust relationships back most secure
internet communication through known public certificate authorities;
decentralized peer-based trust, also known as a web_of_trust, is used for
personal services such as email or files (pretty_good_privacy, GNU_Privacy
Guard) and trust is established by known individuals signing each other's
cryptographic_key at Key_signing_parties, for instance.
The second type of authentication is comparing the attributes of the object
itself to what is known about objects of that origin. For example, an art
expert might look for similarities in the style of painting, check the location
and form of a signature, or compare the object to an old photograph. An
archaeologist, on the other hand, might use carbon_dating to verify the age of
an artifact, do a chemical and spectroscopic analysis of the materials used, or
compare the style of construction or decoration to other artifacts of similar
origin. The physics of sound and light, and comparison with a known physical
environment, can be used to examine the authenticity of audio recordings,
photographs, or videos. Documents can be verified as being created on ink or
paper readily available at the time of the item's implied creation.
Attribute comparison may be vulnerable to forgery. In general, it relies on the
facts that creating a forgery indistinguishable from a genuine artifact
requires expert knowledge, that mistakes are easily made, and that the amount
of effort required to do so is considerably greater than the amount of profit
that can be gained from the forgery.
In art and antiques, certificates are of great importance for authenticating an
object of interest and value. Certificates can, however, also be forged, and
the authentication of these poses a problem. For instance, the son of Han_van
Meegeren, the well-known art-forger, forged the work of his father and provided
a certificate for its provenance as well; see the article Jacques_van_Meegeren.
Criminal and civil penalties for fraud, forgery, and counterfeiting can reduce
the incentive for falsification, depending on the risk of getting caught.
Currency and other financial instruments commonly use this second type of
authentication method. Bills, coins, and cheques incorporate hard-to-duplicate
physical features, such as fine printing or engraving, distinctive feel,
watermarks, and holographic imagery, which are easy for trained receivers to
verify.
The third type of authentication relies on documentation or other external
affirmations. In criminal courts, the rules_of_evidence often require
establishing the chain_of_custody of evidence presented. This can be
accomplished through a written evidence log, or by testimony from the police
detectives and forensics staff that handled it. Some antiques are accompanied
by certificates attesting to their authenticity. Signed sports memorabilia is
usually accompanied by a certificate of authenticity. These external records
have their own problems of forgery and perjury, and are also vulnerable to
being separated from the artifact and lost.
In computer science, a user can be given access_to_secure_systems based on user
credentials that imply authenticity. A network administrator can give a user a
password, or provide the user with a key card or other access device to allow
system access. In this case, authenticity is implied but not guaranteed.
Consumer_goods such as pharmaceuticals, perfume, fashion clothing can use all
three forms of authentication to prevent counterfeit goods from taking
advantage of a popular brand's reputation (damaging the brand owner's sales and
reputation). As mentioned above, having an item for sale in a reputable store
implicitly attests to it being genuine, the first type of authentication. The
second type of authentication might involve comparing the quality and
craftsmanship of an item, such as an expensive handbag, to genuine articles.
The third type of authentication could be the presence of a trademark on the
item, which is a legally protected marking, or any other identifying feature
which aids consumers in the identification of genuine brand-name goods. With
software, companies have taken great steps to protect from counterfeiters,
including adding holograms, security rings, security threads and color shifting
ink.[3]
***** Authentication factors[edit] *****
The ways in which someone may be authenticated fall into three categories,
based on what are known as the factors of authentication: something the user
knows, something the user has, and something the user is. Each authentication
factor covers a range of elements used to authenticate or verify a person's
identity prior to being granted access, approving a transaction request,
signing a document or other work product, granting authority to others, and
establishing a chain of authority.
Security research has determined that for a positive authentication, elements
from at least two, and preferably all three, factors should be verified.[4] The
three factors (classes) and some of elements of each factor are:
    * the knowledge factors: Something the user knows (e.g., a password,
      partial_password, pass_phrase, or personal_identification_number (PIN),
      challenge_response (the user must answer a question, or pattern),
      Security_question
    * the ownership factors: Something the user has (e.g., wrist band, ID_card,
      security_token, implanted_device, cell_phone with built-in hardware
      token, software_token, or cell_phone holding a software_token)
    * the inherence factors: Something the user is or does (e.g., fingerprint,
      retinal pattern, DNA sequence (there are assorted definitions of what is
      sufficient), signature, face, voice, unique bio-electric signals, or
      other biometric identifier).
**** Single-factor authentication[edit] ****
As the weakest level of authentication, only a single component from one of the
three categories of factors is used to authenticate an individualâs identity.
The use of only one factor does not offer much protection from misuse or
malicious intrusion. This type of authentication is not recommended for
financial or personally relevant transactions that warrant a higher level of
security.[1]
**** Multi-factor authentication[edit] ****
Main article: Multi-factor_authentication
Multi-factor authentication involves two or more authentication factors
(something you know, something you have, or something you are). Two-factor
authentication is a special case of multi-factor authentication involving
exactly two factors.[1]
For example, using a bankcard (something the user has) along with a PIN
(something the user knows) provides two-factor authentication. Business
networks may require users to provide a password (knowledge factor) and a
pseudorandom number from a security_token (ownership factor). Access to a very-
high-security system might require a mantrap screening of height, weight,
facial, and fingerprint checks (several inherence factor elements) plus a PIN
and a day code (knowledge factor elements), but this is still a two-factor
authentication.
***** Authentication types[edit] *****
The most frequent types of authentication available in use for authenticating
online users differ in the level of security provided by combining factors from
the one or more of the three categories of factors for authentication:
**** Strong authentication[edit] ****
Main article: Strong_authentication
The U.S. government's National_Information_Assurance_Glossary defines strong
authentication as
     layered authentication approach relying on two or more authenticators
     to establish the identity of an originator or receiver of
     information.[5]
The European Central Bank (ECB) has defined strong authentication as "a
procedure based on two or more of the three authentication factors". The
factors that are used must be mutually independent and at least one factor must
be "non-reusable and non-replicable", except in the case of an inherence factor
and must also be incapable of being stolen off the Internet. In the European,
as well as in the US-American understanding, strong authentication is very
similar to multi-factor authentication or 2FA, but exceeding those with more
rigorous requirements.[1][6]
The Fast_IDentity_Online_(FIDO)_Alliance has been striving to establish
technical specifications for strong authentication.[7]
**** Continuous authentication[edit] ****
Conventional computer systems authenticate users only at the initial log-in
session, which can be the cause of a critical security flaw. To resolve this
problem, systems need continuous user authentication methods that continuously
monitor and authenticate users based on some biometric trait(s). A study used
behavioural biometrics based in writing styles as a continuous authentication
method.[8]
Recent research has shown the possibility of using smartphonesâ sensors and
accessories to extract some behavioral attributes such as touch dynamics,
keystroke dynamics and gait recognition. These attributes are known as
behavioral biometrics and could be used to verify or identify users implicitly
and continuously on smartphones. The authentication systems that have been
built based on these behavioral biometric traits are known as active or
continuous authentication systems.[9]
**** Digital authentication[edit] ****
Main article: Electronic_authentication
The term digital authentication, also known as electronic authentication,
refers to a group of processes where the confidence for user identities is
established and presented via electronic methods to an information system. It
is also referred to as e-authentication. The digital authentication process
creates technical challenges because of the need to authenticate individuals or
entities remotely over a network. The American National_Institute_of_Standards
and_Technology (NIST) has created a generic model for digital authentication
that describes the processes that are used to accomplish secure authentication:
   1. Enrollment â an individual applies to a credential service provider
      (CSP) to initiate the enrollment process. After successfully proving the
      applicantâs identity, the CSP allows the applicant to become a
      subscriber.
   2. Authentication â After becoming a subscriber, the user receives an
      authenticator e.g., a token and credentials, such as a user name. He or
      she is then permitted to perform online transactions within an
      authenticated session with a relying party, where they must provide proof
      that he or she possesses one or more authenticators.
   3. Life-cycle maintenance â the CSP is charged with the task of
      maintaining the userâs credential of the course of its lifetime, while
      the subscriber is responsible for maintaining his or her authenticator
      (s).[1][10]
The authentication of information can pose special problems with electronic
communication, such as vulnerability to man-in-the-middle_attacks, whereby a
third party taps into the communication stream, and poses as each of the two
other communicating parties, in order to intercept information from each. Extra
identity factors can be required to authenticate each party's identity.
**** Product authentication[edit] ****
A security_hologram label on an electronics box for authentication
Counterfeit products are often offered to consumers as being authentic.
Counterfeit_consumer_goods such as electronics, music, apparel, and counterfeit
medications have been sold as being legitimate. Efforts to control the supply
chain and educate consumers help ensure that authentic products are sold and
used. Even security_printing on packages, labels, and nameplates, however, is
subject to counterfeiting.[citation_needed]
A secure_key_storage_device can be used for authentication in consumer
electronics, network authentication, license management, supply chain
management, etc. Generally the device to be authenticated needs some sort of
wireless or wired digital connection to either a host system or a network.
Nonetheless, the component being authenticated need not be electronic in nature
as an authentication chip can be mechanically attached and read through a
connector to the host e.g. an authenticated ink tank for use with a printer.
For products and services that these secure coprocessors can be applied to,
they can offer a solution that can be much more difficult to counterfeit than
most other options while at the same time being more easily verified.[citation
needed]
*** Packaging[edit] ***
Packaging_and_labeling can be engineered to help reduce the risks of
counterfeit_consumer_goods or the theft and resale of products.[11][12] Some
package constructions are more difficult to copy and some have pilfer-
indicating seals. Counterfeit goods, unauthorized sales (diversion), material
substitution and tampering can all be reduced with these anti-counterfeiting
technologies. Packages may include authentication seals and use security
printing to help indicate that the package and contents are not counterfeit;
these too are subject to counterfeiting. Packages also can include anti-theft
devices, such as dye-packs, RFID tags, or electronic_article_surveillance[13]
tags that can be activated or detected by devices at exit points and require
specialized tools to deactivate. Anti-counterfeiting technologies that can be
used with packaging include:
    * Taggant fingerprinting â uniquely coded microscopic materials that are
      verified from a database
    * Encrypted micro-particles â unpredictably placed markings (numbers,
      layers and colors) not visible to the human eye
    * Holograms â graphics printed on seals, patches, foils or labels and
      used at point of sale for visual verification
    * Micro-printing â second-line authentication often used on currencies
    * Serialized barcodes
    * UV printing â marks only visible under UV light
    * Track_and_trace systems â use codes to link products to database
      tracking system
    * Water indicators â become visible when contacted with water
    * DNA tracking â genes embedded onto labels that can be traced
    * Color-shifting ink or film â visible marks that switch colors or
      texture when tilted
    * Tamper_evident seals and tapes â destructible or graphically verifiable
      at point of sale
    * 2d barcodes â data codes that can be tracked
    * RFID chips
    * NFC chips
***** Information content[edit] *****
Literary_forgery can involve imitating the style of a famous author. If an
original manuscript, typewritten text, or recording is available, then the
medium itself (or its packaging â anything from a box to e-mail_headers) can
help prove or disprove the authenticity of the document. However, text, audio,
and video can be copied into new media, possibly leaving only the informational
content itself to use in authentication. Various systems have been invented to
allow authors to provide a means for readers to reliably authenticate that a
given message originated from or was relayed by them. These involve
authentication factors like:
    * A difficult-to-reproduce physical artifact, such as a seal, signature,
      watermark, special stationery, or fingerprint.
    * A shared_secret, such as a passphrase, in the content of the message.
    * An electronic_signature; public-key_infrastructure is often used to
      cryptographically guarantee that a message has been signed by the holder
      of a particular private key.
The opposite problem is detection of plagiarism, where information from a
different author is passed off as a person's own work. A common technique for
proving plagiarism is the discovery of another copy of the same or very similar
text, which has different attribution. In some cases, excessively high quality
or a style mismatch may raise suspicion of plagiarism.
**** Literacy and literature authentication[edit] ****
In literacy, authentication is a readersâ process of questioning the veracity
of an aspect of literature and then verifying those questions via research. The
fundamental question for authentication of literature is â Does one believe
it? Related to that, an authentication project is therefore a reading and
writing activity which students documents the relevant research process ([14]).
It builds students' critical literacy. The documentation materials for
literature go beyond narrative texts and likely include informational texts,
primary sources, and multimedia. The process typically involves both internet
and hands-on library research. When authenticating historical fiction in
particular, readers consider the extent that the major historical events, as
well as the culture portrayed (e.g., the language, clothing, food, gender
roles), are believable for the period.[2]
***** History and state-of-the-art[edit] *****
NSA KAL-55B Tactical Authentication System used by the U.S. military during the
Vietnam_War â National_Cryptologic_Museum
Historically, fingerprints have been used as the most authoritative method of
authentication, but court cases in the US and elsewhere have raised fundamental
doubts about fingerprint reliability.[citation_needed] Outside of the legal
system as well, fingerprints have been shown to be easily spoofable, with
British_Telecom's top computer-security official noting that "few" fingerprint
readers have not already been tricked by one spoof or another.[15] Hybrid or
two-tiered authentication methods offer a compelling[according_to_whom?]
solution, such as private keys encrypted by fingerprint inside of a USB device.
In a computer data context, cryptographic methods have been developed (see
digital_signature and challenge-response_authentication) which are currently
[when?] not spoofable if and only if the originator's key has not been
compromised. That the originator (or anyone other than an attacker) knows (or
doesn't know) about a compromise is irrelevant. It is not known whether these
cryptographically based authentication methods are provably secure, since
unanticipated mathematical developments may make them vulnerable to attack in
future. If that were to occur, it may call into question much of the
authentication in the past. In particular, a digitally_signed contract may be
questioned when a new attack on the cryptography underlying the signature is
discovered.[citation_needed]
***** Authorization[edit] *****
Main article: Authorization
A sailor checks a driver's identification card before allowing her to enter a
military base.
The process of authorization is distinct from that of authentication. Whereas
authentication is the process of verifying that "you are who you say you are",
authorization is the process of verifying that "you are permitted to do what
you are trying to do". This does not mean authorization presupposes
authentication; an anonymous agent could be authorized to a limited action set.
[16]
***** Access control[edit] *****
Main article: Access_control
One familiar use of authentication and authorization is access_control. A
computer system that is supposed to be used only by those authorized must
attempt to detect and exclude the unauthorized. Access to it is therefore
usually controlled by insisting on an authentication procedure to establish
with some degree of confidence the identity of the user, granting privileges
established for that identity.
***** See also[edit] *****
 This "see_also" section may contain an excessive number of suggestions. Please
 ensure that only the most relevant links are given, that they are not red
 links, and that any links are not already in this article. (December 2016)
 (Learn_how_and_when_to_remove_this_template_message)
    * Access_Control_Service
    * AssureID
    * Atomic_authorization
    * Authentication_Open_Service_Interface_Definition
    * Authenticity_in_art
    * Authorization
    * Basic_access_authentication
    * Biometrics
    * CAPTCHA
    * Chip_Authentication_Program
    * Closed-loop_authentication
    * Diameter_(protocol)
    * Digital_identity
    * EAP
    * Electronic_authentication
    * Encrypted_key_exchange (EKE)
    * Fingerprint_Verification_Competition
    * Geolocation
    * Hash-based_message_authentication_code
    * Identification_(information)
    * Java_Authentication_and_Authorization_Service
    * Kantara_Initiative
    * Kerberos
    * Multi-factor_authentication
    * NeedhamâSchroeder_protocol
    * OAuth â an open standard for authorization
    * OpenAthens
    * OpenID_Connect â an authentication method for the web
    * OpenID â an authentication method for the web
    * Provenance
    * Public-key_cryptography
    * RADIUS
    * Reliance_authentication
    * Secret_sharing
    * Secure_Remote_Password_protocol (SRP)
    * Secure_Shell
    * Security_printing
    * SQRL
    * Strong_authentication
    * Tamper-evident_technology
    * TCP_Wrapper
    * Time-based_authentication
    * Two-factor_authentication
    * Usability_of_web_authentication_systems
    * WooâLam
***** References[edit] *****
   1. ^ a b c d eTurner, Dawn M. "Digital_Authentication:_The_Basics".
      Cryptomathic. Archived from the original on 14 August 2016. Retrieved 9
      August 2016.
   2. .mw-parser-output cite.citation{font-style:inherit}.mw-parser-output
      .citation q{quotes:"\"""\"""'""'"}.mw-parser-output .citation .cs1-lock-
      free a{background:url("//upload.wikimedia.org/wikipedia/commons/thumb/6/
      65/Lock-green.svg/9px-Lock-green.svg.png")no-repeat;background-position:
      right .1em center}.mw-parser-output .citation .cs1-lock-limited a,.mw-
      parser-output .citation .cs1-lock-registration a{background:url("//
      upload.wikimedia.org/wikipedia/commons/thumb/d/d6/Lock-gray-alt-2.svg/
      9px-Lock-gray-alt-2.svg.png")no-repeat;background-position:right .1em
      center}.mw-parser-output .citation .cs1-lock-subscription a{background:
      url("//upload.wikimedia.org/wikipedia/commons/thumb/a/aa/Lock-red-alt-
      2.svg/9px-Lock-red-alt-2.svg.png")no-repeat;background-position:right
      .1em center}.mw-parser-output .cs1-subscription,.mw-parser-output .cs1-
      registration{color:#555}.mw-parser-output .cs1-subscription span,.mw-
      parser-output .cs1-registration span{border-bottom:1px dotted;cursor:
      help}.mw-parser-output .cs1-ws-icon a{background:url("//
      upload.wikimedia.org/wikipedia/commons/thumb/4/4c/Wikisource-logo.svg/
      12px-Wikisource-logo.svg.png")no-repeat;background-position:right .1em
      center}.mw-parser-output code.cs1-code{color:inherit;background:
      inherit;border:inherit;padding:inherit}.mw-parser-output .cs1-hidden-
      error{display:none;font-size:100%}.mw-parser-output .cs1-visible-error
      {font-size:100%}.mw-parser-output .cs1-maint{display:none;color:
      #33aa33;margin-left:0.3em}.mw-parser-output .cs1-subscription,.mw-parser-
      output .cs1-registration,.mw-parser-output .cs1-format{font-size:95%}.mw-
      parser-output .cs1-kern-left,.mw-parser-output .cs1-kern-wl-left{padding-
      left:0.2em}.mw-parser-output .cs1-kern-right,.mw-parser-output .cs1-kern-
      wl-right{padding-right:0.2em}
   3. ^ a bMcTigue, E.; Thornton, E.; Wiese, P. (2013). "Authentication
      Projects_for_Historical_Fiction:_Do_you_believe_it?". The Reading
      Teacher. 66 (6): 495â505. doi:10.1002/trtr.1132. Archived from the
      original on 2015-07-07.
   4. ^"How_to_Tell_â_Software". microsoft.com. Archived from the original on
      20 December 2016. Retrieved 11 December 2016.
   5. ^Federal Financial Institutions Examination Council (2008).
      "Authentication_in_an_Internet_Banking_Environment" (PDF). Archived (PDF)
      from the original on 2010-05-05. Retrieved 2009-12-31.
   6. ^Committee on National Security Systems. "National_Information_Assurance_
      (IA)_Glossary" (PDF). National Counterintelligence and Security Center.
      Archived (PDF) from the original on 21 November 2016. Retrieved 9 August
      2016.
   7. ^European Central Bank. "Recommendations_for_the_Security_of_Internet
      Payments" (PDF). European Central Bank. Archived (PDF) from the original
      on 6 November 2016. Retrieved 9 August 2016.
   8. ^"FIDO_Alliance_Passes_150_Post-Password_Certified_Products".
      InfoSecurity Magazine. 2016-04-05. Archived from the original on 2016-06-
      17. Retrieved 2016-06-13.
   9. ^ Brocardo ML, Traore I, Woungang I, Obaidat MS. "Authorship_verification
      using_deep_belief_network_systems Archived 2017-03-22 at the Wayback
      Machine". Int J Commun Syst. 2017. doi:10.1002/dac.3259
  10. ^Mahfouz, Ahmed; Mahmoud, Tarek M.; Eldin, Ahmed Sharaf (2017). "A survey
      on behavioral biometric authentication on smartphones". Journal of
      Information Security and Applications. 37: 28â37. arXiv:1801.09308.
      doi:10.1016/j.jisa.2017.10.002.
  11. ^"Draft_NIST_Special_Publication_800-63-3:_Digital_Authentication
      Guideline". National Institute of Standards and Technology, USA. Archived
      from the original on 13 September 2016. Retrieved 9 August 2016.
  12. ^Eliasson, C; Matousek (2007). "Noninvasive Authentication of
      Pharmaceutical Products through Packaging Using Spatially Offset Raman
      Spectroscopy". Analytical Chemistry. 79 (4): 1696â1701. doi:10.1021/
      ac062223z. PMID 17297975.
  13. ^Li, Ling (March 2013). "Technology designed to combat fakes in the
      global supply chain". Business Horizons. 56 (2): 167â177. doi:10.1016/
      j.bushor.2012.11.010.
  14. ^ How_Anti-shoplifting_Devices_Work" Archived 2006-04-27 at the Wayback
      Machine, HowStuffWorks.com
  15. ^ Norton, D. E. (2004). The effective teaching of language arts. New
      York: Pearson/Merrill/Prentice Hall.
  16. ^ The_Register,_UK;_Dan_Goodin;_30_March_2008;_Get_your_German_Interior
      Minister's_fingerprint,_here._Compared_to_other_solutions,_"It's
      basically_like_leaving_the_password_to_your_computer_everywhere_you_go,
      without_you_being_able_to_control_it_anymore",_one_of_the_hackers
      comments. Archived 10 August 2017 at the Wayback_Machine
  17. ^"Best_Practices_for_Creating_a_Secure_Guest_Account". Archived from the
      original on 2017-11-07. Retrieved 2017-11-06.
***** External links[edit] *****
    * National_Institute_of_Standards_and_Technology, U.S._Department_of
      Commerce (August 2013). "Electronic_Authentication_Guideline_â_NIST
      Special_Publication_800-63-2" (PDF).
"_New_NIST_Publications_Describe_Standards_for_Identity_Credentials_and
Authentication_Systems"
    * v
    * t
    * e
Authentication
                            * BSD_Authentication (BSD Auth)
                            * eAuthentication
                            * Generic_Security_Services_API (GSSAPI)
                            * Java_Authentication_and_Authorization_Service
Authentication APIs           (JAAS)
                            * Pluggable_Authentication_Modules (PAM)
                            * Simple_Authentication_and_Security_Layer (SASL)
                            * Security_Support_Provider_Interface (SSPI)
                            * XCert_Universal_Database_API (XUDA)
                            * ACF2
                            * AKA
                            * CAVE-based_authentication
                            * Challenge-Handshake_Authentication_Protocol
                              (CHAP)
                                  o MS-CHAP
                            * Central_Authentication_Service (CAS)
                            * CRAM-MD5
                            * Diameter
                            * Extensible_Authentication_Protocol (EAP)
                            * Host_Identity_Protocol (HIP)
                            * IndieAuth
                            * Kerberos
Authentication_protocol     * LAN_Manager
                            * NT_LAN_Manager (NTLM)
                            * OAuth
                            * OpenID
                            * OpenID_Connect (OIDC)
                            * Password-authenticated_key_agreement protocols
                            * Password_Authentication_Protocol (PAP)
                            * Protected_Extensible_Authentication_Protocol
                              (PEAP)
                            * Remote_Access_Dial_In_User_Service (RADIUS)
                            * Resource_Access_Control_Facility (RACF)
                            * Secure_Remote_Password_protocol (SRP)
                            * TACACS
                            * WooâLam
    * [Category] Category
    * [Commons page] Commons
Authority_control [Edit_this_at_Wikidata]     * BNF: cb11976657c (data)
                                              * LCCN: sh85009783

Retrieved from "https://en.wikipedia.org/w/
index.php?title=Authentication&oldid=908995028"
Categories:
    * Authentication
    * Applications_of_cryptography
    * Access_control
    * Packaging
    * Notary
    * Computer_access_control
Hidden categories:
    * Webarchive_template_wayback_links
    * Articles_containing_Greek-language_text
    * All_articles_with_unsourced_statements
    * Articles_with_unsourced_statements_from_July_2019
    * Articles_with_unsourced_statements_from_January_2010
    * All_articles_with_specifically_marked_weasel-worded_phrases
    * Articles_with_specifically_marked_weasel-worded_phrases_from_December
      2016
    * All_articles_with_vague_or_ambiguous_time
    * Vague_or_ambiguous_time_from_December_2016
    * Articles_with_unsourced_statements_from_December_2016
    * Articles_with_excessive_see_also_sections_from_December_2016
    * Wikipedia_articles_with_BNF_identifiers
    * Wikipedia_articles_with_LCCN_identifiers
***** Navigation menu *****
**** Personal tools ****
    * Not logged in
    * Talk
    * Contributions
    * Create_account
    * Log_in
**** Namespaces ****
    * Article
    * Talk
⁰
**** Variants ****
**** Views ****
    * Read
    * Edit
    * View_history
⁰
**** More ****
**** Search ****
[Unknown INPUT type][Search][Go]
**** Navigation ****
    * Main_page
    * Contents
    * Featured_content
    * Current_events
    * Random_article
    * Donate_to_Wikipedia
    * Wikipedia_store
**** Interaction ****
    * Help
    * About_Wikipedia
    * Community_portal
    * Recent_changes
    * Contact_page
**** Tools ****
    * What_links_here
    * Related_changes
    * Upload_file
    * Special_pages
    * Permanent_link
    * Page_information
    * Wikidata_item
    * Cite_this_page
**** Print/export ****
    * Create_a_book
    * Download_as_PDF
    * Printable_version
**** Languages ****
    * Ø§ÙØ¹Ø±Ø¨ÙØ©
    * Asturianu
    * AzÉrbaycanca
    * à¦¬à¦¾à¦à¦²à¦¾
    * ÐÑÐ»Ð³Ð°ÑÑÐºÐ¸
    * ÄeÅ¡tina
    * Dansk
    * Deutsch
    * Eesti
    * ÎÎ»Î»Î·Î½Î¹ÎºÎ¬
    * EspaÃ±ol
    * Euskara
    * ÙØ§Ø±Ø³Û
    * FranÃ§ais
    * Galego
    * íêµ­ì´
    * ÕÕ¡ÕµÕ¥ÖÕ¥Õ¶
    * à¤¹à¤¿à¤¨à¥à¤¦à¥
    * Hrvatski
    * Italiano
    * ×¢××¨××ª
    * LatvieÅ¡u
    * Nederlands
    * æ¥æ¬èª
    * Norsk
    * Polski
    * PortuguÃªs
    * Qaraqalpaqsha
    * RomÃ¢nÄ
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Simple_English
    * SlovenÅ¡Äina
    * Ú©ÙØ±Ø¯Û
    * Suomi
    * Svenska
    * TÃ¼rkÃ§e
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * Ø§Ø±Ø¯Ù
    * Tiáº¿ng_Viá»t
    * å´è¯­
    * ç²µèª
    * ä¸­æ
Edit_links
    * This page was last edited on 2 August 2019, at 10:43 (UTC).
    * Text is available under the Creative_Commons_Attribution-ShareAlike
      License; additional terms may apply. By using this site, you agree to the
      Terms_of_Use and Privacy_Policy. WikipediaÂ® is a registered trademark of
      the Wikimedia_Foundation,_Inc., a non-profit organization.
    * Privacy_policy
    * About_Wikipedia
    * Disclaimers
    * Contact_Wikipedia
    * Developers
    * Cookie_statement
    * Mobile_view
    * [Wikimedia_Foundation]
    * [Powered_by_MediaWiki]
