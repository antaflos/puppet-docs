---
layout: default
built_from_commit: bf21e710449e0f547daacd58df9685c937b7936e
title: 'Resource Type: stage'
canonical: "/puppet/latest/types/stage.html"
---

> **NOTE:** This page was generated from the Puppet source code on 2017-10-02 13:43:52 -0700

stage
-----

* [Attributes](#stage-attributes)

<h3 id="stage-description">Description</h3>

A resource type for creating new run stages.  Once a stage is available,
classes can be assigned to it by declaring them with the resource-like syntax
and using
[the `stage` metaparameter](https://docs.puppetlabs.com/puppet/latest/reference/metaparameter.html#stage).

Note that new stages are not useful unless you also declare their order
in relation to the default `main` stage.

A complete run stage example:

    stage { 'pre':
      before => Stage['main'],
    }

    class { 'apt-updates':
      stage => 'pre',
    }

Individual resources cannot be assigned to run stages; you can only set stages
for classes.

<h3 id="stage-attributes">Attributes</h3>

<pre><code>stage { 'resource title':
  <a href="#stage-attribute-name">name</a> =&gt; <em># <strong>(namevar)</strong> The name of the stage. Use this as the value for </em>
  # ...plus any applicable <a href="{{puppet}}/metaparameter.html">metaparameters</a>.
}</code></pre>

<h4 id="stage-attribute-name">name</h4>

_(**Namevar:** If omitted, this attribute's value defaults to the resource's title.)_

The name of the stage. Use this as the value for the `stage` metaparameter
when assigning classes to this stage.

([↑ Back to stage attributes](#stage-attributes))





> **NOTE:** This page was generated from the Puppet source code on 2017-10-02 13:43:52 -0700