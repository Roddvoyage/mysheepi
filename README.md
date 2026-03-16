# MySheepi Shopify Theme Task

The page was built as part of a technical task for a recruiter.

---

## Overview

The landing page is composed of four custom sections:

- Hero
- How It Works
- Why You'll Love This
- FAQs

All content is driven by Shopify metafields using a consistent namespace.

The landing page is rendered using a custom **page template** and accessed via:

/pages/mysheepi-project

---

## Metafield Namespace

All metafields use the namespace:

custom

Values are accessed using:

page.metafields.custom.key

Example:

page.metafields.custom.hero_heading.value

---

## Sections

### Hero

Metafields used:

- custom.hero_heading
- custom.hero_subheading
- custom.hero_cta_label
- custom.hero_cta_link
- custom.hero_trust_line
- custom.hero_image
- custom.hero_image_mobile

Images are rendered using:

image_url  
image_tag

---

### How It Works

Metafields:

- custom.how_it_works_heading
- custom.how_it_works_cta_label
- custom.how_it_works_cta_link

Steps:

- custom.how_it_works_step_1_icon
- custom.how_it_works_step_1_title
- custom.how_it_works_step_1_text

- custom.how_it_works_step_2_icon
- custom.how_it_works_step_2_title
- custom.how_it_works_step_2_text

- custom.how_it_works_step_3_icon
- custom.how_it_works_step_3_title
- custom.how_it_works_step_3_text

- custom.how_it_works_step_4_icon
- custom.how_it_works_step_4_title
- custom.how_it_works_step_4_text

---

### Why You'll Love This

Metafields:

- custom.why_love_us_heading
- custom.why_love_us_cta_label
- custom.why_love_us_cta_link
- custom.why_love_us_image

Items:

- custom.why_love_us_item_1_icon
- custom.why_love_us_item_1_title
- custom.why_love_us_item_1_text

- custom.why_love_us_item_2_icon
- custom.why_love_us_item_2_title
- custom.why_love_us_item_2_text

- custom.why_love_us_item_3_icon
- custom.why_love_us_item_3_title
- custom.why_love_us_item_3_text

- custom.why_love_us_item_4_icon
- custom.why_love_us_item_4_title
- custom.why_love_us_item_4_text

---

### FAQs

Metafields:

- custom.faq_heading

Questions:

- custom.faq_1_question
- custom.faq_1_answer

- custom.faq_2_question
- custom.faq_2_answer

- custom.faq_3_question
- custom.faq_3_answer

- custom.faq_4_question
- custom.faq_4_answer

- custom.faq_5_question
- custom.faq_5_answer

---

## Fallbacks

Fallback values are implemented using the Liquid `default` filter to ensure the page renders even if a metafield is missing.

Example:

hero_heading | default: "Our product is the best product"
