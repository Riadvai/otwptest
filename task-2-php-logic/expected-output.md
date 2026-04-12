# Expected HTML Output Structure

Your PHP loop should produce HTML that looks like this structure for each doctor.
The exact styling doesn't matter — we're checking the **HTML structure and escaping**.

```html
<div class="doctor-card">
    <img src="https://placehold.co/640x565" alt="Dr. Sarah Mitchell">
    <h3>Dr. Sarah Mitchell</h3>
    <p class="specialty">Orthodontics &amp; Invisalign</p>
    <p class="experience">15+ Years</p>
    <p class="bio">Dr. Mitchell brings over 15 years of experience...</p>
    <ul class="credentials">
        <li>DDS — University of Michigan School of Dentistry</li>
        <li>Board Certified Orthodontist</li>
        <li>Invisalign Diamond Provider</li>
        <li>Member, American Association of Orthodontists</li>
    </ul>
</div>
```

## Key Things We Check:

1. **esc_html()** on all text output (name, specialty, bio, credentials)
2. **esc_url()** on the image src attribute
3. **esc_attr()** on the image alt attribute
4. Proper **foreach** loop — not hardcoded HTML
5. The `&` in "Orthodontics & Invisalign" should become `&amp;` (that's what esc_html does)
6. The apostrophe in "O'Brien" should be properly escaped
7. Credentials rendered as a proper `<ul>` with `<li>` items
