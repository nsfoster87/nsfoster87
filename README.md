# Hi, I'm Nate 👋

**Full-stack software engineer** building and scaling a production medical-imaging platform: the React viewer pathologists use, the Java and Python services behind it, and the AWS/Terraform infrastructure that ships it.

I like performance work driven by measurement, debugging problems that only show up in production, and reading third-party code until I understand it.

[LinkedIn](https://www.linkedin.com/in/nate-foster) · [Email](mailto:nate.s.foster@gmail.com)

---

## What I work on

- **Imaging backend:** a just-in-time DICOMweb server (Java / Spring Boot) that synthesizes whole-slide images on demand from S3, so there's no full PACS to run.
- **Clinical viewer:** an open-source research viewer turned into a production React app, with a rebuilt component tree, routing, and an extended `dicomweb-client`.
- **Data pipelines:** PNG-to-DICOM ETL in Python (pydicom, NumPy, Pillow) that writes valid whole-slide files with zoom pyramids.
- **Platform:** Terraform, GitHub Actions, Docker, ECS, and OpenTelemetry/Grafana observability.

## Results I'm proud of

| Problem | Result | How |
|---|---|---|
| Study load time | **~34 s → ~25 ms** | Profiled a 34 MB metadata parse, showed a parser swap wouldn't help, and worked cross-team to shrink the payload to 3.4 MB |
| Worklist load | **10–60 s → ~100 ms** | Moved search, sort, and pagination server-side for hundreds of thousands of studies |
| Panorama load | **17.4 s → 8.2 s** | Found a cache that was switched off in every environment, causing 1,000+ redundant DynamoDB lookups |
| Missing tiles in production | **Root-caused** | Traced a prod-only bug to a non-sticky load balancer in front of in-memory state |

## Tech I use

![Java](https://skillicons.dev/icons?i=java,spring,react,ts,js,python&perline=6)
![AWS](https://skillicons.dev/icons?i=aws,terraform,docker,githubactions,nginx,redis&perline=6)
![Tools](https://skillicons.dev/icons?i=nodejs,grafana,prometheus,bash,git,vite&perline=6)

DICOM / DICOMweb · OpenLayers · DynamoDB · CloudFront + Lambda@Edge · OpenTelemetry

## Background

I came to software through a 1000+ hour immersive program ([Hack Reactor](https://www.hackreactor.com/)) after a career in performing arts. I stayed on as a resident and mentored students in JavaScript, React, and Node.js. I still enjoy helping newer engineers.

## Get in touch

I'm open to full-stack roles. The best way to reach me is [LinkedIn](https://www.linkedin.com/in/nate-foster) or [nate.s.foster@gmail.com](mailto:nate.s.foster@gmail.com).
