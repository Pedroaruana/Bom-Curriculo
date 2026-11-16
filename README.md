# Bom Currículo - ATS Resume Builder

> Este é o meu fork do projeto Bom Currículo (open source). O repositório original saiu do ar, então deixei aqui uma cópia do histórico com as minhas contribuições.
>
> O que eu fiz no projeto:
> - Tela de confirmação dos dados antes de gerar o currículo, em React e TypeScript (#124, #247)
> - Configuração de testes do frontend com Vitest e Testing Library (#141)
> - Bot em Python que recebe CV, LinkedIn, GitHub e habilidades pra gerar o currículo com IA (#144) e CI dos testes do bot (#145)
> - Testes dos endpoints da API (#183)
>
> Meus commits estão nas branches `upstream-backup` e `backup-prs-antigos`.

https://bomcurriculo.tech

## UNDER CONSTRUCTION

Build ATS-friendly resumes using AI.

## About

Bom Currículo is an open-source project that generates professional resumes optimized for Applicant Tracking Systems (ATS).

The system can use multiple optional sources of information, including:

- Current resume
- LinkedIn Profile (PDF export)
- GitHub profile
- Portfolio
- Personal information
- Target job description

The user does not need to provide every source. The only requirement is enough information to generate a resume.

## Features

- LinkedIn profile analysis
- GitHub profile analysis
- Portfolio analysis
- Job description matching
- ATS-friendly resume generation
- Resume optimization

## Screen prototype

An initial interface prototype was also developed in Figma to validate the user experience, feature organization, and the platform's main flow before final implementation.

The screen is still evolving, but it already represents the first visual proposal of the user dashboard, including:

- ATS score overview;
- General resume performance indicator;
- AI-powered optimization tips;
- List of uploaded resumes;
- Application progress tracking;
- Sidebar menu with access to the platform’s main areas.


> **Note:** the design is still under development and may be adjusted as the product evolves.

![Project screens preview](./docs/assets/figma-preview.png)

## Roadmap

- [ ] Resume generation
- [ ] LinkedIn PDF parser
- [ ] GitHub integration
- [ ] Portfolio analysis
- [ ] Job matching
- [ ] Multiple templates
- [ ] Export to PDF
- [ ] Export to DOCX

## Contributing

Contributions are welcome!

Please read CONTRIBUTING.md before submitting a Pull Request.

## Running the project

Create the environment files:

```bash
cp .env.example .env
cp backend/.env.example backend/.env
cp frontend/.env.example frontend/.env
cp bot/.env.example bot/.env
```

On Windows PowerShell:

```powershell
Copy-Item .env.example .env
Copy-Item backend/.env.example backend/.env
Copy-Item frontend/.env.example frontend/.env
Copy-Item bot/.env.example bot/.env
```

```bash
docker compose up --build
```

Services:

- Frontend: http://localhost:5173
- Backend: http://localhost:9000
- Bot: http://localhost:8000

Health endpoints:

- Backend: http://localhost:9000/up
- Bot: http://localhost:8000/health

## License

This project is licensed under the MIT License.