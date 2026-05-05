---
title: "Building a security-first mindset: three key themes from AWS re:Invent 2023"
url: "https://aws.amazon.com/blogs/security/building-a-security-first-mindset-three-key-themes-from-aws-reinvent-2023/"
date: "Wed, 17 Jan 2024 14:55:42 +0000"
author: "Clarke Rodgers"
feed_url: "https://aws.amazon.com/blogs/security/tag/amazon-detective/feed/"
---
<p><a href="https://reinvent.awsevents.com/faqs/" rel="noopener" target="_blank">AWS re:Invent</a> drew 52,000 attendees from across the globe to Las Vegas, Nevada, November 27 to December 1, 2023.</p> 
<p>Now in its 12<sup>th</sup> year, the conference featured 5 keynotes, 17 innovation talks, and over 2,250 sessions and hands-on labs offering immersive learning and networking opportunities.</p> 
<div class="wp-caption aligncenter" id="attachment_33106" style="width: 790px;">
 <img alt="Amazon CSO Stephen Schmidt" src="https://d2908q01vomqb2.cloudfront.net/22d200f8670dbdb3e253a90eee5098477c95c23d/2024/01/16/main-2292.jpg" width="780" />
 <p class="wp-caption-text" id="caption-attachment-33106">Amazon CSO Stephen Schmidt</p>
</div> 
<p>With dozens of service and feature announcements—and innumerable best practices shared by AWS executives, customers, and <a href="https://aws.amazon.com/partners/work-with-partners/" rel="noopener" target="_blank">partners</a>—the air of excitement was palpable. We were on site to experience all of the innovations and insights, but summarizing highlights isn’t easy. This post details three key security themes that caught our attention.</p> 
<h2>Security culture</h2> 
<p>When we think about cybersecurity, it’s natural to focus on technical security measures that help protect the business. But organizations are made up of people—not technology. The best way to protect ourselves is to foster a proactive, resilient culture of cybersecurity that supports effective risk mitigation, incident detection and response, and continuous collaboration.</p> 
<p>In <a href="https://www.youtube.com/watch?v=FqJlomvyaFo" rel="noopener" target="_blank">Sustainable security culture: Empower builders for success</a>, AWS Global Services Security Vice President Hart Rossman and AWS Global Services Security Organizational Excellence Leader Sarah Currey presented practical strategies for building a sustainable security culture.</p> 
<p>Rossman noted that many customers who meet with AWS about security challenges are attempting to manage security as a project, a program, or a side workstream. To strengthen your security posture, he said, you have to embed security into your business.</p> 
<table style="border-collapse: collapse; border: 1px solid #808080;" width="100%"> 
 <tbody>
  <tr> 
   <td style="background-color: #e6e6e6; padding: 18px; border: 1px solid #808080;" width="100%">“You’ve got to understand early on that security can’t be effective if you’re running it like a project or a program. You really have to run it as an operational imperative—a core function of the business. That’s when magic can happen.” — <strong>Hart Rossman</strong>, <em>Global Services Security Vice President at AWS</em></td> 
  </tr> 
 </tbody>
</table> 
<p>Three best practices can help:</p> 
<ol> 
 <li><strong>Be consistently persistent.</strong> Routinely and emphatically thank employees for raising security issues. It might feel repetitive, but treating security events and escalations as learning opportunities helps create a positive culture—and it’s a practice that can spread to other teams. An empathetic leadership approach encourages your employees to see security as everyone’s responsibility, share their experiences, and feel like collaborators.</li> 
 <li><strong>Brief the board.</strong> Engage executive leadership in regular, business-focused meetings. By providing operational metrics that tie your security culture to the impact that it has on customers, crisply connecting data to business outcomes, and providing an opportunity to ask questions, you can help build the support of executive leadership, and advance your efforts to establish a sustainable proactive security posture.</li> 
 <li><strong>Have a mental model</strong> for creating a good security culture. Rossman presented a diagram (Figure 1) that highlights three elements of security culture he has observed at AWS: a student, a steward, and a builder. If you want to be a good steward of security culture, you should be a student who is constantly learning, experimenting, and passing along best practices. As your stewardship grows, you can become a builder, and progress the culture in new directions.<br />&nbsp;</li> 
</ol> 
<div class="wp-caption aligncenter" id="attachment_33096" style="width: 790px;">
 <img alt="Figure 1: Sample mental model for building security culture" class="size-full wp-image-33096" src="https://d2908q01vomqb2.cloudfront.net/22d200f8670dbdb3e253a90eee5098477c95c23d/2024/01/16/img1.png" style="border: 1px solid #bebebe;" width="780" />
 <p class="wp-caption-text" id="caption-attachment-33096">Figure 1: Sample mental model for building security culture</p>
</div> 
<p>Thoughtful investment in the principles of inclusivity, empathy, and psychological safety can help your team members to confidently speak up, take risks, and express ideas or concerns. This supports an escalation-friendly culture that can reduce employee burnout, and empower your teams to champion security at scale.</p> 
<p>In <a href="https://www.youtube.com/watch?v=Q0Gn9X9wQ7Q" rel="noopener" target="_blank">Shipping securely: How strong security can be your strategic advantage</a>, AWS Enterprise Strategy Director Clarke Rodgers reiterated the importance of security culture to building a security-first mindset. </p> 
<p>Rodgers highlighted three pillars of progression (Figure 2)—aware, bolted-on, and embedded—that are based on meetings with more than 800 customers. As organizations mature from a reactive security posture to a proactive, security-first approach, he noted, security culture becomes a true business enabler.</p> 
<table style="border-collapse: collapse; border: 1px solid #808080;" width="100%"> 
 <tbody>
  <tr> 
   <td style="background-color: #e6e6e6; padding: 18px; border: 1px solid #808080;" width="100%">“When organizations have a strong security culture and everyone sees security as their responsibility, they can move faster and achieve quicker and more secure product and service releases.” — <strong>Clarke Rodgers</strong>, <em>Director of Enterprise Strategy at AWS</em></td> 
  </tr> 
 </tbody>
</table> 
<div class="wp-caption aligncenter" id="attachment_33098" style="width: 790px;">
 <img alt="Figure 2: Shipping with a security-first mindset" class="size-full wp-image-33098" src="https://d2908q01vomqb2.cloudfront.net/22d200f8670dbdb3e253a90eee5098477c95c23d/2024/01/16/img2.png" style="border: 1px solid #bebebe;" width="780" />
 <p class="wp-caption-text" id="caption-attachment-33098">Figure 2: Shipping with a security-first mindset</p>
</div> 
<h2>Human-centric AI</h2> 
<p>CISOs and security stakeholders are increasingly pivoting to a human-centric focus to establish effective cybersecurity, and ease the burden on employees.</p> 
<p>According to <a href="https://www.gartner.com/document/4191399" rel="noopener" target="_blank">Gartner</a>, by 2027, 50% of large enterprise CISOs will have adopted human-centric security design practices to minimize cybersecurity-induced friction and maximize control adoption.</p> 
<p>As Amazon CSO Stephen Schmidt noted in <a href="https://www.youtube.com/watch?v=T-LwDlZbbU4" rel="noopener" target="_blank">Move fast, stay secure: Strategies for the future of security</a>, focusing on technology first is fundamentally wrong. Security is a people challenge for threat actors, and for defenders. To keep up with evolving changes and securely support the businesses we serve, we need to focus on dynamic problems that software can’t solve. </p> 
<p>Maintaining that focus means providing security and development teams with the tools they need to automate and scale some of their work.</p> 
<table style="border-collapse: collapse; border: 1px solid #808080;" width="100%"> 
 <tbody>
  <tr> 
   <td style="background-color: #e6e6e6; padding: 18px; border: 1px solid #808080;" width="100%">“People are our most constrained and most valuable resource. They have an impact on every layer of security. It’s important that we provide the tools and the processes to help our people be as effective as possible.” — <strong>Stephen Schmidt</strong>, <em>CSO at Amazon</em></td> 
  </tr> 
 </tbody>
</table> 
<p>Organizations can use artificial intelligence (AI) to impact all layers of security—but AI doesn’t replace skilled engineers. When used in coordination with other tools, and with appropriate human review, it can help make your security controls more effective.</p> 
<p>Schmidt highlighted the internal use of AI at Amazon to accelerate our software development process, as well as new generative AI-powered <a href="https://aws.amazon.com/about-aws/whats-new/2023/11/amazon-inspector-aws-lambda-code-scanning/" rel="noopener" target="_blank">Amazon Inspector</a>, <a href="https://aws.amazon.com/about-aws/whats-new/2023/11/amazon-detective-group-summaries-generative-ai/" rel="noopener" target="_blank">Amazon Detective</a>, <a href="https://aws.amazon.com/about-aws/whats-new/2023/11/aws-config-generative-ai-powered-natural-language-querying-preview/" rel="noopener" target="_blank">AWS Config</a>, and <a href="https://aws.amazon.com/about-aws/whats-new/2023/11/amazon-codewhisperer-new-enhancements/" rel="noopener" target="_blank">Amazon CodeWhisperer</a> features that complement the human skillset by helping people make better security decisions, using a broader collection of knowledge. This pattern of combining sophisticated tooling with skilled engineers is highly effective, because it positions people to make the nuanced decisions required for effective security that AI can’t make on its own.</p> 
<p>In <a href="https://www.youtube.com/watch?v=iiBUiC-2nPM&amp;list=PLB3flZ7qA4xu__uOEfpc-coXm04swNWva&amp;index=12" rel="noopener" target="_blank">How security teams can strengthen security using generative AI</a>, AWS Senior Security Specialist Solutions Architects Anna McAbee and Marshall Jones, and Principal Consultant Fritz Kunstler featured a virtual security assistant (chatbot) that can address common security questions and use cases based on your internal knowledge bases, and trusted public sources.</p> 
<div class="wp-caption aligncenter" id="attachment_33099" style="width: 790px;">
 <img alt="Figure 3: Generative AI-powered chatbot architecture" class="size-full wp-image-33099" src="https://d2908q01vomqb2.cloudfront.net/22d200f8670dbdb3e253a90eee5098477c95c23d/2024/01/16/img3.png" style="border: 1px solid #bebebe;" width="780" />
 <p class="wp-caption-text" id="caption-attachment-33099">Figure 3: Generative AI-powered chatbot architecture</p>
</div> 
<p>The generative AI-powered solution depicted in Figure 3—which includes Retrieval Augmented Generation (RAG) with <a href="https://aws.amazon.com/kendra/" rel="noopener" target="_blank">Amazon Kendra</a>, <a href="https://aws.amazon.com/security-lake/" rel="noopener" target="_blank">Amazon Security Lake</a>, and <a href="https://aws.amazon.com/bedrock/" rel="noopener" target="_blank">Amazon Bedrock</a>—can help you automate mundane tasks, expedite security decisions, and increase your focus on novel security problems.</p> 
<p>It’s <a href="https://github.com/aws-samples/aws-genai-llm-chatbot" rel="noopener" target="_blank">available on Github</a> with ready-to-use code, so you can start experimenting with a variety of large and multimodal language models, settings, and prompts in your own AWS account.</p> 
<h2>Secure collaboration</h2> 
<p>Collaboration is key to cybersecurity success, but evolving threats, flexible work models, and a growing patchwork of data protection and privacy regulations have made maintaining <a href="https://aws.amazon.com/blogs/security/reduce-the-security-and-compliance-risks-of-messaging-apps-with-aws-wickr/" rel="noopener" target="_blank">secure and compliant messaging</a> a challenge.</p> 
<p>An estimated 3.09 billion mobile phone users access messaging apps to communicate, and this figure is projected to grow to <a href="https://www.statista.com/statistics/483255/number-of-mobile-messaging-users-worldwide/" rel="noopener" target="_blank">3.51 billion</a> users in 2025.</p> 
<p>The use of consumer messaging apps for business-related communications makes it more difficult for organizations to verify that data is being adequately protected and retained. This can lead to increased risk, particularly in industries with unique recordkeeping requirements.</p> 
<p>In <a href="https://www.youtube.com/watch?v=yYCTLr9YqO8" rel="noopener" target="_blank">How the U.S. Army uses AWS Wickr to deliver lifesaving telemedicine</a>, Matt Quinn, Senior Director at The U.S. Army Telemedicine &amp; Advanced Technology Research Center (TATRC), Laura Baker, Senior Manager at Deloitte, and Arvind Muthukrishnan, AWS Wickr Head of Product highlighted how The TATRC National Emergency Tele-Critical Care Network (NETCCN) was integrated with <a href="https://aws.amazon.com/wickr/" rel="noopener" target="_blank">AWS Wickr</a>—a HIPAA-eligible secure messaging and collaboration service—and <a href="https://aws.amazon.com/private5g/" rel="noopener" target="_blank">AWS Private 5G</a>, a managed service for deploying and scaling private cellular networks.</p> 
<p>During the session, Quinn, Baker, and Muthukrishnan described how TATRC achieved a low-resource, cloud-enabled, virtual health solution that facilitates secure collaboration between onsite and remote medical teams for real-time patient care in austere environments. Using Wickr, medics on the ground were able to treat injuries that exceeded their previous training (Figure 4) with the help of end-to-end encrypted video calls, messaging, and file sharing with medical professionals, and securely retain communications in accordance with organizational requirements.</p> 
<table style="border-collapse: collapse; border: 1px solid #808080;" width="100%"> 
 <tbody>
  <tr> 
   <td style="background-color: #e6e6e6; padding: 18px; border: 1px solid #808080;" width="100%">“Incorporating Wickr into Military Emergency Tele-Critical Care Platform (METTC-P) not only provides the security and privacy of end-to-end encrypted communications, it gives combat medics and other frontline caregivers the ability to gain instant insight from medical experts around the world—capabilities that will be needed to address the simultaneous challenges of prolonged care, and the care of large numbers of casualties on the multi-domain operations (MDO) battlefield.” — <strong>Matt Quinn</strong>, <em>Senior Director at TATRC</em></td> 
  </tr> 
 </tbody>
</table> 
<div class="wp-caption aligncenter" id="attachment_33102" style="width: 790px;">
 <img alt="Figure 4: Telemedicine workflows using AWS Wickr" class="size-full wp-image-33102" src="https://d2908q01vomqb2.cloudfront.net/22d200f8670dbdb3e253a90eee5098477c95c23d/2024/01/16/img4.png" style="border: 1px solid #bebebe;" width="780" />
 <p class="wp-caption-text" id="caption-attachment-33102">Figure 4: Telemedicine workflows using AWS Wickr</p>
</div> 
<p>In a separate Chalk Talk titled <em>Bolstering Incident Response with AWS Wickr and Amazon EventBridge, </em>Senior AWS Wickr Solutions Architects Wes Wood and Charles Chowdhury-Hanscombe demonstrated how to integrate Wickr with <a href="https://aws.amazon.com/pm/eventbridge/?gclid=EAIaIQobChMI9Nq8uuOegwMVFU9HAR0qZgFEEAAYASAAEgKkx_D_BwE&amp;trk=023e579b-fefa-4cea-8fe9-eca10449ac3a&amp;sc_channel=ps&amp;ef_id=EAIaIQobChMI9Nq8uuOegwMVFU9HAR0qZgFEEAAYASAAEgKkx_D_BwE:G:s&amp;s_kwcid=AL!4422!3!629393325334!!!g!!!16080176144!133788117598" rel="noopener" target="_blank">Amazon EventBridge</a> and <a href="https://aws.amazon.com/guardduty/" rel="noopener" target="_blank">Amazon GuardDuty</a> to strengthen incident response capabilities with an integrated workflow (Figure 5) that connects your AWS resources to Wickr bots. Using this approach, you can quickly alert appropriate stakeholders to critical findings through a secure communication channel, even on a potentially compromised network.</p> 
<div class="wp-caption aligncenter" id="attachment_33103" style="width: 790px;">
 <img alt="Figure 5: AWS Wickr integration for incident response communications" class="size-full wp-image-33103" src="https://d2908q01vomqb2.cloudfront.net/22d200f8670dbdb3e253a90eee5098477c95c23d/2024/01/16/img5.png" style="border: 1px solid #bebebe;" width="780" />
 <p class="wp-caption-text" id="caption-attachment-33103">Figure 5: AWS Wickr integration for incident response communications</p>
</div> 
<h2>Security is our top priority</h2> 
<p>AWS re:Invent featured many more highlights on a variety of topics, including adaptive access control with <a href="https://aws.amazon.com/blogs/security/new-whitepaper-available-charting-a-path-to-stronger-security-with-zero-trust/" rel="noopener" target="_blank">Zero Trust</a>, <a href="https://www.youtube.com/watch?v=lPyV8kTpBjk" rel="noopener" target="_blank">AWS cyber insurance partners</a>, Amazon CTO <a href="https://www.youtube.com/watch?v=UTRBVPvzt9w" rel="noopener" target="_blank">Dr. Werner Vogels’</a> popular keynote, and the security partnerships showcased on the Expo floor. It was a whirlwind experience, but one thing is clear: AWS is working hard to help you build a security-first mindset, so that you can meaningfully improve both technical and business outcomes.</p> 
<p>To watch on-demand conference sessions, visit the <a href="https://www.youtube.com/watch?v=Vf-s3ZQmJhc&amp;list=PLB3flZ7qA4xu__uOEfpc-coXm04swNWva" rel="noopener" target="_blank">AWS re:Invent Security, Identity, and Compliance playlist on YouTube</a>.</p> 
<p>If you have feedback about this post, submit comments in the <strong>Comments</strong> section below.</p> 
<p><strong>Want more AWS Security news? Follow us on <a href="https://twitter.com/AWSsecurityinfo" rel="noopener noreferrer" target="_blank" title="Twitter">Twitter</a>.</strong></p> 
<footer> 
 <div class="blog-author-box"> 
  <div class="blog-author-image"> 
   <img alt="Clarke Rodgers" class="aligncenter size-full wp-image-33105" height="160" src="https://d2908q01vomqb2.cloudfront.net/22d200f8670dbdb3e253a90eee5098477c95c23d/2024/01/16/Clarke-Rodgers.jpg" width="120" /> 
  </div> 
  <h3 class="lb-h4">Clarke Rodgers</h3> 
  <p>Clarke is a Director of Enterprise Security at AWS. Clarke has more than 25 years of experience in the security industry, and works with enterprise security, risk, and compliance-focused executives to strengthen their security posture, and understand the security capabilities of the cloud. Prior to AWS, Clarke was a CISO for the North American operations of a multinational insurance company. </p> 
  <p></p>
 </div> 
 <div class="blog-author-box"> 
  <div class="blog-author-image"> 
   <img alt="Anne Grahn" class="aligncenter size-full wp-image-26275" height="160" src="https://d2908q01vomqb2.cloudfront.net/22d200f8670dbdb3e253a90eee5098477c95c23d/2022/06/16/agrahn.jpg" width="120" /> 
  </div> 
  <h3 class="lb-h4">Anne Grahn</h3> 
  <p>Anne is a Senior Worldwide Security GTM Specialist at AWS, based in Chicago. She has more than 13 years of experience in the security industry, and focuses on effectively communicating cybersecurity risk. She maintains a Certified Information Systems Security Professional (CISSP) certification.</p> 
  <p></p>
 </div> 
</footer>
