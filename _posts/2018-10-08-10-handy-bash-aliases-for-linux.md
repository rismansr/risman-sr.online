---
ID: 7
post_title: 10 handy Bash aliases for Linux
author: risman
post_excerpt: ""
layout: post
permalink: >
  http://blog.risman-sr.online/os/linux/10-handy-bash-aliases-for-linux/
published: true
post_date: 2018-10-08 13:33:53
---
<!-- wp:heading -->
<h2>Get more efficient by using condensed versions of long Bash commands.</h2>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p>How many times have you repeatedly typed out a long command on the command line and wished there was a way to save it for later? This is where Bash aliases come in handy. They allow you to condense long, cryptic commands down to something easy to remember and use. Need some examples to get you started? No problem!</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>To use a Bash alias you've created, you need to add it to your .bash_profile file, which is located in your home folder. Note that this file is hidden and accessible only from the command line. The easiest way to work with this file is to use something like Vi or Nano.</p>
<!-- /wp:paragraph -->

<!-- wp:heading -->
<h2 id="handy-bash-aliases">10 handy Bash aliases</h2>
<!-- /wp:heading -->

<!-- wp:list -->
<ul><li>How many times have you needed to unpack a .tar file and couldn't remember the exact arguments needed? Aliases to the rescue! Just add the following to your .bash_profile file and then use <strong>untar FileName</strong> to unpack any .tar file.</li></ul>
<!-- /wp:list -->

<!-- wp:code -->
<pre class="wp-block-code"><code>alias untar='tar -zxvf '</code></pre>
<!-- /wp:code -->

<!-- wp:list -->
<ul><li>Want to download something but be able to resume if something goes wrong?</li></ul>
<!-- /wp:list -->

<!-- wp:code -->
<pre class="wp-block-code"><code>alias wget='wget -c '</code></pre>
<!-- /wp:code -->

<!-- wp:list -->
<ul><li>Need to generate a random, 20-character password for a new online account? No problem.</li></ul>
<!-- /wp:list -->

<!-- wp:code -->
<pre class="wp-block-code"><code>alias getpass="openssl rand -base64 20"</code></pre>
<!-- /wp:code -->

<!-- wp:list -->
<ul><li>Downloaded a file and need to test the checksum? We've got that covered too.</li></ul>
<!-- /wp:list -->

<!-- wp:code -->
<pre class="wp-block-code"><code>alias sha='shasum -a 256 '</code></pre>
<!-- /wp:code -->

<!-- wp:list -->
<ul><li>A normal ping will go on forever. We don't want that. Instead, let's limit that to just five pings.</li></ul>
<!-- /wp:list -->

<!-- wp:code -->
<pre class="wp-block-code"><code>alias ping='ping -c 5'</code></pre>
<!-- /wp:code -->

<!-- wp:list -->
<ul><li>Start a web server in any folder you'd like.</li></ul>
<!-- /wp:list -->

<!-- wp:code -->
<pre class="wp-block-code"><code>alias www='python -m SimpleHTTPServer 8000'</code></pre>
<!-- /wp:code -->

<!-- wp:list -->
<ul><li>Want to know how fast your network is? Just download Speedtest-cli and use this alias. You can choose a server closer to your location by using the <strong>speedtest-cli --list</strong> command.</li></ul>
<!-- /wp:list -->

<!-- wp:code -->
<pre class="wp-block-code"><code>alias speed='speedtest-cli --server 2406 --simple'</code></pre>
<!-- /wp:code -->

<!-- wp:list -->
<ul><li>How many times have you needed to know your external IP address and had no idea how to get that info? Yeah, me too.</li></ul>
<!-- /wp:list -->

<!-- wp:code -->
<pre class="wp-block-code"><code>alias ipe='curl ipinfo.io/ip'</code></pre>
<!-- /wp:code -->

<!-- wp:list -->
<ul><li>Need to know your local IP address?</li></ul>
<!-- /wp:list -->

<!-- wp:code -->
<pre class="wp-block-code"><code>alias ipi='ipconfig getifaddr en0'</code></pre>
<!-- /wp:code -->

<!-- wp:list -->
<ul><li>Finally, let's clear the screen.</li></ul>
<!-- /wp:list -->

<!-- wp:code -->
<pre class="wp-block-code"><code>alias c='clear'</code></pre>
<!-- /wp:code -->

<!-- wp:paragraph -->
<p>As you can see, Bash aliases are a super-easy way to simplify your life on the command line. Want more info? I recommend a quick Google search for "Bash aliases" or a trip to GitHub.</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>source: <a href="https://opensource.com/article/18/9/handy-bash-aliases">https://opensource.com/article/18/9/handy-bash-aliases</a></p>
<!-- /wp:paragraph -->