---
title: 'Accessibility Regression'
description:
  'An accessibility regression is a code change that makes a product harder to
  use with assistive technology, keyboard navigation, or other access needs.'
date: 2026-06-04
author: 'Gaetano'
---

# Accessibility Regression

## Definition

An accessibility regression is a change that reduces a product's usability for
people who rely on assistive technology, keyboard navigation, captions,
contrast, predictable focus, or semantic structure. The feature may still look
correct visually while becoming harder or impossible to use for some users.

## Context and Usage

Accessibility regressions often appear in small interface edits. A developer
can replace a labeled input with placeholder text, turn a text button into an
icon-only button without an accessible name, remove `aria-live` from a dynamic
status message, or break keyboard focus order while reorganizing a form.

For example, changing a reset button from `Reset filters` to a visual `x`
without `aria-label="Reset filters"` can remove the button's accessible name.
The visual design still appears clear to sighted users, but screen reader users
hear an ambiguous control.
