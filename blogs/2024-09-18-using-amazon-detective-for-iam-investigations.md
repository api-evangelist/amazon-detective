---
title: "Using Amazon Detective for IAM investigations"
url: "https://aws.amazon.com/blogs/security/using-amazon-detective-for-iam-investigations/"
date: "Wed, 18 Sep 2024 16:06:31 +0000"
author: "Ahmed Adekunle"
feed_url: "https://aws.amazon.com/blogs/security/tag/amazon-detective/feed/"
---
<blockquote>
 <p><strong>January 31, 2025:</strong> This post was revised to update several paragraphs in the section <strong>Scenario 1: Automated investigations</strong>.</p>
</blockquote> 
<hr /> 
<p>Uncovering&nbsp; <a href="https://aws.amazon.com/iam/" rel="noopener" target="_blank">AWS Identity and Access Management (IAM)</a> users and roles potentially involved in a security event can be a challenging task, requiring security analysts to gather and analyze data from various sources, and determine the full scope of affected resources.</p> 
<p><a href="https://aws.amazon.com/detective/" rel="noopener" target="_blank">Amazon Detective</a> includes <a href="https://docs.aws.amazon.com/detective/latest/userguide/investigations-about.html" rel="noopener" target="_blank">Detective Investigation</a>, a feature that you can use to investigate IAM users and roles to help you determine if a principal is involved in a security event and obtain an in-depth analysis. It automatically analyzes resources in your <a href="https://aws.amazon.com/" rel="noopener" target="_blank">Amazon Web Services (AWS)</a> environment using machine learning and threat intelligence to identify potential indicators of compromise (IoCs) or suspicious activity. This allows analysts to identify patterns and identify which resources are impacted by security events, offering a proactive approach to threat identification and mitigation. Detective Investigation can help determine if IAM principals have potentially been compromised or involved in known <a href="https://csrc.nist.gov/glossary/term/Tactics_Techniques_and_Procedures" rel="noopener" target="_blank">tactics, techniques, and procedures</a> (TTPs) from the <a href="https://attack.mitre.org/" rel="noopener" target="_blank">MITRE ATT&amp;CK framework</a>, a well adopted framework for security and threat detection. MITRE TTPs are the terms used to describe the behaviors, processes, actions, and strategies used by threat actors engaged in cyberattacks.</p> 
<p>In this post, I show you how to use Detective Investigation and how to interpret and use the information provided from an IAM investigation.</p> 
<h2>Prerequisites</h2> 
<p>The following are the prerequisites to follow along with this post:</p> 
<ul> 
 <li>Access to the AWS Management Console with an active <a href="https://portal.aws.amazon.com/billing/signup#/start/email" rel="noopener" target="_blank">AWS account</a>.</li> 
 <li><a href="https://aws.amazon.com/detective/" rel="noopener" target="_blank">Amazon Detective</a> and <a href="https://aws.amazon.com/guardduty/" rel="noopener" target="_blank">Amazon GuardDuty</a> enabled in the same AWS account and AWS Region.</li> 
</ul> 
<h2>Use Detective Investigation to investigate IAM users and roles</h2> 
<p>To get started with an investigation, sign in to the console. The walkthrough uses three scenarios:</p> 
<ol> 
 <li>Automated investigations</li> 
 <li>Investigator persona</li> 
 <li>Threat hunter persona</li> 
</ol> 
<p>In addition to Detective, some of these scenarios also use <a href="https://aws.amazon.com/guardduty" rel="noopener" target="_blank">Amazon GuardDuty</a>, which is an intelligent threat detection service.</p> 
<h2>Scenario 1: Automated investigations</h2> 
<p>Amazon Detective automatically aggregates and displays relevant security information, but automatic investigations must be manually created in the console by <a href="https://docs.aws.amazon.com/detective/latest/userguide/investigations-about.html" rel="noopener" target="_blank">running a Detective investigation</a> or programmatically created through the <a href="https://docs.aws.amazon.com/detective/latest/APIReference/API_StartInvestigation.html" rel="noopener" target="_blank">StartInvestigation API action</a>. After an investigation has been created, you can see the number of IAM roles and users that were impacted by security events over a set period.</p> 
<p>The Detective summary dashboard, shown in Figure 1, shows you the number of critical investigations, high investigations, and the number of IAM roles and users found in suspicious activities over a period of time. <a href="https://docs.aws.amazon.com/detective/latest/userguide/investigations-about.html" rel="noopener" target="_blank">Detective Investigation</a> uses machine learning models and threat intelligence to analyze resources in your AWS environment to identify potential security incidents, allowing you to focus on high-priority investigations. It automatically analyzes resources in your AWS environment to identify potential indicators of compromise or suspicious activity.</p> 
<p>To get to the dashboard using the Detective console, choose <strong>Summary </strong>from the navigation pane.</p> 
<div class="wp-caption aligncenter" id="attachment_35799" style="width: 790px;">
 <img alt="Figure 1: AWS roles and users impacted by a security event" class="size-full wp-image-35799" src="https://d2908q01vomqb2.cloudfront.net/22d200f8670dbdb3e253a90eee5098477c95c23d/2024/09/16/img1-5.png" style="border: 1px solid #bebebe;" width="780" />
 <p class="wp-caption-text" id="caption-attachment-35799">Figure 1: AWS roles and users impacted by a security event</p>
</div> 
<p>Choose <strong>View active investigations</strong> on the <strong>Summary</strong> dashboard to go to the <strong>Investigations</strong> page (shown in Figure 2), which shows potential security events identified by Detective. You can select a specific investigation to view additional details in the investigations report summary.</p> 
<div class="wp-caption aligncenter" id="attachment_35800" style="width: 783px;">
 <img alt="Figure 2: Active investigations that are related to IAM entities" class="size-full wp-image-35800" height="494" src="https://d2908q01vomqb2.cloudfront.net/22d200f8670dbdb3e253a90eee5098477c95c23d/2024/09/16/img2-5.png" style="border: 1px solid #bebebe;" width="773" />
 <p class="wp-caption-text" id="caption-attachment-35800">Figure 2: Active investigations that are related to IAM entities</p>
</div> 
<p>Select a report ID to view its details. Figure 3 shows the details of the selected event under <strong>Indicators of compromise</strong> along with the AWS role that was involved, period of time, role name, and the recommended mitigation action. The indicators of compromise list includes observed tactics from the MITRE ATT&amp;CK framework, flagged IP addresses involved in potential compromise (if any), impossible travel under the indicators, and the finding group. You can continue your investigation by selecting and reviewing the details of each item from the list of indicators of compromise.</p> 
<div class="wp-caption aligncenter" id="attachment_35801" style="width: 790px;">
 <img alt="Figure 3: Summary of the selected investigation" class="size-full wp-image-35801" src="https://d2908q01vomqb2.cloudfront.net/22d200f8670dbdb3e253a90eee5098477c95c23d/2024/09/16/img3-4.png" style="border: 1px solid #bebebe;" width="780" />
 <p class="wp-caption-text" id="caption-attachment-35801">Figure 3: Summary of the selected investigation</p>
</div> 
<p>Figure 4 shows the lower portion of the selected investigation. Detective maps the investigations to TTPs from the MITRE ATT&amp;CK framework. TTPs are classified according to their severity. The console shows the techniques and actions used. When selecting a specific TTP, you can see the details in the right pane. In this example, the valid cloud credential has IP addresses involved in 34 successful API call attempts.</p> 
<div class="wp-caption aligncenter" id="attachment_35802" style="width: 790px;">
 <img alt="Figure 4: TTP mappings" class="size-full wp-image-35802" src="https://d2908q01vomqb2.cloudfront.net/22d200f8670dbdb3e253a90eee5098477c95c23d/2024/09/16/img4-3.png" style="border: 1px solid #bebebe;" width="780" />
 <p class="wp-caption-text" id="caption-attachment-35802">Figure 4: TTP mappings</p>
</div> 
<h2>Scenario 2: Investigator persona</h2> 
<p>For this scenario, you have triaged the resources associated with a GuardDuty finding informing you that an IAM user or role has been identified in an anomalous behavior. You need to investigate and analyze the impact this security issue might have had on other resources and ensure that nothing else needs to be remediated.</p> 
<p>The example for this use case starts by going to the GuardDuty console and choosing <strong>Findings</strong> from the navigation pane, selecting a GuardDuty IAM finding, and then choosing the <strong>Investigate with Detective</strong> link.</p> 
<div class="wp-caption aligncenter" id="attachment_35803" style="width: 776px;">
 <img alt="Figure 5: List of findings in GuardDuty" class="size-full wp-image-35803" height="402" src="https://d2908q01vomqb2.cloudfront.net/22d200f8670dbdb3e253a90eee5098477c95c23d/2024/09/16/img5-2.png" style="border: 1px solid #bebebe;" width="766" />
 <p class="wp-caption-text" id="caption-attachment-35803">Figure 5: List of findings in GuardDuty</p>
</div> 
<p>Let’s now investigate an IAM user associated with the GuardDuty finding. As shown in Figure 6, you have multiple options for pivoting to Detective, such as the GuardDuty finding itself, the AWS account, the role session, and the internal and external IP addresses.</p> 
<div class="wp-caption aligncenter" id="attachment_35804" style="width: 786px;">
 <img alt="Figure 6: Options for pivoting to Detective" class="size-full wp-image-35804" height="426" src="https://d2908q01vomqb2.cloudfront.net/22d200f8670dbdb3e253a90eee5098477c95c23d/2024/09/16/img6-3.png" style="border: 1px solid #bebebe;" width="776" />
 <p class="wp-caption-text" id="caption-attachment-35804">Figure 6: Options for pivoting to Detective</p>
</div> 
<p>From the list of Detective options, you can choose <strong>Role session</strong>, which will help you investigate the IAM role session that was in use when the GuardDuty finding was created. Figure 7 shows the IAM role session page.</p> 
<p>Before moving on to the next section, you would scroll down to <strong>Resources affected</strong> in the <strong>GuardDuty finding details</strong> panel on the right side of the screen and take note of the <strong>Principal ID</strong>.</p> 
<div class="wp-caption aligncenter" id="attachment_35805" style="width: 767px;">
 <img alt="Figure 7: IAM role session page in Detective" class="size-full wp-image-35805" height="414" src="https://d2908q01vomqb2.cloudfront.net/22d200f8670dbdb3e253a90eee5098477c95c23d/2024/09/16/img7-2.png" style="border: 1px solid #bebebe;" width="757" />
 <p class="wp-caption-text" id="caption-attachment-35805">Figure 7: IAM role session page in Detective</p>
</div> 
<p>A role session consists of an instantiation of an IAM role and the associated set of short-term credentials. A role session involves the following:</p> 
<ul> 
 <li>The role that is assumed</li> 
 <li>The entity—IAM user or role, federated user, or <a href="https://aws.amazon.com/ec2" rel="noopener" target="_blank">Amazon Elastic Compute Cloud (Amazon EC2)</a> instance—that assumes the role</li> 
</ul> 
<p>When investigating a role session, consider the following questions:</p> 
<ul> 
 <li>How long has the role been active?</li> 
 <li>Is the role routinely used?</li> 
 <li>Has activity changed over that use?</li> 
 <li>Was the role assumed by multiple users?</li> 
 <li>Was it assumed by a large number of users? A narrowly used role session might guide your investigation differently from a role session with overlapping use.</li> 
</ul> 
<p>You can use the principal ID to get more in-depth details using the Detective search function. Figure 8 shows the search results of an IAM role’s details. To use the search function, choose <strong>Search</strong> from the navigation pane, select <strong>Role session</strong> as the type, and enter an exact identifier or identifier with wildcard characters to search for. Note that the search is case sensitive.</p> 
<p>When you select the assumed role link, additional information about the IAM role will be displayed, helping to verify if the role has been involved in suspicious activities.</p> 
<div class="wp-caption aligncenter" id="attachment_35824" style="width: 662px;">
 <img alt="Figure 8: Results of an IAM role details search" class="size-full wp-image-35824" height="241" src="https://d2908q01vomqb2.cloudfront.net/22d200f8670dbdb3e253a90eee5098477c95c23d/2024/09/18/img8_v2.png" style="border: 1px solid #bebebe;" width="652" />
 <p class="wp-caption-text" id="caption-attachment-35824">Figure 8: Results of an IAM role details search</p>
</div> 
<p>Figure 9 shows other findings related to the role. This information is displayed by choosing the <strong>Assumed Role</strong> link in the search results.</p> 
<p>Now you should see a new screen with information specific to the role entity that you selected. Look through the role information and gather evidence that would be important to you if you were investigating this security issue.</p> 
<p>Were there other findings associated to the role? Was there newly observed activity during this time in terms of new behavior? Were there resource interaction associated with the role? What permissions did this role have?</p> 
<div class="wp-caption aligncenter" id="attachment_35807" style="width: 779px;">
 <img alt="Figure 9: Other findings related to the role" class="size-full wp-image-35807" height="426" src="https://d2908q01vomqb2.cloudfront.net/22d200f8670dbdb3e253a90eee5098477c95c23d/2024/09/16/img9-2.png" style="border: 1px solid #bebebe;" width="769" />
 <p class="wp-caption-text" id="caption-attachment-35807">Figure 9: Other findings related to the role</p>
</div> 
<p>In this scenario, you used Detective to investigate an IAM role session. The information that you have gathered about the security findings will help give you a better understanding of other resources that need to be remediated, how to remediate, permissions that need to be scoped down, and root cause analysis insight to include in your action reports.</p> 
<h2>Scenario 3: Threat hunter persona</h2> 
<p>Another use case is to aid in threat hunting (searching) activities. In this scenario, suspicious activity has been detected in your organization and you need to find out what resources (that is, what IAM entities) have been communicating with a command-and-control IP address. You can check from the Detective summary page for <a href="https://docs.aws.amazon.com/detective/latest/userguide/profile-panel-drilldown-overall-api-volume.html" rel="noopener" target="_blank">roles and users with the highest API call volume</a>,<strong> which automatically lists the IAM roles and users </strong>that were impacted by security events over a set time scope, as shown in Figure 10.</p> 
<div class="wp-caption aligncenter" id="attachment_35808" style="width: 776px;">
 <img alt="Figure 10: Roles and users with the highest API call volume" class="size-full wp-image-35808" height="291" src="https://d2908q01vomqb2.cloudfront.net/22d200f8670dbdb3e253a90eee5098477c95c23d/2024/09/16/img10-1.png" style="border: 1px solid #bebebe;" width="766" />
 <p class="wp-caption-text" id="caption-attachment-35808">Figure 10: Roles and users with the highest API call volume</p>
</div> 
<p>From the list of <strong>Principal (role or user)</strong> options, choose the user or role that you find interesting based on the data presented. Things to consider when choosing the role or user to examine:</p> 
<ul> 
 <li>Is there a role with a large amount of failed API calls?</li> 
 <li>Is there a role with an unusual data trend?</li> 
</ul> 
<p>After choosing a role from the <strong>DetectiveSummary</strong> page, you’re taken to the role overview page. Scroll down to the <strong>Overall API call volume</strong> section to view the overall volume of API calls issued by the resource during the scope time. Detective presents this information to you in a graphical interface without the need to create complex queries.</p> 
<div class="wp-caption aligncenter" id="attachment_35809" style="width: 779px;">
 <img alt="Figure 11: Graph showing API call volume" class="size-full wp-image-35809" height="435" src="https://d2908q01vomqb2.cloudfront.net/22d200f8670dbdb3e253a90eee5098477c95c23d/2024/09/16/img11-1.png" style="border: 1px solid #bebebe;" width="769" />
 <p class="wp-caption-text" id="caption-attachment-35809">Figure 11: Graph showing API call volume</p>
</div> 
<p>In the <strong>Overall API call volume</strong>, choose the <strong>display details for time scope </strong>button at the bottom of the section to search through the observed IP addresses, API method by service, and resource.</p> 
<div class="wp-caption aligncenter" id="attachment_35810" style="width: 790px;">
 <img alt="Figure 12: &lt;strong&gt;Overall API call volume&lt;/strong&gt; during the specified scope time" class="size-full wp-image-35810" src="https://d2908q01vomqb2.cloudfront.net/22d200f8670dbdb3e253a90eee5098477c95c23d/2024/09/16/img12-1.png" style="border: 1px solid #bebebe;" width="780" />
 <p class="wp-caption-text" id="caption-attachment-35810">Figure 12: <strong>Overall API call volume</strong> during the specified scope time</p>
</div> 
<p>To see the details for a specific IP address, use the <strong>Overall API call volume</strong> panel to search through different locations and to determine where the failed API calls came from. Select an IP address to get more granular details (as shown in Figure 13). When looking through this information, think about what this might tell you in your own environment.</p> 
<ul> 
 <li>Do you know who normally uses this role?</li> 
 <li>What is this role used for?</li> 
 <li>Should this role be making calls from various geolocations?</li> 
</ul> 
<div class="wp-caption aligncenter" id="attachment_35826" style="width: 665px;">
 <img alt="Figure 13: Granular details for the selected IP address" class="size-full wp-image-35826" height="413" src="https://d2908q01vomqb2.cloudfront.net/22d200f8670dbdb3e253a90eee5098477c95c23d/2024/09/18/img13_v2.png" style="border: 1px solid #bebebe;" width="655" />
 <p class="wp-caption-text" id="caption-attachment-35826">Figure 13: Granular details for the selected IP address</p>
</div> 
<p>In this scenario, you used Detective to review potentially suspicious activity in your environment related to information assumed to be malicious. If adversaries have assumed the same role with different session names, this gives you more information about how this IAM role was used. If you find information related to the suspicious resources in question, you should conduct a formal search according to your internal incident response playbooks.</p> 
<h2>Conclusion</h2> 
<p>In this blog post, I walked you through how to investigate IAM entities (IAM users or rules) using Amazon Detective. You saw different scenarios on how to investigate IAM entities involved in a security event. You also learned about the <a href="https://aws.amazon.com/about-aws/whats-new/2023/11/amazon-detective-investigations-iam/" rel="noopener" target="_blank">Detective investigations for IAM</a> feature, which you can use to automatically investigate IAM entities for <a href="https://docs.aws.amazon.com/whitepapers/latest/aws-security-incident-response-guide/use-indicators-of-compromise.html" rel="noopener" target="_blank">indicators of compromise</a> (IOCs), helping security analysts determine whether IAM entities have potentially been compromised or involved in known TTPs from the <a href="https://attack.mitre.org/" rel="noopener" target="_blank">MITRE ATT&amp;CK framework</a>.</p> 
<p>There’s no additional charge for this capability, and it’s available today for existing and new Detective customers in&nbsp;<a href="https://docs.aws.amazon.com/general/latest/gr/detective.html" rel="noopener" target="_blank">AWS Regions that support Detective</a>. If you don’t currently use Detective, you can&nbsp;<a href="https://aws.amazon.com/detective/pricing/" rel="noopener" target="_blank">start a free 30-day trial</a>. For more information about Detective investigations, see&nbsp;<a href="https://docs.aws.amazon.com/detective/latest/userguide/investigations-about.html" rel="noopener" target="_blank">Detective Investigation</a>.</p> 
<p>&nbsp;<br />If you have feedback about this post, submit comments in the<strong> Comments</strong> section below. If you have questions about this post, <a href="https://console.aws.amazon.com/support/home" rel="noopener noreferrer" target="_blank">contact AWS Support</a>.<br />&nbsp;</p> 
<footer> 
 <div class="blog-author-box">
  <img alt="Ahmed Adekunle" class="alignleft size-full wp-image-33350" src="https://d2908q01vomqb2.cloudfront.net/22d200f8670dbdb3e253a90eee5098477c95c23d/2024/09/16/ahmedkun.jpg" style="margin-left: 12px; margin-right: 18px; margin-top: 12px; margin-bottom: 6px; width: 93.750px; height: 125px;" />
  <span class="lb-h4" style="line-height: 2.1em; padding-top: 12px; margin-top: 24px;">Ahmed Adekunle</span>
  <br />Ahmed is a Security Specialist Solutions Architect focused on detection and response services at AWS. Before AWS, his background was in business process management and AWS tech consulting, helping customers use cloud technology to transform their business. Outside of work, Ahmed enjoys playing soccer, supporting less privileged activities, traveling, and eating spicy food, specifically African cuisine.
 </div> 
</footer>
