# KungFu Travels — Complete Viva Prep (Zero se Shuru)

Is document mein bilkul basic se le kar project-specific sawalon tak sab hai. Har jawab chhota aur
simple rakha hai — ratta mat maaro, samajh kar padho, phir khud se bolne ki practice karo.

---

## PART 1: Bilkul Basic HTML (agar "HTML kya hai" bhi pooche)

**Q: HTML kya hai?**
A: HyperText Markup Language — ye web pages ka "structure/skeleton" banane ki language hai.
Ye batata hai page mein kya-kya hai (heading, paragraph, image, link) aur kahan hai.

**Q: HTML "tag" kya hota hai?**
A: Angle brackets `< >` mein likhe gaye keywords, jo content ko define karte hain. Jaise `<p>` matlab
paragraph, `<h1>` matlab sabse bada heading.

**Q: Opening tag aur closing tag mein farq?**
A: Opening tag: `<p>`, Closing tag: `</p>` (slash ke sath). Content dono ke beech mein hota hai:
`<p>Ye text hai</p>`. Kuch tags closing nahi mangte, jaise `<img>`, `<br>`.

**Q: Attribute kya hota hai?**
A: Tag ke andar extra information, jaise `<img src="photo.jpg" alt="description">` — yahan `src`
aur `alt` attributes hain jo tag ko extra detail dete hain.

**Q: `<!DOCTYPE html>` kyun likhte hain sabse upar?**
A: Browser ko batata hai "ye ek modern HTML5 document hai" — isay sahi tarike se render karo.

**Q: `<html lang="en">` mein `lang="en"` kyun hai?**
A: Batata hai page ki language English hai — screen readers aur search engines ke liye zaroori hai.

**Q: `<head>` aur `<body>` mein farq?**
A: `<head>` mein wo cheezein hoti hain jo user ko seedha page pe nahi dikhtin (title, CSS link,
meta tags). `<body>` mein wo sab hota hai jo asal mein page pe dikhta hai (headings, text, images).

**Q: `<meta charset="UTF-8">` kya karta hai?**
A: Batata hai page kis character encoding mein hai — isse special characters (jaise Urdu text, ya
symbols) sahi dikhte hain.

**Q: viewport meta tag kya karta hai?**
`<meta name="viewport" content="width=device-width, initial-scale=1.0">`
A: Mobile phones pe page ko sahi size mein dikhata hai — bina is ke page mobile pe bahut chhota
ya zoomed-out dikhta.

---

## PART 2: Semantic HTML Tags

**Q: "Semantic" tag ka matlab kya hai?**
A: Aise tags jo apna **matlab khud bata dete hain** — jaise `<header>` ka naam hi bata raha hai
ye header hai. Isse code padhne mein aasan hota hai aur screen readers bhi behtar samajhte hain.

**Q: `<header>` kya hota hai?**
A: Page ka sabse upar wala hissa — usually logo/site name aur navigation.

**Q: `<nav>` kya hota hai?**
A: Links ka group jo navigation ke liye hai (Home, About, waghera).

**Q: `<main>` kya hota hai?**
A: Page ka asal/main content. Har page mein sirf **ek hi** `<main>` hona chahiye.

**Q: `<section>` kya hota hai?**
A: Content ka ek group jiska apna heading ho (jaise "Our Values" section).

**Q: `<article>` kya hota hai?**
A: Ek independent/standalone cheez — jo akele bhi samajh aa jaye, jaise ek destination card ya
ek team member ka info.

**Q: `<section>` aur `<article>` mein farq?**
A: Section = related content ka group (heading ke sath). Article = khud mukammal/independent
cheez. Jaise "Our Destinations" ek section hai, aur usme har destination ek article hai.

**Q: `<footer>` kya hota hai?**
A: Page ke sabse neeche — credit line, copyright, waghera.

**Q: `<address>` kya hota hai?**
A: Sirf contact info (email, phone, location) ke liye khaas tag.

---

## PART 3: Links aur Paths

**Q: `<a>` tag kya hai?**
A: Anchor tag — clickable link banata hai. `href` attribute batata hai kahan jaana hai.

**Q: `href` kya hai?**
A: Hypertext REFerence — batata hai link click karne par browser kahan jayega.

**Q: `src` aur `href` mein farq?**
A: `href` = kisi **doosri jagah ka link** (click karke jana). `src` = file ko **seedha yahin dikhana**
(jaise image, CSS).

**Q: Relative path kya hota hai?**
A: Ek file se doosri file tak ka raasta, current file ke hisaab se likha gaya. Full internet address
nahi, bas "yahan se wahan tak kaise jaana hai."

**Q: `index.html` se `pages/about.html` tak path kya likhoge?**
A: `pages/about.html` — seedha folder ka naam likho, andar jana hai.

**Q: `pages/about.html` se wapas Home (`index.html`) tak path?**
A: `../index.html` — `../` ka matlab hai "ek folder upar jao" (pages se bahar niklo, root mein aao).

**Q: `pages/about.html` se `pages/contact.html` tak path?**
A: Sirf `contact.html` — dono same folder mein hain (sibling files), koi `../` ya folder naam
nahi chahiye.

**Q: Agar path galat likh doon, kya hoga?**
A: "File not found" / "ERR_FILE_NOT_FOUND" error aayega — browser ko file milegi nahi.

---

## PART 4: Images

**Q: `<img>` tag ke zaroori attributes kaunse hain?**
A: `src` (image kahan hai), `alt` (image ka description), `width` aur `height` (size).

**Q: `alt` attribute kyun zaroori hai?**
A: Agar image load na ho, ya screen reader use ho raha ho, to `alt` text uski jagah dikhta/bolta
hai. Accessibility ke liye zaroori hai.

**Q: `width` aur `height` kyun set karte hain?**
A: Taake page load hote waqt browser ko pehle se pata ho image kitni jagah legi — content "jump"
nahi karta (layout stable rehta hai).

**Q: Tumhari image kahan se aayi?**
A: Kuch khud SVG code se banayi, kuch Pinterest se download ki (sources.txt mein likha hai).

---

## PART 5: Navigation Concepts (Lecture 3 ka kaam)

**Q: Tumhari site mein kitni nav bars hain har page pe?**
A: Do — Main navigation (Home, About, Destinations, Booking, Contact) aur Account navigation
(Login, Register), dono alag `<nav>` tags mein.

**Q: `aria-current="page"` kya karta hai?**
A: Batata hai user abhi kaunse page/link pe hai — browser aur screen reader dono ke liye.

**Q: Ye kahan lagta hai?**
A: Jo link us waqt khule hue page ko point kar raha ho. Jaise About page khula ho to "About"
link pe lagta hai.

**Q: Subpage pe (jaise Mission and Values) kahan lagta hai?**
A: Parent link ("About") pe NAHI lagta — sirf breadcrumb ke aakhri item pe lagta hai.

**Q: Breadcrumb kya hai?**
A: Ek chhota trail jo dikhata hai user kahan hai: "Home / About / Mission and Values" — har hissa
clickable hai wapas jaane ke liye.

---

## PART 6: Forms (Login, Register, Contact)

**Q: `<label>` aur `<input>` kaise connect hote hain?**
A: `label` ka `for` attribute aur `input` ka `id` attribute **match** karte hain:
`<label for="email">Email</label> <input id="email">`

**Q: `required` attribute kya karta hai?**
A: Browser ko khali field submit nahi karne deta — apna hi error message dikhata hai.

**Q: `type="email"` kya karta hai?**
A: Browser basic email format check karta hai (@ hona zaroori hai).

**Q: `type="password"` kya karta hai?**
A: Jo bhi type karo, dots/stars mein dikhta hai, asal characters chhup jate hain.

**Q: Kya ye forms kaam karte hain — account bante hain?**
A: Nahi, abhi ye sirf interface/structure hai. `action="#"` hai jo temporary hai. Real functionality
(account banana, data save karna) baad mein server/database se aayegi.

**Q: `<fieldset>` aur `<legend>` kya karte hain?**
A: `fieldset` related fields ko group karta hai (box banata hai), `legend` us group ka naam deta
hai (jaise "Your details").

**Q: `<select>` kya hai?**
A: Dropdown list — user ek option choose karta hai (jaise Topic: Destinations/Booking/Pricing).

**Q: Radio button aur checkbox mein farq?**
A: Radio buttons — sirf **ek** choose ho sakta hai group mein se. Checkbox — **multiple** choose
ho sakte hain, ya ek simple yes/no (jaise "I agree").

---

## PART 7: CSS Basics (Lecture 4)

**Q: CSS kya hai?**
A: Cascading Style Sheets — HTML ko **visually style** karne ki language (colors, spacing, fonts,
layout).

**Q: External CSS kya hai, aur kyun use ki?**
A: Ek alag `.css` file jo HTML se `<link>` tag se connect hoti hai. Isliye use ki kyunke ek hi file
se poori site (17 pages) control hoti hai — har page mein alag CSS nahi likhni padti.

**Q: CSS rule ka structure kya hota hai?**
A: `selector { property: value; }` — jaise `h1 { color: red; }`

**Q: Class selector kya hai?**
A: HTML mein `class="naam"` likha element select karta hai. CSS mein `.naam { }` se likha jata hai
(dot ke sath).

**Q: CSS Variables (`--peak`, `var()`) kya hain?**
A: Colors/values ko naam dete hain (`:root { --peak: #65000b; }`), phir `var(--peak)` se use karte
hain. Agar color change karna ho, ek hi jagah badlo, poori site update ho jati hai.

**Q: `:hover` kya hai?**
A: Pseudo-class — jab mouse kisi element ke upar ho (bina click kiye), style change karta hai.

---

## PART 8: Flexbox aur Grid (Assignment 3 — sabse naya)

**Q: Flexbox kya hai?**
A: `display: flex` — items ko ek **line (row ya column)** mein arrange karta hai, spacing aur
alignment easily control hoti hai.

**Q: Tumne Flexbox kahan use ki?**
A: Header mein (logo + nav bars ek row mein), nav links ke beech spacing ke liye, aur form ke
radio button rows mein.

**Q: Grid kya hai?**
A: `display: grid` — items ko **rows aur columns** dono mein arrange karta hai, jaise table lekin
flexible.

**Q: Tumne Grid kahan use ki?**
A: Jahan multiple cards (articles) ek sath hon — jaise Destinations ke 3 destination cards, Our
Team ke members — wo ab grid mein side-by-side dikhte hain.

**Q: Flexbox aur Grid mein farq?**
A: Flexbox = ek direction (row YA column). Grid = dono directions (rows AUR columns) ek sath.
Chhoti cheezein (nav, buttons) ke liye flexbox, bade layouts (cards grid) ke liye grid behtar hai.

**Q: `repeat(auto-fit, minmax(240px, 1fr))` ka matlab kya hai?**
A: Jitni jagah available ho utne columns fit kar do, har column kam se kam 240px chaudi ho — isse
layout responsive ban jata hai, chhoti screen pe khud columns kam ho jate hain.

---

## PART 9: Project-Specific (apne project ke baare mein)

**Q: Tumhare project mein kitni total files/pages hain?**
A: 17 HTML pages — 5 main (Home, About, Destinations, Booking, Contact), 10 subpages, 2 account
pages (Login, Register).

**Q: Tumhara target audience kaun hai?**
A: Pakistan mein log jo affordable guided trips chahte hain northern destinations ke liye (Hunza,
Murree, Naran).

**Q: Koi CSS/JS/Database abhi hai?**
A: CSS hai (Lecture 4 se), lekin JavaScript ya real database abhi nahi — wo future lectures mein
aayenge.

**Q: Forms data kahan jata hai abhi?**
A: Kahin nahi — ye sirf classroom demonstration hai, browser validation tak limited hai.

---

## PART 10: Agar Live Change Maange (practice zaroor karo)

1. Kisi page ka `<h1>` text turant change karna
2. `style.css` mein koi ek color (jaise `--peak`) change kar ke save karna, phir browser refresh
   karke dikhana poori site update ho gayi
3. Kisi image ka `alt` text change karna
4. Form ko khali submit kar ke required-field error dikhana
5. Browser window chhoti kar ke dikhana nav wrap hoti hai, cards stack hote hain

---

## SABSE IMPORTANT TIP

Agar koi sawal samajh na aaye ya bhool jao, **ghabrana mat** — bolo "ye concept mujhe thoda aur
clear karna hai" aur jo pata hai wo confidently bolo. Sir zyada tar ye dekhna chahte hain ke
tumne khud kaam kiya hai aur basic logic samajhti ho — perfect memorization nahi chahiye hoti.
