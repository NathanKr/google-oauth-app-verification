
<h1>Project Name</h1>
my experience with Google OAuth App Verification

<h2>Project Description</h2>
This project show my experince in the process of Google OAuth App Verification of my www.post2youtube.com 


  <h2>What is Google OAuth App Verification?</h2>

  <p>Google OAuth App Verification is a process mandated by Google for third-party applications that use Google's OAuth 2.0 authorization system to access Google user data. The primary goals are to ensure the <strong>safety and trustworthiness</strong> of these applications and to protect users and their data.</p>

  <p>During verification, Google reviews the application's:</p>
  <ul>
    <li><strong>Identity and Branding:</strong> Ensuring accurate representation of the application.</li>
    <li><strong>Requested Scopes:</strong> Verifying the necessity and explanation of requested permissions.</li>
    <li><strong>Privacy Policy:</strong> Confirming a clear and comprehensive data usage disclosure.</li>
    <li><strong>Website and Domain Ownership:</strong> Validating the legitimacy of the associated website.</li>
    <li><strong>Demonstration of Functionality (in some cases):</strong> Reviewing a video showcasing the use of sensitive scopes.</li>
  </ul>

  <p>The benefits of verification include increased user trust, reduced risk of malicious apps, enhanced transparency, and removal of the "Unverified app" warning screen.</p>

  <h2>When is Google OAuth App Verification Required?</h2>

  <p>Google OAuth App Verification is typically required in the following situations:</p>

  <ul>
    <li>
      <h3>Accessing Sensitive or Restricted Scopes</h3>
      <p>If your application requests access to Google API scopes categorized as <strong>sensitive</strong> (e.g., email, calendar, contacts) or <strong>restricted</strong> (granting broad data access), verification is <strong>mandatory</strong>. The Google Cloud Console indicates the scope category.</p>
    </li>
    <li>
      <h3>Displaying Brand Information for External Users</h3>
      <p>For applications with the <strong>User Type</strong> set to <strong>"External"</strong> that want to show their <strong>app name and logo</strong> on the OAuth consent screen, at least <strong>brand verification</strong> is needed.</p>
    </li>
    <li>
      <h3>External User Type and Production Status</h3>
      <p>Apps set to <strong>"External"</strong> with a <strong>"In Production"</strong> publishing status generally require verification, especially when using scopes beyond basic profile information.</p>
    </li>
    <li>
      <h3>Changes to Previously Verified Apps</h3>
      <p>Significant changes to a verified app, such as requesting new sensitive scopes or major branding updates, may necessitate <strong>re-verification</strong>.</p>
    </li>
  </ul>

  <h2>When is Google OAuth App Verification NOT Typically Required?</h2>

  <p>Verification is often not required in these scenarios:</p>

  <ul>
    <li>
      <h3>Personal Use Apps</h3>
      <p>Apps for your personal use or a small number of users (under 100) might not initially need verification. However, scaling beyond this limit will require it, and users will see an "Unverified app" screen.</p>
    </li>
    <li>
      <h3>Development/Testing/Staging Apps</h3>
      <p>Apps in the <strong>"Testing"</strong> publishing status are generally exempt from verification. Keep development and production projects separate. These apps may have a 100-user cap.</p>
    </li>
    <li>
      <h3>Internal Use Apps</h3>
      <p>Apps used solely within your <strong>Google Workspace or Cloud Identity organization</strong>, configured for <strong>internal use</strong>, usually don't need verification. The project must be owned by the organization.</p>
    </li>
    <li>
      <h3>Service-owned Data Only</h3>
      <p>Apps that only access their own data using a <strong>Service Account</strong> and don't access user data do not require verification.</p>
    </li>
  </ul>

  <p><strong>Important:</strong> Regardless of verification status, all apps integrating with Google APIs must adhere to the <a href="https://developers.google.com/terms/api-services-user-data-policy">Google API Services User Data Policy</a>.</p>

  <p>Always consult the <strong>Google Cloud Console's OAuth consent screen settings</strong> for your specific project to determine the exact verification requirements.</p>


<h2>Motivation for me</h2>
required for post2youtube for better UI expereince and more quota chance
In my case i want more than 100 users so it violate 'Personal Use apps'


<h2>important verification steps</h2>

<h3>step 1 : branding</h3>
the app logo requirements are shown in this image
my logo is <a href='https://github.com/NathanKr/post2youtube-website-private/blob/main/public/images/post2youtube_logo_120x120.png'>here</a>

The app logo requirements appear in this image

<img src='./figs/app-logo-requirements.png'/>

I have used chatgpt to create the logo

<h3>step 2 : privecy policy</h3>

The privacy policy appears here

<img src='./figs/privacy-policy.png'/>

But what i did was to provide gemini <a href='https://www.post2youtube.com'>my app landing page</a> and ask him what to do using Q & A session.

check <a href='./figs/post2youtube.com.png'>landing page</a>

and the target appears in <a href='https://www.post2youtube.com/privacy-policy'>my app privacy-policy</a>


check <a href='./figs/post2youtube-privacy-policy.com.png'>privacy-policy</a>

<h3>step 3 : verifiy domain ownership</h3>
<a href='https://support.google.com/webmasters/answer/9008080?sjid=6673206062964333071-EU'>here</a></li>

You can choose any option out of 7 as shown in this image 
<img src='./figs/7-domain-verification-options.png'/>

<h4>post2youtube.com</h4>

google cloud console side <img  src='./figs/verify-google-side.png'/>

domain provider side (nameschaep) <img  src='./figs/verify-namecheap-side.png'/>

back to google clicked verify after few minutes <img src='./figs/google-verified.png'/>

<h4>post2youtube.online</h4>
I was not able to do this using namecheap because i was not able to add record

<h3>step 4 : create a video</h3>
scroll down <a href='https://support.google.com/cloud/answer/13464321?hl=en&ref_topic=13460882&sjid=2157921980951485823-EU#'>here</a>

check <img src='./figs/demo-video.png'/>




<h2>Points of Interest</h2>
<ul>
    <li>why i get verification not needed ? <img src='./figs/verification-not-needed.png'/> : in my case it was still in testing.  the "Verification not needed" status you currently see in your Google OAuth Console will likely disappear or change when you attempt to publish your application</li>
</ul>

<h2>References</h2>
<ul>
    <li><a href='https://support.google.com/cloud/answer/13463073?hl=en'>official docs</a></li>
    <li><a href='https://support.google.com/cloud/answer/13464321?hl=en&ref_topic=13460882&sjid=7676787867668491552-EU'>verification requirement</a></li>
</ul>
