---
ID: 2704
post_title: 2018 Zcash Security Audit Details
author: Zooko Wilcox
post_excerpt: ""
layout: post
permalink: >
  https://blog.z.cash/2018-zcash-security-audit-details/
published: true
post_date: 2018-03-27 19:52:16
---
We at Zcash are committed to the security and safety of our user community as we seek to empower everyone with economic freedom and opportunity.

Zcash has engaged five leading industry experts to conduct comprehensive security and design audits in support of the <a href="https://z.cash/upgrade/overwinter.html">Overwinter</a> and <a href="https://blog.z.cash/cultivating-sapling-faster-zksnarks/">Sapling</a> in line with <a href="https://blog.z.cash/2018-security-audits/">our approach to comprehensive peer reviews</a>.
<h2>Audit Scope</h2>
The audits will focus on changes to Zcash since our <a href="https://blog.z.cash/audit-results/">prior reviews</a>, including security analysis of protocol design, cryptographic constructions, consensus rules, and implementation. We have also engaged with cryptographic scientists to analyze security arguments, proofs, and constructions.

All Overwinter changes will be audited and are presented in five Zcash Improvement Proposals (ZIPs):
<ul>
 	<li><a href="https://github.com/zcash/zips/blob/master/zip-0200.rst">ZIP 200</a></li>
 	<li><a href="https://github.com/zcash/zips/blob/master/zip-0201.rst">ZIP 201</a></li>
 	<li><a href="https://github.com/zcash/zips/blob/master/zip-0202.rst">ZIP 202</a></li>
 	<li><a href="https://github.com/zcash/zips/blob/master/zip-0203.rst">ZIP 203</a></li>
 	<li><a href="https://github.com/zcash/zips/blob/master/zip-0143.rst">ZIP 143</a></li>
</ul>
The Sapling libraries to be audited are:
<ul>
 	<li>An implementation of a new pairing-friendly elliptic curve in the Rust <a href="https://github.com/ebfull/pairing">pairing library</a></li>
 	<li>The Rust library for building zk-SNARKs called <a href="https://github.com/ebfull/bellman">Bellman</a></li>
 	<li>Various components as part of the <a href="https://github.com/ebfull/sapling-crypto">Sapling-crypto</a> implementation </li>
</ul>
As with the previous audit, we are also commissioning a review of the C++ code including race conditions, networking, buffer overflows and dependency management.

We will bring forward <a href="https://blog.z.cash/auditing-zcash/#scope">previous audit assumptions</a> and assume that previous security audits were accurate and truthful.
<h2>Auditors</h2>
All audits will be performed by top security, cryptology and technology professionals. Each auditor will have a specific focus and scope. 

<a href="https://www.nccgroup.trust/us/">NCC Group</a>: The NCC Group is a leading cybersecurity firm. They have prior experience with the Zcash through their <a href="https://blog.z.cash/audit-results/#ncc-group">audit</a> of the initial Zcash protocol implementation, <a href="https://github.com/zcash/zcash">source code</a> and <a href="https://blog.z.cash/ceremony-audit-results/">ceremony artifacts</a>.

<a href="https://coinspect.com/">Coinspect</a>: Coinspect provides Bitcoin security services. As with their <a href="https://blog.z.cash/audit-results/#coinspect">previous audit</a>, they will place specific emphasis on Zcash additions over the Bitcoin Core source code. 

<a href="https://leastauthority.com/">Least Authority</a> - Recently spun off as a <a href="https://blog.z.cash/spinning-off-our-sibling-company/">sibling company</a> of Zcash Company, the Least Authority team is highly experienced in security audits and design analysis including <a href="https://leastauthority.com/blog/least_authority_performs_incentive_analysis_for_ethereum/">Ethereum’s gas model</a>. 

<a href="https://www.kudelskisecurity.com/">Kudelski Security</a> - Kudelski is a highly regarded international cybersecurity company. The specific auditor engaged, Jean-Philippe Aumasson, is a accomplished cryptographer, having written numerous papers analyzing cryptographic algorithms, and authored several important cryptographic algorithms, including BLAKE2, SipHash, and Gravity-SPHINCS. 

<a href="http://www0.cs.ucl.ac.uk/staff/M.Maller/">Mary Maller</a> - As a PhD candidate in the area of cryptography at the University of London under the supervision of <a href="http://www0.cs.ucl.ac.uk/staff/S.Meiklejohn/">Dr Sarah Meiklejohn</a> and <a href="http://www0.cs.ucl.ac.uk/staff/j.groth/">Dr Jens Groth</a>, Maller is studying the formal design and analysis of cryptographic protocols including different types of signature schemes and how they can be used in blockchain technologies. 
<h2>Understanding Risk</h2>
Zcash is sophisticated and novel technology. While security audits help reduce risk, they cannot eliminate them entirely. Additionally, each auditor is focused on a specific kind of analysis and cannot vouch for the entire system, nor do they necessarily endorse Zcash as a product.
<h2>Schedule</h2>
The audits are underway. Final reports of all Overwinter and Sapling related audits will be completed before code is activated in the main Zcash network. 

As stated in the <a href="https://blog.z.cash/new-release-1-0-15/">1.0.15 release announcement</a>, the scheduled activation for Overwinter on testnet went live at block 207500. The upcoming 1.1.0 release will set an activation block height on the main network.

While we intend to release these upgrades according to our current schedule, the security and stability of the Zcash network is our priority. Any unforeseen issues arising from our testing or these audits may delay releases.