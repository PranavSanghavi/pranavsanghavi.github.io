---
title: Pranav Sanghavi:<br />A Personal Website
layout: home
author: Pranav Sanghavi
date: January 2021
abstract: This website is a brief compilation of details about the author. I direct the reader to pertinent information. This is an eternal work in progress <i class="fa fa-cog fa-spin"></i>
---

<nav role="navigation" class="toc">
    <h2>Contents</h2>
    <ol>
        <li><a href="#intro">Introduction</a></li>
        <li><a href="#research">Research Interstests</a></li>
        <li><a href="#cv">Curriculum Vitae</a></li>
        <li><a href="#misc">Miscellenious</a></li>
    </ol>
</nav>

<div id="ToC"></div>

<h2 id="intro">Introduction</h2>

Hello! I am Pranav Sanghavi, and am a graduate research assistant at West Virginia University, WV, USA. I build radio
telescopes. My doctoral work focuses on Fast Radio Burst detection and Very Large Baseline Interferometric(VLBI)
localization.

<figure>
    <img src="/images/pranav.jpeg" loading="lazy" alt="Pranav" width="250" height="400" />
    <figcaption>
        <em>Figure 1:</em> Pranav Sanghavi, cool person.
        <a href=""></a>
    </figcaption>
</figure>

<h2 id="research">Research Interests</h2>
<ol>
    <li> Radio Astronomy </li>
    <li> Instrumentation </li>
    <li> Fast Radio Bursts </li>
    <li> Very Large Baseline Interferometry (VLBI) </li>
    <li> Cosmology </li>
</ol>
<figure>
    <img src="/images/tone.png" loading="lazy" alt="TONE: Array of radio telescope dishes" width="600" height="400" />
    <figcaption>
        <em>Figure 2:</em> TONE: A 6m parabolic dish array at the Green Bank Observatory.
        <a href=""></a>
    </figcaption>
</figure>

<figure>
    <img src="/images/tone.jpeg" loading="lazy" alt="TONE: Array of radio telescope dishes" width="600" height="400" />
    <figcaption>
        <em>Figure 3:</em> TONE: A 6m parabolic dish array at Green Bank Observatory with the Green Bank Telescope
        in the background.
        <a href=""></a>
    </figcaption>
</figure>

<h2 id="cv">Curriculum Vitae</h2>

Click on the links below to see my CV and the list of contributed publications.

<div style="text-align: center;">
    <a href="{{ site.url }}/cv/" class="button">CV</a>
    <a href="{{ site.url }}/pub_list" class="button">Publication List</a>
</div>

<h2 id="misc">Miscellenious</h2>

When not building radio telescopes and crunching data, one can find me making <a
    href="https://m.soundcloud.com/pranav-sanghavi">music</a> and <a href="https://dimensionslost.com/">painting</a>. I
enjoy long walks and consuming copious amounts of all art and books. I am an avid home cook who occasionally cooks
specials as a guest chef at a local restaurant for fun!

<script type="text/javascript">
    // Get ToC div
    toc = document.getElementById("ToC");

    //Add a header
    tocHeader = document.createElement("h2");
    tocHeader.innerText="Table of contents";
    toc.appendChild(tocHeader);
    
    // Create a list for the ToC entries
    tocList = document.createElement("ol");    

    // Get the h3 tags - ToC entries
    headers = document.getElementsByTagName("h2");
    
    // For each h3
    for (i = 0; i < headers.length; i++){
      
      // Create an id
      name = "h"+i;
      headers[i].id=name;
      
      // a list item for the entry
      tocListItem = document.createElement("li");

      // a link for the h2
      tocEntry = document.createElement("a");
      tocEntry.setAttribute("href","#"+name);
      tocEntry.innerText=headers[i].innerText;
      
      tocListItem.appendChild(tocEntry);
      tocList.appendChild(tocListItem);
    }
    toc.appendChild(tocList);
</script>
