---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---
<script src="https://ajax.googleapis.com/ajax/libs/jquery/3.5.1/jquery.min.js"></script>
<script>
  $(document).ready(function () {
    $(".abstract").hide();
    $(".button").on("click", function () {
        $(this).next(".abstract").slideToggle(400);
    });
});
</script>


<style>
.abstract{text-align:justify; }
.button{ text-align:justify; }
</style>

{% if author.googlescholar %}
  You can also find my articles on <u><a href="{{author.googlescholar}}">my Google Scholar profile</a>.</u>
{% endif %}



<ol reversed>
<div id="6">
<li> <b>Securing Software in the Presence of Third-Party Modules</b>, <em>Licentiate thesis</em>, 2021 [<a href="/papers/licentiate.pdf">pdf</a>] [<a href="https://research.chalmers.se/en/publication/525880">link</a>] [<a href="https://youtu.be/0Mdj-sNxqXU">video</a>]
  <br>Supervisor: Andrei Sabelfeld
<div class='button' data-content="toggle-text"><a href="#6">abstract</a></div>
<div class='abstract'>
Modular programming is a key concept in software development where the program consists of code modules that are designed and implemented independently. This approach accelerates the development process and enhances scalability of the final product. Modules, however, are often written by third parties, aggravating security concerns such as stealing confidential information, tampering with sensitive data, and executing malicious code.
<p style="margin-top: -0.1%;">
Trigger-Action Platforms (TAPs) are concrete examples of employing modular programming. Any user can develop TAP applications by connecting trigger and action services, and publish them on public repositories. In the presence of malicious application makers, users cannot trust applications written by third parties, which can threaten users’ and platform’s security.</p>
<p style="margin-top: -2.5%;">
We present SandTrap, a novel runtime monitor for JavaScript that can be used to securely integrate third-party applications. SandTrap enforces fine-grained access control policies at the levels of module, API, value, and context. We instantiate SandTrap to IFTTT, Zapier, and Node-RED, three popular JavaScript-driven TAPs, and illustrate how it enforces various policies on a set of benchmarks while incurring a tolerable runtime overhead. We also prove soundness and transparency of the monitoring framework on an essential model of Node-RED.</p>
<p style="margin-top: -2.5%;">
Furthermore, nontransitive policies have been recently introduced as a natural fit for coarse-grained information-flow control where labels are specified at the level of modules. The flow relation does not need to be transitive, resulting in nonstandard noninterference and enforcement mechanism. We develop a lattice encoding to prove that nontransitive policies can be reduced to classical transitive policies. We also devise a lightweight program transformation that leverages standard flow-sensitive information-flow analyses to enforce nontransitive policies more permissively.</p>
</div></li></div>

<div id="5">
<li> <b>Securing Node-RED Applications</b>, <em>Protocols, Strands, and Logic: Festschrift in honor of Joshua Guttman'21</em> [<a href="/papers/joshua21.pdf">pdf</a>]
<br><i>Mohammad M. Ahmadpanah</i>, Musard Balliu, Daniel Hedin, Lars Eric Olsson, and Andrei Sabelfeld
<br><a class='button' data-content="toggle-text" href="#5">abstract</a>
<div class='abstract'>
Trigger-Action Platforms (TAPs) play a vital role in fulfilling the promise of the Internet of Things (IoT) by seamlessly connecting otherwise unconnected devices and services. While enabling novel and exciting applications across a variety of services, security and privacy issues must be taken into consideration because TAPs essentially act as persons-in-the-middle between trigger and action services. The issue is further aggravated since the triggers and actions on TAPs are mostly provided by third parties extending the trust beyond the platform providers.
<p style="margin-top: -0.1%;">
Node-RED, an open-source JavaScript-driven TAP, provides the opportunity for users to effortlessly employ and link nodes via a graphical user interface. Being built upon Node.js, third-party developers can extend the platform's functionality through publishing nodes and their wirings, known as flows.</p>
<p style="margin-top: -2.5%;">
This paper proposes an essential model for Node-RED, suitable to reason about nodes and flows, be they benign, vulnerable, or malicious. We expand on attacks discovered in recent work, ranging from exfiltrating data from unsuspecting users to taking over the entire platform by misusing sensitive APIs within nodes. We present a formalization of a runtime monitoring framework for a core language that soundly and transparently enforces fine-grained allowlist policies at module-, API-, value-, and context-level. We introduce the monitoring framework for Node-RED that isolates nodes while permitting them to communicate via well-de ned API calls complying with the policy specified for each node.</p>
</div></li></div>





<div id="4">
<li> <b>Nontransitive Policies Transpiled</b>, <em><a href="http://www.ieee-security.org/TC/EuroSP2021/accepted.html">EuroS&P'21</a></em> [<a href="/papers/eurosp21.pdf">pdf</a>] [<a href="https://www.cse.chalmers.se/research/group/security/ntni/">link</a>] [<a href="https://youtu.be/mAMgyhWL-AE?t=320">short talk</a>]
<br><i>Mohammad M. Ahmadpanah</i>, Aslan Askarov, and Andrei Sabelfeld
<div class='button' data-content="toggle-text"><a href="#4">abstract</a></div>
<div class='abstract'>
Nontransitive Noninterference (NTNI) and Nontransitive Types (NTT) are a new security condition and enforcement for policies, which in contrast to Denning's classical lattice model, assume no transitivity of the underlying flow relation. Nontransitive security policies are a natural fit for coarse-grained information-flow control where labels are specified at module rather than variable level of granularity.
<p style="margin-top: -0.1%;">
While the nontransitive and transitive policies pursue different goals and have different intuitions, this paper demonstrates that nontransitive noninterference can be in fact reduced to classical transitive noninterference. We develop a power-lattice encoding that establishes a precise relation between NTNI and classical noninterference. Our results make it possible to clearly position the new NTNI characterization with respect to the large body of work on noninterference. Further, we devise a lightweight program transformation that enables us to leverage standard flow-sensitive information-flow analyses to enforce nontransitive policies. We demonstrate several immediate benefits of our approach, both theoretical and practical. First, we improve the permissiveness over (while retaining the soundness of) the nonstandard NTT enforcement. Second, our results naturally generalize to a language with intermediate input and outputs. Finally, we demonstrate the practical benefits by leveraging state-of-the-art flow-sensitive tool JOANA to enforce nontransitive policies for Java programs.</p>
</div></li></div>

<div id="3">
<li> <b>SandTrap: Securing JavaScript-driven Trigger-Action Platforms</b>, <em><a href="https://www.usenix.org/conference/usenixsecurity21/presentation/ahmadpanah">USENIX Security'21</a></em> [<a href="/papers/usenix21.pdf">pdf</a>] [<a href="https://www.cse.chalmers.se/research/group/security/SandTrap/">link</a>]
<br><i>Mohammad M. Ahmadpanah</i>, Daniel Hedin, Musard Balliu, Lars Eric Olsson, and Andrei Sabelfeld
<br><a class='button' data-content="toggle-text" href="#3">abstract</a>
<div class='abstract'>
Trigger-Action Platforms (TAPs) seamlessly connect a wide variety of otherwise unconnected devices and services, ranging from IoT devices to cloud services and social networks. TAPs raise critical security and privacy concerns because a TAP is effectively a “person-in-the-middle” between trigger and action services. Third-party code, routinely deployed as “apps” on TAPs, further exacerbates these concerns. This paper focuses on JavaScript-driven TAPs. We show that the popular IFTTT and Zapier platforms and an open-source alternative Node-RED are susceptible to attacks ranging from exfiltrating data from unsuspecting users to taking over the entire platform. We report on the changes by the platforms in response to our findings and present an empirical study to assess the implications for Node-RED. Motivated by the need for a secure yet flexible way to integrate third-party JavaScript apps, we propose SandTrap, a novel JavaScript monitor that securely combines the Node.js vm module with fully structural proxy-based two-sided membranes to enforce fine-grained access control policies. To aid developers, SandTrap includes a policy generation mechanism. We instantiate SandTrap to IFTTT, Zapier, and Node-RED and illustrate on a set of benchmarks how SandTrap enforces a variety of policies while incurring a tolerable runtime overhead.
</div></li></div>


<div id="2">
<li> <b>Improving Multi-Execution-based Mechanisms for Enforcing Information Flow Policies</b>, <em>Master's thesis</em>, 2017 [<a href="https://github.com/smahmadpanah/MScDocuments/blob/master/Thesis/Thesis.pdf">pdf</a>] [<a href="https://github.com/smahmadpanah/MScDocuments/tree/master/Thesis">link</a>]
  <br>Supervisor: Mehran S. Fallah
<div class='button' data-content="toggle-text"><a href="#2">abstract</a></div>
<div class='abstract'>
Secure Multi-Execution (SME) proves to be a successful technique for
enforcing noninterference. A security mechanism based on SME schedules and
executes multiple copies of a given program, one copy for each security
level, and controls the input/output operations of the copies in a certain
manner. A main challenge in devising such mechanisms is to achieve precision,
which basically stipulates that changes to the executions of secure programs
must be as minimal as possible. Although research in this area has yielded
interesting results, the proposed mechanisms do not attain an acceptable
level of precision even for the security policies that are weakly sensitive
to the timing behavior of programs. This paper proposes a sound and highly
precise mechanism for a strong timing-sensitive noninterference. Using a
specific round-robin-like scheduler, the mechanism indeed arrives at a
highest level of precision demanding that the relative order of input/output
events from different security levels should be preserved.
</div></li></div>


<div id="2'">
<li> <b>Dynamic Enforcement of Security Hyperproperties: A Survey</b>, <em>Technical report</em>, 2016 [<a href="https://github.com/smahmadpanah/MScDocuments/blob/master/Seminar/Dynamic%20Enforcement%20of%20Security%20Hyperproperties-SeminarReport.pdf">pdf</a>]
<br>Supervisor: Mehran S. Fallah
<div class='button' data-content="toggle-text"><a href="#2'">abstract</a></div>
<div class='abstract'>
Security policies can be categorized as properties and non-properties. Information flow control is one of the important confidentiality and integrity policies. The difference between expressing policies using only one or more than one trace entails several enforcement mechanisms. 
<p style="margin-top: -0.1%;">
Two main types of security enforcement mechanisms are static and dynamic. The common feature of static mechanisms is being conservative due to source-code static analysis before the execution. On the other side, runtime monitoring is a well-known technique among dynamic mechanisms. Recently, permissiveness of dynamic techniques for enforcing information flow policies, compared to static analysis, has attracted increasing attraction. Hybrid approaches make use of source-code analysis as additional information on other possible executions of the program under the monitor. Security enforcement mechanisms can be measured in terms of soundness, transparency, and precision. </p>
<p style="margin-top: -2.5%;">
In this technical report, we review the notion of security policies and hyperproperties. We study a wide range of enforcement techniques, including static mechanisms, dynamic mechanisms, program rewriting, and hybrid analysis. We also review the characterization of various dynamic mechanisms and runtime monitors (with or without prior knowledge of possible behaviors of the program) in the literature with reference to enforcement paradigms and comparison factors. </p>
</div></li></div>

<div id="1">
<li> <b>A Tool for Rewriting-Based Enforcement of Noninterference in While Programs</b>, <em>Bachelor's thesis</em>, 2015 [<a href="https://github.com/smahmadpanah/BScProject/blob/master/Final%20Documents/Thesis.pdf">pdf</a>] [<a href="https://github.com/smahmadpanah/BScProject">link</a>]
<br>Supervisor: Mehran S. Fallah
<div class='button' data-content="toggle-text"><a href="#1">abstract</a></div>
<div class='abstract'>
  Program rewriting has recently been suggested as a means of enforcing security
policies and proven more powerful than execution monitoring and static analysis.
We implement a novel, sound and transparent rewriting mechanism
using Program Dependence Graphs (PDG) to enforce progress-sensitive and -insensitive noninterference in programs with observable intermediate values.
</div></li></div>
</ol>







<!-- 
{% include base_path %}

{% for post in site.publications reversed %}
  {% include archive-single.html %}
{% endfor %}
-->