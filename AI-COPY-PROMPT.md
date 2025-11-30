# AI Copy Generation Prompt Template

Copy this entire prompt and paste it into ChatGPT, Claude, or any AI assistant. Fill in the `[CLIENT ANSWERS]` section with the responses from your client intake form.

---

## THE PROMPT:

```
You are an expert conversion copywriter specializing in service-based business websites.

I need you to write compelling, benefit-focused copy for a one-page website template. The copy should be clear, action-oriented, and speak directly to the customer's pain points and desires.

Write copy that:
- Grabs attention immediately
- Focuses on benefits, not just features
- Uses simple, direct language
- Creates urgency without being pushy
- Builds trust and credibility
- Has a strong call-to-action

---

CLIENT INFORMATION:
[Paste the client intake answers here]

Business Name: [Business Name]
What They Do: [Description]
Service 1: [Service 1]
Service 2: [Service 2]
Service 3: [Service 3]
Phone: [Phone Number]
Additional Notes: [Any special requests, colors, timeline, etc.]

---

GENERATE THE FOLLOWING SECTIONS:

1. **HERO HEADLINE** (5-10 words, punchy, benefit-driven)
   - Should immediately communicate the main benefit or transformation
   - Make it bold and attention-grabbing

2. **HERO SUBTEXT** (1-2 sentences, 20-30 words)
   - Expand on the headline
   - Address a pain point or desire
   - Include a soft call-to-action hint

3. **THE PROBLEM** (2-3 sentences, focus on customer pain points)
   - What frustration/challenge do customers face?
   - Why is it hard to find a good solution?
   - Make them feel understood

4. **OUR SOLUTION** (2-3 sentences, position the business as the answer)
   - How does this business solve the problem differently?
   - What makes them uniquely qualified?
   - Build confidence and trust

5. **SERVICE DESCRIPTIONS** (For each of the 3 services)
   - Service 1: [Name] - (1 sentence description, focus on the outcome/benefit)
   - Service 2: [Name] - (1 sentence description, focus on the outcome/benefit)
   - Service 3: [Name] - (1 sentence description, focus on the outcome/benefit)

6. **CTA HEADLINE** (4-8 words, action-oriented)
   - What should the customer do next?
   - Create urgency or highlight ease

7. **CTA SUBTEXT** (1 sentence, remove friction)
   - Make it feel easy and risk-free
   - Mention response time or value

---

FORMAT YOUR RESPONSE EXACTLY LIKE THIS:

## GENERATED COPY

**Hero Headline:**
[Your headline here]

**Hero Subtext:**
[Your subtext here]

**The Problem:**
[Problem copy here]

**Our Solution:**
[Solution copy here]

**Service 1 - [Name]:**
[Description]

**Service 2 - [Name]:**
[Description]

**Service 3 - [Name]:**
[Description]

**CTA Headline:**
[CTA headline here]

**CTA Subtext:**
[CTA subtext here]

---

ADDITIONAL INSTRUCTIONS:
- Write in a confident, professional tone
- Avoid jargon or overly technical language
- Focus on what the customer GETS, not what the business DOES
- Use active voice
- Be specific where possible (use details from client info)
- Keep it concise and scannable
```

---

## EXAMPLE OUTPUT

Here's what you should expect to receive back from the AI:

```
## GENERATED COPY

**Hero Headline:**
We Solve Your Toughest Landscaping Problems Fast

**Hero Subtext:**
The job others won't touch? That's what we do best. Overgrown lots,
steep terrain, emergency cleanup—get your free quote in minutes.

**The Problem:**
Most landscaping companies turn down difficult jobs. Overgrown yards,
challenging terrain, urgent storm damage—if it's hard, they're not
interested. You're left searching for someone willing to do the work.

**Our Solution:**
We specialize in exactly those tough jobs nobody else wants. Fast
response times, fair pricing, and we show up ready to handle whatever
you've got. No job too big, too messy, or too complicated.

**Service 1 - Overgrown Lot Clearing:**
Reclaim abandoned properties and neglected spaces—brush removal,
debris hauling, and total lot transformation.

**Service 2 - Difficult Terrain Work:**
We handle steep slopes, tight access, and hard-to-reach areas other
companies can't tackle safely.

**Service 3 - Emergency Storm Cleanup:**
Fallen trees, storm damage, urgent cleanups—we respond fast when you
need help immediately.

**CTA Headline:**
Send a Photo, Get Your Free Quote

**CTA Subtext:**
Takes 60 seconds. We'll text you back with a price today.
```

---

## HOW TO USE THE OUTPUT

1. **Copy each section** from the AI response
2. **Open your template site** (`index.html`)
3. **Find and replace** the placeholder text with AI-generated copy:

| Template Location | AI Section | HTML ID |
|------------------|------------|---------|
| Main headline | Hero Headline | `id="heroHeadline"` |
| Subtitle | Hero Subtext | `id="heroSubtext"` |
| Problem section | The Problem | `id="problemText"` |
| Solution section | Our Solution | `id="solutionText"` |
| Service 1 | Service 1 | `id="service1"` |
| Service 2 | Service 2 | `id="service2"` |
| Service 3 | Service 3 | `id="service3"` |
| CTA button area | CTA Headline & Subtext | In the CTA section |
| Nav/Footer | Business Name | `id="navBrand"` |

---

## TIPS FOR BETTER AI OUTPUT

### If the copy feels too generic:
Add to the prompt: "Make the copy more specific to [industry] and use concrete examples from the client info."

### If it's too salesy:
Add: "Tone down the hype. Write in a more straightforward, honest voice."

### If you want different variations:
Add: "Give me 3 different versions of the hero headline to choose from."

### If the client has brand personality notes:
Add them to the prompt: "The brand voice should be [friendly/professional/edgy/luxury/etc.]"

---

## ADVANCED: Batch Processing

If you're doing multiple clients at once, you can ask the AI:

```
I have 3 clients. I'll give you each client's info, and you generate
all website copy for each one. Label them clearly as Client 1, Client 2, Client 3.

[Paste all 3 client intake forms]
```

This lets you knock out multiple websites in one go!

---

**Save this prompt template and use it for every new client. Tweak as needed for different industries or brand voices.** 🚀
