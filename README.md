# SEO & AI Search Izvještaj  

# 1. Uvod

Ovaj dokument predstavlja sveobuhvatan izvještaj o trenutnom stanju SEO performansi i AI Search spremnosti web stranice **NelsonKB.com**. Cilj analize je identifikovati faktore koji utiču na organsku vidljivost, performanse u Google pretrazi i pozicioniranje unutar novih AI-driven pretraživača, te dati jasne preporuke za poboljšanje.

Moderne AI pretrage (Google SGE, Bing Copilot, ChatGPT Search, Perplexity) oslanjaju se na:

- tehničke performanse web stranice (Core Web Vitals)
- kvalitet i strukturu sadržaja
- kvalitet product opisa i blog članaka
- E-E-A-T signale (expertise, authority, trust)
- precizno definisane schema.org podatke
- jasnu taksonomiju kategorija i proizvoda

Izvještaj obuhvata:

- tehničku SEO analizu  
- analizu indeksabilnosti i strukture  
- analizu product i blog stranica  
- AI Search readiness pregled  
- preporučene schema.org implementacije  
- prioritete za optimizaciju  


# 2. Trenutna analiza web stranice

## 2.1. Tehnički SEO pregled

### Core Web Vitals – Mobile

Realni podaci pokazuju prolazne CWV metrike, ali Lighthouse simulacija ukazuje na ključne probleme koji mogu negativno uticati na SEO i AI Search vidljivost.

#### Glavni nalazi

- LCP spor (6.6 s u Lighthouse; 1.4 s u Field Data)  
- CLS odličan (0.0 – 0.001)  
- Nestabilan TTFB (~1.0 s)  
- Velik JavaScript bundle (TrustIndex, WP skripte)  
- Render-blocking CSS  
- Fontovi povećavaju mrežni payload  
- Veoma velika DOM struktura (≈ 2900 elemenata)

#### Uticaj na AI Search  
Mobilna sporost direktno utiče na vidljivost u Google SGE i drugim AI sistemima.


### Core Web Vitals – Desktop

Desktop performanse su stabilne, ali postoji prostor za značajna poboljšanja.

#### Glavni nalazi

- LCP: 1.5–1.9 s  
- CLS: 0.04  
- TTFB: 1.4 s  
- Render-blocking CSS (~350 ms)  
- Ukupni payload: ~1.7 MB  
- Third-party skripte uzrokuju reflows  
- Veliki DOM (~3000 elemenata)


### Fetch & Render analiza (10 URL-ova)

- Svi URL-ovi vraćaju 200 OK  
- Googlebot-Mobile renderuje sadržaj u potpunosti  
- Nema blokiranih resursa  
- DOM je identičan korisničkom prikazu  

**Bot vidi isto što i korisnik**, što je važno za AI Search sisteme.


## 2.2. Sitemap i Robots.txt

### Robots.txt  
- Pravilno konfigurisan  
- Sitemap ispravno naveden  
- Nema blokiranja SEO-kritičnih direktorija  

### Sitemap Index  
- 31 sitemap (products, posts, pages, categories, cities)  
- Ažurira se automatski  
- URL-ovi su SEO-friendly  


## 2.3. Indexabilnost

- Sve analizirane stranice su indexable  
- Nema `noindex` tagova  
- Status kôd 200  
- Googlebot-Mobile allowed  
- Rendering uspješan  


## 2.4. Status i Redirect analiza

- Nema redirect lanaca  
- Nema 404 grešaka  
- Nema broken linkova  
- Sve testirane stranice vraćaju 200  


## 2.6. Off-page analiza

### Backlink profil  
- 116,000+ backlinkova  
- 1,300+ linking domena  
- 99% dofollow linkova  
- Domain Rating: 42  

### Prednosti  
- Visok domain authority  
- Linkovi sa kvalitetnih magazina i portala  

### Slabosti  
- Preveliki fokus linkovanja na homepage  
- Nedovoljno deep-linkova ka produktima i blogovima  


# 2.5. On-page analiza


# Product Page Analiza

## Elemente koji postoje (potvrđeno)

- H1 naslov proizvoda  
- Cijena  
- SKU  
- Add to Cart dugme  
- Galerija slika  
- Opis proizvoda  
- Tabovi (Description / Additional Info / Reviews)  
- Interno linkanje (Related Products)  
- Buyer reviews  
- Globalna FAQ sekcija  
- Optimizovani alt tagovi  
- Video sadržaj (How to Assemble)


## Elementi koji nedostaju

- Semantički bogat opis (H2 sekcije, benefiti, liste)  
- E-E-A-T elementi (autorstvo, stručne reference)  
- Proširena Product schema:
  - aggregateRating  
  - review  
  - material  
  - color  
  - additionalProperty  
  - shippingDetails  
  - hasMerchantReturnPolicy  


# Blog Page Analiza

## Elemente koji postoje

- Naslov + uvodni tekst  
- Featured image  
- Interni linkovi  
- SEO-friendly URL  
- Globalna Organization / LocalBusiness schema  
- Vidljiv autor i biografija  


## Elementi koji nedostaju

- Article schema  
- E-E-A-T markup (author schema, reviewedBy, publisher logo)  
- FAQ sekcija  
- Table of Contents  
- VideoObject schema  


# 3. Google Rich Results analiza

## Product Page

- Osnovna Product schema postoji  
- Nedostaju prošireni atributi:
  - aggregateRating  
  - review  
  - material, color  
  - dimensions (additionalProperty)  
  - return policy  
  - shipping details  

## Blog Page

- Detektovana Organization schema  
- Nedostaju:
  - Article schema  
  - FAQPage schema  
  - VideoObject schema  


# 4. AI Search analiza

## Prednosti

- Jak domen i autoritet  
- Kompletna indeksabilnost  
- Dobra osnovna struktura  
- Kvalitetna taksonomija  
- Velika količina sadržaja  

## Ključne slabosti

- Mobilni LCP i render-blocking CSS  
- Nedostatak dubokih product opisa  
- Nedovoljno E-E-A-T signala  
- Minimalna Product schema  
- Nedostatak Article, FAQPage i VideoObject schema  
- Blog sadržaj nije semantički strukturiran  


# 5. Schema.org — Preporuke

## 5.1. Šta je Schema Markup?

Schema markup je JSON-LD struktura koja omogućava Google-u, SGE-u, Copilotu i ChatGPT-u da razumiju sadržaj stranice, identifikuju ključne informacije i prikazuju rich rezultate.


## 5.2. Zašto je schema važna?

### 1. Pojavljivanje u rich rezultatima  
Povećava CTR i vidljivost u SERP-u.

### 2. AI Search koristi schemu kao primarni izvor informacija  
SGE i ChatGPT direktno čitaju product, article i FAQ podatke.

### 3. Poboljšava semantičko razumijevanje  
Omogućava bolje rangiranje za buyer-intent i info-intent upite.


## 5.3. Preporučene schema vrste

- Product  
- FAQPage  
- Article  
- BreadcrumbList  
- VideoObject  


## 5.4. Primjeri Schema Markupa

### Product Schema

```json
{
  "@context": "https://schema.org/",
  "@type": "Product",
  "name": "Gray Shaker 09 Wall Cabinet",
  "image": [
    "IMAGE_URL_1",
    "IMAGE_URL_2"
  ],
  "description": "Full expanded product description...",
  "sku": "WS09",
  "brand": {
    "@type": "Brand",
    "name": "Nelson Cabinetry"
  },
  "material": "Solid wood frame, MDF panels",
  "color": "Gray",
  "offers": {
    "@type": "Offer",
    "priceCurrency": "USD",
    "price": "149.00",
    "availability": "https://schema.org/InStock"
  }
}
```
### FAQPage Schema — primjer

```json
{
  "@context": "https://schema.org",
  "@type": "FAQPage",
  "mainEntity": [
    {
      "@type": "Question",
      "name": "Are Shaker cabinets durable?",
      "acceptedAnswer": {
        "@type": "Answer",
        "text": "Yes, Shaker cabinets are known for durability because..."
      }
    }
  ]
}
```

### Article Schema — primjer

```json
{
  "@context": "https://schema.org",
  "@type": "Article",
  "headline": "Example Blog Title",
  "author": {
    "@type": "Person",
    "name": "Nelson Cabinetry Team"
  },
  "image": "IMAGE_URL",
  "datePublished": "2025-01-01",
  "dateModified": "2025-01-01",
  "publisher": {
    "@type": "Organization",
    "name": "Nelson Cabinetry",
    "logo": {
      "@type": "ImageObject",
      "url": "https://nelsonkb.com/wp-content/uploads/2019/07/logo_2x.png"
    }
  }
}
```

### 5.5. Implementacija u WordPress-u

**Rank Math (preporučeno)**  
- Automatski dodaje Product, Article, BreadcrumbList, WebPage, Organization  
- Preporuka: uključiti “Advanced Schema” i dodati custom fields za material, dimensions, color  

**Yoast SEO**  
- Automatski dodaje osnovni schema markup  
- FAQ block dodaje FAQPage schemu  
- Article schema se aktivira kada postoji autor  

**Ručna implementacija**  
- Code Snippets plugin  
- functions.php  
- Custom HTML block u Gutenberg editoru  

### 5.6. Testiranje Schema Markupa

- Google Rich Results Test  
- Schema.org Validator  
- Search Console (Product/FAQ/Article izvještaji)  
- Screaming Frog – Structured Data Extraction  

### 6. Preporuke za klasični SEO

- Kompresovati hero slike  
- Eliminisati render-blocking CSS  
- Smanjiti JS bundle  
- Optimizovati alt tagove  
- Proširiti product opise  
- Ojačati interno linkanje  
- Unaprijediti meta opise  
- Kreirati category content hubove  

### 7. Preporuke za AI-driven SEO

- Dodati duboko strukturirane product opise  
- Implementirati Article i FAQPage schema  
- Dodati VideoObject schema na sve video materijale  
- Pojačati E-E-A-T signale (autor, ekspert review, brand trust)  
- Upotpuniti Product schema sa svim dostupnim atributima  
- Kreirati buyer-intent sadržaj  

### 8. Zaključak

NelsonKB.com posjeduje snažnu SEO osnovu i visok domain authority.  
Da bi se poboljšala vidljivost u AI-driven pretraživačima potrebno je unaprijediti mobilne performanse, semantičku strukturu product i blog sadržaja, advanced schema markup, E-E-A-T signale i interni content cluster.

Očekivani rezultati uključuju bolju SGE/Copilot/ChatGPT vidljivost, veći CTR, bolje rangiranje i rast organskog saobraćaja.
