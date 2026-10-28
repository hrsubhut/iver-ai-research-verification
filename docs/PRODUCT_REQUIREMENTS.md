
# IVER — Product Requirements

## 1. Product Vision

IVER is an AI-powered research platform that helps users investigate
questions, retrieve relevant evidence, verify claims, and produce
traceable research reports.

## 2. Target Users

- Students and academic researchers
- Professionals conducting evidence-based research
- Users who need to investigate and verify factual claims

## 3. Core User Journey

1. Submit a research question or factual claim.
2. Retrieve relevant documents and evidence.
3. Analyze claims against the available evidence.
4. Review verification results and source citations.
5. Save or export the research report.

## 4. Functional Requirements

### Research Workspace
- Accept research questions and factual claims.
- Support a clear research initiation workflow.
- Show validation errors for invalid input.
- Display progress, success, empty, and error states.

### Evidence Retrieval
- Retrieve relevant passages from available sources.
- Preserve source metadata and passage references.
- Link findings to the evidence used to support them.

### Claim Verification
- Classify claim-evidence relationships.
- Support, at minimum, supported, contradicted,
  and insufficient-evidence outcomes.
- Display uncertainty and relevant evidence.
- Never present a model prediction as definitive proof.

### Research Management
- Provide a research history.
- Allow users to revisit saved reports.
- Support report export in a later phase.

### Document Processing
- Plan for document upload and text extraction.
- Validate file types and sizes.
- Handle extraction failures safely.

## 5. Non-Functional Requirements

- Responsive and accessible user interface.
- Clear separation between frontend, backend, and ML code.
- Input validation and safe error handling.
- Reproducible ML experiments and evaluation.
- Secure handling of credentials and user data.
- Testable and maintainable components.
- Traceable source citations.

## 6. UI/UX Direction

- Minimal white interface with blue accents.
- Clear typography and consistent spacing.
- Research-focused layouts rather than a generic chatbot.
- Reusable components and responsive navigation.
- Accessible labels, contrast, and keyboard interactions.

## 7. Development Phases

### Phase 1: Design and Frontend MVP
- Finalize user journeys and page wireframes.
- Define the design system.
- Build the research workspace with clearly labelled mock data.
- Implement responsive layouts and UI states.

### Phase 2: Backend and ML
- Implement API contracts and backend services.
- Build evidence retrieval and claim verification.
- Evaluate model performance on held-out data.
- Connect the frontend to real API responses.

### Phase 3: Complete Platform
- Add persistent research history and reports.
- Integrate document processing and research workflows.
- Add integration tests, security controls, and deployment.

## 8. Success Criteria

- Users can submit a research request and inspect its results.
- Every displayed verification result identifies its evidence.
- Missing or conflicting evidence is handled transparently.
- The frontend and backend have testable interfaces.
- ML evaluation is reproducible and documented.
- The application can be deployed using documented steps.

## 9. Scope Management

Build the product incrementally. Do not implement all
planned features in the initial frontend milestone.
Use clearly labelled mock data until real services exist.
