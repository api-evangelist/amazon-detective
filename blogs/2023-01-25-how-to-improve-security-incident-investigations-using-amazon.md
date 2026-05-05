---
title: "How to improve security incident investigations using Amazon Detective finding groups"
url: "https://aws.amazon.com/blogs/security/how-to-improve-security-incident-investigations-using-amazon-detective-finding-groups/"
date: "Wed, 25 Jan 2023 17:34:00 +0000"
author: "Anna McAbee"
feed_url: "https://aws.amazon.com/blogs/security/tag/amazon-detective/feed/"
---
<p>Uncovering the root cause of an <a href="https://aws.amazon.com/guardduty/" rel="noopener" target="_blank">Amazon GuardDuty</a> finding can be a complex task, requiring security operations center (SOC) analysts to collect a variety of logs, correlate information across logs, and determine the full scope of affected resources.</p> 
<p>Sometimes you need to do this type of in-depth analysis because investigating individual security findings in insolation doesn’t always capture the full impact of affected resources.</p> 
<p>With <a href="https://aws.amazon.com/detective/" rel="noopener" target="_blank">Amazon Detective</a>, you can analyze and visualize various logs and relationships between AWS entities to streamline your investigation. In this post, you will learn how to use a <a href="https://aws.amazon.com/about-aws/whats-new/2022/10/amazon-detective-reduce-time-investigate-amazon-guardduty-findings-grouping-related-findings/" rel="noopener" target="_blank">feature</a> of Detective—finding groups—to simplify and expedite the investigation of a GuardDuty finding.</p> 
<p>Detective uses machine learning, statistical analysis, and graph theory to generate visualizations that help you to conduct faster and more efficient security investigations. The finding groups feature reduces triage time and provides a clear view of related GuardDuty findings. With finding groups, you can investigate entities and security findings that might have been overlooked in isolation. Finding groups also map GuardDuty findings and their relevant tactics, techniques, and procedures to the <a href="https://attack.mitre.org/" rel="noopener" target="_blank">MITRE ATT&amp;CK framework</a>. By using MITRE ATT&amp;CK, you can better understand the event lifecycle of a finding group.</p> 
<p>Finding groups are automatically enabled for both existing and new customers in <a href="https://docs.aws.amazon.com/general/latest/gr/detective.html" rel="noopener" target="_blank">AWS Regions that support Detective</a>. There is no additional charge for finding groups. If you don’t currently use Detective, you can <a href="https://aws.amazon.com/detective/pricing/" rel="noopener" target="_blank">start a free 30-day trial</a>.</p> 
<h2>Use finding groups to simplify an investigation</h2> 
<p>Because finding groups are enabled by default, you start your investigation by simply navigating to the Detective console. You will see these finding groups in two different places: the <strong>Summary</strong> and the <strong>Finding groups</strong> pages. On the <strong>Finding groups</strong> overview page, you can also use the search capability to look for collected metadata for finding groups, such as severity, title, finding group ID, observed tactics, AWS accounts, entities, finding ID, and status. The entities information can help you narrow down finding groups that are more relevant for specific workloads.</p> 
<p>Figure 1 shows the finding groups area on the <strong>Summary</strong> page in the Amazon Detective console, which provides high-level information on some of the individual finding groups.</p> 
<div class="wp-caption aligncenter" id="attachment_28334" style="width: 770px;">
 <img alt="Figure 1: Detective console summary page" class="size-large wp-image-28334" src="https://d2908q01vomqb2.cloudfront.net/22d200f8670dbdb3e253a90eee5098477c95c23d/2023/01/19/img1-3-1024x315.png" style="border: 1px solid #bebebe;" width="760" />
 <p class="wp-caption-text" id="caption-attachment-28334">Figure 1: Detective console summary page</p>
</div> 
<p>Figure 2 shows the <strong>Finding groups</strong> overview page, with a list of finding groups filtered by status. The finding group shown has a status of <strong>Active</strong>.</p> 
<div class="wp-caption aligncenter" id="attachment_28335" style="width: 770px;">
 <img alt="Figure 2: Detective console finding groups overview page" class="size-large wp-image-28335" src="https://d2908q01vomqb2.cloudfront.net/22d200f8670dbdb3e253a90eee5098477c95c23d/2023/01/19/img2-4-1024x320.png" style="border: 1px solid #bebebe;" width="760" />
 <p class="wp-caption-text" id="caption-attachment-28335">Figure 2: Detective console finding groups overview page</p>
</div> 
<p>You can choose the finding group title to see details like the severity of the finding group, the status, scope time, parent or child finding groups, and the observed tactics from the MITRE ATT&amp;CK framework. Figure 3 shows a specific finding group details page.</p> 
<div class="wp-caption aligncenter" id="attachment_28336" style="width: 770px;">
 <img alt="Figure 3: Detective console showing a specific finding group details page" class="size-large wp-image-28336" src="https://d2908q01vomqb2.cloudfront.net/22d200f8670dbdb3e253a90eee5098477c95c23d/2023/01/19/img3-2-1024x491.png" style="border: 1px solid #bebebe;" width="760" />
 <p class="wp-caption-text" id="caption-attachment-28336">Figure 3: Detective console showing a specific finding group details page</p>
</div> 
<p>Below the finding group details, you can review the entities and associated findings for this finding group, as shown in Figure 4. From the <strong>Involved entities</strong> tab, you can pivot to the entity profile pages for more details about that entity’s behavior. From the <strong>Involved findings</strong> tab, you can select a finding to review the details pane.</p> 
<div class="wp-caption aligncenter" id="attachment_28337" style="width: 770px;">
 <img alt="Figure 4: Detective console showing involved entities of a finding group" class="size-full wp-image-28337" src="https://d2908q01vomqb2.cloudfront.net/22d200f8670dbdb3e253a90eee5098477c95c23d/2023/01/19/img4-3.png" style="border: 1px solid #bebebe;" width="760" />
 <p class="wp-caption-text" id="caption-attachment-28337">Figure 4: Detective console showing involved entities of a finding group</p>
</div> 
<p>In Figure 4, the search functionality on the <strong>Involved entities</strong> tab is being used to look at involved entities that are of type <strong>AWS role</strong> or <strong>EC2 instance</strong>. With such a search filter in Detective, you have more data in a single place to understand which <a href="https://aws.amazon.com/ec2/" rel="noopener" target="_blank">Amazon Elastic Compute Cloud (Amazon EC2)</a> instances and <a href="https://aws.amazon.com/iam/" rel="noopener" target="_blank">AWS Identity and Access Management (IAM)</a> roles were involved in the GuardDuty finding and what findings were associated with each entity. You can also select these different entities to see more details. With finding groups, you no longer have to craft specific log searches or search for the AWS resources and entities that you should investigate. Detective has done this correlation for you, which reduces the triage time and provides a more comprehensive investigation.</p> 
<p>With the release of finding groups, Detective infers relationships between findings and groups them together, providing a more convenient starting point for investigations. Detective has evolved from helping you determine which resources are related to a single entity (for example, what EC2 instances are communicating with a malicious IP), to correlating multiple related findings together and showing what MITRE tactics are aligned across those findings, helping you better understand a more advanced single security event.</p> 
<h2>Conclusion</h2> 
<p>In this blog post, we showed how you can use Detective finding groups to simplify security investigations through grouping related GuardDuty findings and AWS entities, which provides a more comprehensive view of the lifecycle of the potential security incident. Finding groups are automatically enabled for both existing and new customers in <a href="https://docs.aws.amazon.com/general/latest/gr/detective.html" rel="noopener" target="_blank">AWS Regions that support Detective</a>. There is no additional charge for finding groups. If you don’t currently use Detective, you can <a href="https://aws.amazon.com/detective/pricing/" rel="noopener" target="_blank">start a free 30-day trial</a>. For more information on finding groups, see <a href="https://docs.aws.amazon.com/detective/latest/userguide/groups-about.html" rel="noopener" target="_blank">Analyzing finding groups</a> in the Amazon Detective User Guide.</p> 
<p>If you have feedback about this post, submit comments in the Comments section below. You can also start a new thread on the <a href="https://repost.aws/tags/TAUrK2r73PTHyirNVS4hKn6w/amazon-detective" rel="noopener" target="_blank">Amazon Detective re:Post</a> or <a href="https://console.aws.amazon.com/support/home" rel="noopener" target="_blank">contact AWS Support</a>.</p> 
<p><strong>Want more AWS Security news? Follow us on <a href="https://twitter.com/AWSsecurityinfo" rel="noopener" target="_blank">Twitter</a>.</strong></p> 
<footer> 
 <div class="blog-author-box"> 
  <div class="blog-author-image"> 
   <img alt="Author" class="aligncenter size-full wp-image-16868" height="160" src="https://d2908q01vomqb2.cloudfront.net/22d200f8670dbdb3e253a90eee5098477c95c23d/2023/01/04/Anna-McAbee-author.jpg" width="120" /> 
  </div> 
  <h3 class="lb-h4">Anna McAbee </h3> 
  <p>Anna is a Security Specialist Solutions Architect focused on threat detection and incident response at AWS. Before AWS, she worked as an AWS customer in financial services on both the offensive and defensive sides of security. Outside of work, Anna enjoys cheering on the Florida Gators football team, wine tasting, and traveling the world.</p> 
  <p></p>
 </div> 
 <div class="blog-author-box"> 
  <div class="blog-author-image"> 
   <img alt="Author" class="aligncenter size-full wp-image-16868" height="160" src="https://d2908q01vomqb2.cloudfront.net/22d200f8670dbdb3e253a90eee5098477c95c23d/2021/12/15/Marshall-Jones-Author.jpeg" width="120" /> 
  </div> 
  <h3 class="lb-h4">Marshall Jones </h3> 
  <p>Marshall is a Worldwide Security Specialist Solutions Architect at AWS. His background is in AWS consulting and security architecture, focused on a variety of security domains including edge, threat detection, and compliance. Today, he is focused on helping enterprise AWS customers adopt and operationalize AWS security services to increase security effectiveness and reduce risk.</p> 
  <p></p>
 </div> 
 <div class="blog-author-box"> 
  <div class="blog-author-image"> 
   <img alt="Luis Pastor" class="aligncenter size-full wp-image-28338" height="160" src="https://d2908q01vomqb2.cloudfront.net/22d200f8670dbdb3e253a90eee5098477c95c23d/2023/01/19/Luis-Pastor.jpg" width="120" /> 
  </div> 
  <h3 class="lb-h4">Luis Pastor</h3> 
  <p>Luis is a Security Specialist Solutions Architect focused on infrastructure security at AWS. Before AWS he worked with large and boutique system integrators, helping clients in an array of industries improve their security posture and reach and maintain compliance in hybrid environments. Luis enjoys keeping active, cooking and eating spicy food, specially Mexican cuisine.</p> 
  <p></p>
 </div> 
</footer>
