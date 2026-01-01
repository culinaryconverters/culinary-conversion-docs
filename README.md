# culinary-conversion-docs

# Precision Baking: Ingredient Density Database & Conversion Logic

[![Website Status](https://img.shields.io/website?url=https%3A%2F%2Fwww.culinaryconverters.com&label=Live%20Tool)](https://www.culinaryconverters.com)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Tech Stack](https://img.shields.io/badge/Built%20With-Next.js%2014-black)](https://nextjs.org/)
[![Lighthouse Score](https://img.shields.io/badge/Lighthouse-100%25-brightgreen)](https://www.culinaryconverters.com)

## 📖 Introduction

This repository documents the scientific methodology and density data used in the **[Culinary Converters](https://www.culinaryconverters.com)** project. 

While most online converters use generic estimations (e.g., treating all flours as the same weight), this project aims to solve the "Volume vs. Mass" discrepancy in professional baking by utilizing specific density values ($g/ml$) for over 500+ ingredients.

> **Live Tool:** Access the production-ready calculator at **[www.culinaryconverters.com](https://www.culinaryconverters.com)**.

---

## 🧪 The "Cup Problem" (The Science)

In the US Customary System, volume measurements (Cups, Tablespoons) are notoriously inaccurate for dry ingredients due to variable density and compression.

**The Physics:**
$$Mass (g) = Volume (ml) \times Density (g/ml)$$

**Real-world Variance Data:**
A standard "1 Cup" volume (approx. 236ml) yields drastically different weights depending on the ingredient's physical properties:

| Ingredient | Density (g/ml) | Weight of 1 Cup |
| :--- | :---: | :---: |
| **Water** | 1.00 | ~236g |
| **All-Purpose Flour (Sifted)** | 0.46 | ~109g |
| **All-Purpose Flour (Packed)** | 0.65 | ~155g |
| **Granulated Sugar** | 0.85 | ~200g |
| **Honey** | 1.42 | ~335g |

*Data source: USDA FoodData Central and independent density testing used in the [Culinary Converters Algorithm](https://www.culinaryconverters.com).*

---

## ⚡ Tech Stack & Performance

This project was built to demonstrate how a scientific tool can achieve **100% Performance & Accessibility** scores on Google Lighthouse.

* **Framework:** [Next.js 14](https://nextjs.org/) (App Router)
* **Styling:** [Tailwind CSS](https://tailwindcss.com/)
* **Language:** TypeScript
* **Deployment:** Vercel Global Edge Network
* **Analytics:** GA4 (Privacy-focused implementation)

### Accessibility First
The project adheres to WCAG 2.1 AA standards, ensuring that semantic HTML and ARIA labels make the conversion engine accessible to screen readers.

---

## 🛠️ Usage

This repository serves as a reference for the density logic. To perform actual conversions:

1.  Navigate to the **[Official Calculator](https://www.culinaryconverters.com)**.
2.  Select your ingredient (Database includes specific variations like *"Almond Flour, Blanched"* vs *"Almond Meal"*).
3.  Enter the volume (Cups, Tbsp, Tsp, etc.).
4.  Get the precise weight in Grams or Ounces.

---

## 🤝 Contributing

We welcome contributions to the density dataset! If you have verified weight data for obscure ingredients, please open an Issue or Pull Request.

## 📄 License

This documentation is open-source under the [MIT License](LICENSE). 
The core application logic and branding are copyright of [Culinary Converters](https://www.culinaryconverters.com).

## 📚 Read the Story
- **The Tech Stack:** [How I built this with Next.js 14 (Dev.to)](https://dev.to/trinc4/how-i-built-a-global-saas-with-nextjs-14-and-achieved-a-100-lighthouse-score-2nm6)
- **The Science:** [Why "Cups" are broken & Density matters (Medium)](https://medium.com/@culinaryconverter/why-your-1-cup-of-flour-is-ruining-your-cake-the-science-of-density-303d09f80f9d)
  **TABNEWS:** [TabNews POST](https://www.tabnews.com.br/trinc4/engenharia-de-performance-como-atingi-100-100-no-lighthouse-gerando-500-paginas-estaticas-com-next-js-14)
  **LINKEDIN POST:** [Linkedin POST](https://www.linkedin.com/pulse/from-local-legacy-global-saas-achieving-perfect-seo-14-converters-eysde/?trackingId=mXQqUkGZw1qfRf2YzdlS1g%3D%3D)
  
---
*Maintained by the Culinary Converters Engineering Team.*
