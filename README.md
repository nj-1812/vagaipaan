<div align="center">

# வகைப்பான் (Vakaippaan)

**AI-Powered Reverse Logistics Multi-Tier Classifier**

*Intelligent return processing for faster, cheaper, and sustainable reverse supply chains.*

[![Status](https://img.shields.io/badge/status-under%20development-yellow)]()
[![Team](https://img.shields.io/badge/team-Epsilon-blue)]()
[![License](https://img.shields.io/badge/license-MIT-green)]()

</div>

---

## Overview

E-commerce platforms process millions of product returns every year. The current standard — manual inspection — is slow, expensive, inconsistent across reviewers, and frequently leads to perfectly usable products being discarded.

**Vakaippaan** removes that bottleneck. It uses AI to inspect returned items, assess their condition, flag potential fraud, and automatically route each item to the most economically and environmentally sound outcome — without a human ever having to manually sort it.

---

## The Problem

| Pain Point | Impact |
|---|---|
| Manual inspection | Slow turnaround, high labor cost |
| Inconsistent grading | Same product, different verdicts across reviewers |
| Return fraud | Revenue leakage from item-swap and wardrobing scams |
| Poor routing decisions | Usable inventory ends up liquidated or landfilled |

---

## The Solution

Vakaippaan ingests images (and supporting documentation) of a returned item and runs it through an automated pipeline that:

1. **Inspects** the product visually for damage, wear, and completeness
2. **Detects fraud signals** by cross-referencing claims against visual evidence
3. **Classifies** the item's condition into a defined tier
4. **Routes** the item automatically to the optimal disposition channel

### Routing Outcomes

- 🟢 **Restocking** — item is in original, sellable condition
- 🟡 **Open-Box Sale** — minor cosmetic wear, sold at a discount
- 🔧 **Refurbishment** — functional but needs repair or reconditioning
- 📦 **Liquidation** — bulk resale through secondary channels
- ♻️ **Recycling** — material recovery for non-resalable items
- ⚠️ **Safe Disposal** — items unsuitable for any resale or recovery path

---

## System Architecture

```
Customer → Image Upload → AI Inspection → Fraud Detection → Classification → Routing Decision
```

### Frontend
- React + TypeScript
- Tailwind CSS
- AWS Amplify

### Backend
- AWS Lambda
- Amazon API Gateway

### AI & Machine Learning
- Amazon Rekognition — visual condition inspection
- Amazon Textract — document and label extraction
- Amazon Bedrock — classification and reasoning layer

### Data & Storage
- Amazon S3 — image and document storage
- Amazon DynamoDB — metadata and decision records

---

## Project Status

🚧 **Under active development.** Core architecture is defined; pipeline integration and model tuning are in progress.

---

<div align="center">

*Built to make reverse logistics smarter, faster, and more sustainable.*

</div>
