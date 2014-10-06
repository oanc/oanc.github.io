---
layout: default
title: American National Corpus
---

The [American National Corpus](http://www.anc.org) (ANC) maintains a corpus of contemporary
American English. These are some of the software projects developed by the ANC.

### Maven

Most ANC projects are deployed to our own Nexus repository. They are not (yet) pushed to
Maven Central.  To use these projects users must add the following repositories to their
settings.xml file or the project's pom.xml file.

<div class="highlight highlight-xml"><pre><span class="nt">&lt;repository&gt;</span>
  <span class="nt">&lt;id&gt;</span>anc-releases<span class="nt">&lt;/id&gt;</span>
  <span class="nt">&lt;url&gt;</span>http://www.anc.org:8080/nexus/content/repositories/releases/<span class="nt">&lt;/url&gt;</span>
  <span class="nt">&lt;releases&gt;</span>
    <span class="nt">&lt;enabled&gt;</span>true<span class="nt">&lt;/enabled&gt;</span>
  <span class="nt">&lt;/releases&gt;</span>
  <span class="nt">&lt;snapshots&gt;</span>
    <span class="nt">&lt;enabled&gt;</span>false<span class="nt">&lt;/enabled&gt;</span>
  <span class="nt">&lt;/snapshots&gt;</span>
<span class="nt">&lt;/repository&gt;</span>
<span class="nt">&lt;repository&gt;</span>
  <span class="nt">&lt;id&gt;</span>anc-snapshots<span class="nt">&lt;/id&gt;</span>
  <span class="nt">&lt;url&gt;</span>http://www.anc.org:8080/nexus/content/repositories/snapshots/<span class="nt">&lt;/url&gt;</span>
  <span class="nt">&lt;releases&gt;</span>
    <span class="nt">&lt;enabled&gt;</span>false<span class="nt">&lt;/enabled&gt;</span>
  <span class="nt">&lt;/releases&gt;</span>
  <span class="nt">&lt;snapshots&gt;</span>
    <span class="nt">&lt;enabled&gt;</span>true<span class="nt">&lt;/enabled&gt;</span>
    <span class="nt">&lt;updatePolicy&gt;</span>always<span class="nt">&lt;/updatePolicy&gt;</span>
  <span class="nt">&lt;/snapshots&gt;</span>
<span class="nt">&lt;/repository&gt;</span>
</pre></div>

