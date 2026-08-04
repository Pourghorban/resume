# Resume — MohammadReza Pourghorban

LaTeX sources for my resume, in Persian and English. Built with XeLaTeX.

**Latest PDFs:** [English](https://github.com/Pourghorban/resume/releases/latest/download/resume-en.pdf) · [Persian](https://github.com/Pourghorban/resume/releases/latest/download/resume-fa.pdf)

## Structure

| File | Description |
|---|---|
| `resume-en.tex` | English version — single-column, ATS-friendly, EB Garamond |
| `resume-fa.tex` | Persian version — RTL via `xepersian`, Vazirmatn |
| `fonts/` | Bundled Vazirmatn (OFL 1.1) |

## Building

Requires XeLaTeX (TeX Live or MiKTeX) and `poppler-utils` for verification.

```bash
xelatex -interaction=nonstopmode resume-en.tex
xelatex -interaction=nonstopmode resume-en.tex   # second pass
```

Both documents compile in two passes. The Persian version needs
`xepersian`, `bidi`, and the bundled fonts; the English version needs
`titlesec`, `enumitem`, and `microtype`.

## Notes on the Persian version

Persian is a cursive script, so letter-spacing breaks glyph joining —
the typographic emphasis in the Persian document comes from size and
weight instead. Text extraction from the Persian PDF is unreliable
(a known Poppler limitation with complex Arabic-script shaping), so the
English version is the one intended for automated parsing.

## License

Template and build configuration: MIT (see `LICENSE`).
Resume content — text, personal details, employment history — is not
covered by that license and may not be reused.
Bundled fonts are under their own licenses; see `fonts/README.md`.

---

<div dir="rtl">

## دربارهٔ این ریپو

سورس لاتک رزومهٔ من است، به فارسی و انگلیسی، ساخته‌شده با XeLaTeX. نسخهٔ فارسی راست‌به‌چپ است و از `xepersian` و فونت وزیرمتن استفاده می‌کند؛ نسخهٔ انگلیسی تک‌ستونه و سازگار با سامانه‌های ATS است. برای کامپایل به XeLaTeX نیاز دارید (TeX Live یا MiKTeX)؛ هر دو سند در دو مرحله کامپایل می‌شوند. قالب و تنظیمات ساخت تحت مجوز MIT است، اما متن و اطلاعات شخصی رزومه مشمول آن نیست. فونت‌های همراه تحت مجوز OFL 1.1 هستند (جزئیات در `fonts/README.md`).

</div>
