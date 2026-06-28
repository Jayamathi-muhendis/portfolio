# Jayamathi M — Data Engineer Portfolio

A production-ready personal portfolio site built with React, TypeScript, Tailwind CSS, and Vite. Deploys cleanly to Vercel.

## Folder structure

```
portfolio/
├── public/
│   └── resume-placeholder.txt   # replace with your real resume.pdf
├── src/
│   ├── components/
│   │   ├── Nav.tsx
│   │   ├── Hero.tsx
│   │   ├── PipelineDiagram.tsx  # animated signature visual
│   │   ├── ScrollFlowLine.tsx   # scroll-progress signature element
│   │   ├── Projects.tsx
│   │   ├── ProjectCard.tsx
│   │   ├── Experience.tsx
│   │   ├── Skills.tsx
│   │   ├── Contact.tsx
│   │   └── Footer.tsx
│   ├── data/
│   │   ├── projects.ts          # edit your project content here
│   │   ├── experience.ts
│   │   └── skills.ts
│   ├── App.tsx
│   ├── main.tsx
│   └── index.css
├── index.html
├── package.json
├── tailwind.config.js
├── vite.config.ts
└── vercel.json
```

## Setup (local)

Requires Node.js 18+.

```bash
npm install
npm run dev       # http://localhost:5173
```

Build for production:

```bash
npm run build
npm run preview
```

## Editing content

All real content lives in `src/data/*.ts` — no need to touch component code to update projects, experience, or skills. Anything wrapped as a placeholder (search for `[Add` or `[Replace`) is clearly marked for you to fill in with real metrics or links — nothing in the data files is invented.

Replace `public/resume-placeholder.txt` with your actual `resume.pdf` (same filename) so the "Resume ↓" button in the nav works.

## Deploying to Vercel

1. Push this folder to a GitHub repo.
2. Go to [vercel.com/new](https://vercel.com/new) and import the repo.
3. Vercel auto-detects Vite — framework preset: **Vite**, build command `npm run build`, output directory `dist`. Leave these as default.
4. Click **Deploy**. You'll get a live URL in ~60 seconds.
5. (Optional) Add a custom domain under Project → Settings → Domains.

No environment variables are required for the current version.

## Suggested content for Resume, LinkedIn, and GitHub

**Resume headline:** Data Engineer | ELT Pipelines, dbt, AWS | Healthcare & Retail Data Platforms

**LinkedIn "About" draft:**
> Data Engineer with 3+ years building ELT pipelines, data warehouses, and automated data-quality systems across healthcare and retail. Currently building HIPAA-sensitive EMR pipelines at Clustrex Data, processing 200K+ records/month across 23+ clinical data sections, with dbt-based incremental loading and a 12-notebook automated QA suite running on AWS ECS. Portfolio: [your-portfolio-url]

**LinkedIn featured section:** Pin your portfolio link and resume PDF.

**GitHub profile README suggestions:**
- Pin 2–3 repos that demonstrate ETL/ELT code, dbt models, or data quality testing (even small personal projects count — e.g., a sample dbt project with watermark logic, or a Papermill-based notebook test runner).
- Add a short bio matching your LinkedIn About.
- Link your portfolio site in the GitHub profile bio field.

## Future enhancements

- **Case studies:** turn the McKesson project into a deeper case-study page (problem → architecture diagram → decisions → outcome) once you have permission to share more detail or fully anonymized specifics.
- **Blog:** a `/writing` route with posts on dbt patterns, data reconciliation strategies, or Papermill testing — strong signal for hiring managers and freelance clients.
- **Certifications:** add a row of cert badges (e.g., AWS, dbt) once earned.
- **Testimonials:** a short quote section once you have manager/colleague references.
- **Dark/light toggle:** currently dark-only by design; could add a light theme if desired.
- **Analytics:** add Vercel Analytics or Plausible to track recruiter traffic.

## Notes on content accuracy

All project bullets and the experience timeline are derived directly from your resume. The one placeholder (`[Add a QA defect-catch-rate or pipeline-runtime metric here...]`) and the GitHub URL placeholder are intentionally left for you to fill in with real numbers/links rather than invented ones.
