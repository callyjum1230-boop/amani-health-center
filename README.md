You are a frontend developer building a healthcare website 
for Amani Health Center. This follows styles.css already created.

Build two components: a top crisis bar and the main navigation.

COMPONENT A — Crisis/Emergency Top Bar:
A fixed top strip (height 44px) in deep red (#C0392B), 
full viewport width, above everything else (z-index 1000).
Content centered: 
"🆘 If you are in crisis, call our 24/7 helpline: 
+255 800 AMANI (26264)  |  
<a>Chat Now</a>  |  <a>Text "HELP" to 741741</a>"
- Text: white, Nunito 600, 13px
- Links: white underline, hover turns light yellow
- Dismissible: small "✕" button on far right, 
  clicking hides bar and saves to sessionStorage 
  so it doesn't reappear in session
- When bar is visible, push all content below by 44px 
  (add/remove .has-crisis-bar class on body via JS)

COMPONENT B — Main Navigation:
A sticky navbar below the crisis bar. 
Initial state: transparent background, white text.
Scrolled state (.scrolled class): white background, 
charcoal text, bottom shadow.

LEFT: Logo area — "Amani" in Cormorant Garamond 700 teal, 
"Health Center" in Nunito 300 charcoal, smaller. 
Stack vertically, no image needed.

CENTER (desktop): Nav links in Nunito 600, 14px, 
uppercase letter-spacing:
- Our Programs
- How It Works
- Meet Our Team
- Success Stories
- Insurance & Cost
- Contact Us

RIGHT: Two buttons:
- "VERIFY INSURANCE" (btn-secondary, smaller)
- "GET HELP NOW" (btn-primary)

MOBILE (hamburger):
- Animated hamburger (3 bars → X transform in CSS)
- Full-screen overlay menu, ivory background, 
  centered links in large Cormorant Garamond, 
  teal color, each link fades in with 0.1s stagger
- Social links at bottom of mobile menu: 
  FB | IG | WhatsApp (text links)

JAVASCRIPT (vanilla, no libraries):
1. Scroll listener: add .scrolled to nav after 60px
2. Crisis bar dismiss with sessionStorage
3. Hamburger toggle with aria-expanded
4. Close mobile menu on link click
5. Offset anchor scroll by navbar+crisis bar height

Output: Complete self-contained HTML block for both 
components with <style> and <script> tags. 
Reference CSS variables from styles.css.
