# Accessible Pictogram Communication System

**Role:** Instructional designer and developer · **Context:** Special education classroom, junior high level, Utah
**Frameworks:** WCAG 2.1 · Universal Design for Learning (CAST) · AAC

---

> **Note on the case profile:** "Ana" is an illustrative composite profile used to ground the design decisions in a concrete set of needs. She is not an identifiable student, and no school is named.

---

## The challenge

A special education classroom used an adapted PECS pictogram card system every single day: for every
transition, every choice, every functional communication exchange. It was the highest-impact material in
the room. Without it, functional communication for students with multiple disabilities collapsed.

It had never been formally evaluated for accessibility, because it looked simple and therefore was assumed
to be accessible. That assumption is the failure mode this project exists to correct. A prior audit
(project 02) found five critical failures across the eight WCAG criteria evaluated: no alternative text on
any pictogram, no auditory version, no keyboard or assistive-technology access in the static PDF
distributed to families, and no semantic structure in the digital document.

The material worked visually for the teacher. It did not work for the student who needed it most.

## The approach

Rather than describing improvements, I built the replacement. The design brief was to satisfy all four
WCAG 2.1 principles (perceivable, operable, understandable, robust) while applying UDL's three
principles of representation, action and expression, and engagement.

Every design decision traced back to a specific failure in the audit. Constraints were deliberate: open
and free technologies only, no software installation, no internet connection required after download, and
runnable in any modern browser on any device. Pedagogical sustainability was a requirement, not a
preference. A resource a school cannot afford to maintain is a resource that stops being used.

## What I built

An interactive HTML communication system organizing 16 pictograms into four colour-coded categories:
actions, objects, people, and emotions.

- **Original SVG pictograms** rather than raster images, so they stay sharp at any magnification, resolving
  a limitation identified in the audit
- **Descriptive alternative text** on every pictogram via `aria-label`, describing the object, the action
  shown, and the category, for screen reader users
- **Speech synthesis** on card selection at 0.85x rate, giving an auditory channel alongside the visual one
- **AAC message panel** that accumulates selected words, builds a full message, and speaks it aloud with a
  single button, for students with severe motor limitations
- **High contrast mode** with black background and yellow text, exceeding a 7:1 contrast ratio
- **Adjustable text sizing** from 12 to 28 points without layout overflow
- **Full keyboard operability** and assistive technology compatibility, replacing a static PDF that
  supported neither

## What this demonstrates

The full instructional design cycle carried through to a working artifact: audit, diagnosis, design
rationale, build, and compliance mapping. It also shows accessibility handled as a design constraint from
the first decision rather than a remediation pass at the end, which is the difference between a resource
that technically passes and one a student can actually use.

**Full documentation (Spanish):**
[01-accessible-pictogram-communication-system.pdf](01-accessible-pictogram-communication-system.pdf) · 15 pages
