`Project Requirements rules *@docs/project-requirements.md* You will use tools codebase to know what are the details of the files of this *@docs/project-requirements.md* directory files to check the project requirements and the project standards that you need to follow. This will be the guide for you to make sure you are following the project standards. So make sure to read this when planning and implementing the project to avoid duplications, conflicts, and errors. Don't touch that folder and files, you will only read it. Don't over do it to the point that you are not following the project requirements. DON'T REMOVE THIS LINE 1!!!!`


# Accounting Website Project Requirements

## Core Features
1. **Calculation Engine**
   - Financial ratio analysis
   - Depreciation calculations (straight-line & reducing balance)
   - Tax computations
   - Break-even analysis
   - Cash flow projections

2. **Financial Statement Generator**
   - Balance sheet templates
   - Income statement builder
   - Cash flow statement wizard
   - Custom report creation

3. **Realtime Collaboration**
   - Multi-user editing
   - Version control
   - Change tracking
   - Audit trails

4. **Data Management**
   - CSV/Excel import/export
   - Cloud sync capabilities
   - Data validation rules
   - Historical data comparison

## Technical Specifications
**Frontend:**
- Mobile first approach
- Next.js 14 (App Router)
- TypeScript
- Tailwind CSS + Shadcn UI
- Recharts (data visualization)
- Math.js (calculations)
- Zustand (state management)
- Framer motion (animation)

**Backend:**
- Next.js API routes
- Supabase (PostgreSQL Database)
- Supabase Auth
- Supabase Realtime
- Supabase Storage (for files)
- Prisma ORM (optional)
- Zod (validation)

**Key Integrations:**
- Tax rates: Supabase Edge Functions (self-contained)
- Currency rates: Supabase PostgreSQL extensions
- PDF export: Supabase Storage + React-PDF
- CSV handling: Supabase Import/Export

## Security Requirements
1. AES-256 encryption for data at rest
2. TLS 1.3 for data in transit
3. Role-based access control (RBAC)
4. Activity logging & audit trails
5. SOC 2 compliance (Future Phase)

## Compliance Requirements
- GAAP/IFRS compliance checks
- Tax regulation updates
- Data retention policies
- Accessibility (WCAG 2.1 AA)
- GDPR-ready architecture

## Documentation Standards
1. Inline TSDoc comments for all calculations
2. OpenAPI specification for APIs
3. ER diagrams for database schema
4. Audit trail documentation
5. Financial formula registry

## Project Roadmap (Updated Implementation Sequence)

### Epic 1 - Core Accounting Features (2-3 weeks)
**Implementation Order**:
1. **Feature 1.1 - Project Infrastructure Setup** (1 day)
   - User Story 1.1.1 - Supabase initialization
   - User Story 1.1.2 - Next.js boilerplate with TypeScript
   - User Story 1.1.3 - Core component structure
   - User Story 1.1.4 - Error boundary setup



2. **Feature 1.2 - Calculation Engine Foundation** (5 days)
   - User Story 1.2.1 - Math.js integration
   - User Story 1.2.2 - Depreciation calculator (straight-line)
   - User Story 1.2.3 - Financial ratio formulas
   - User Story 1.2.4 - Calculation validation system
   - User Story 1.2.5 - Unit test setup


3. **Feature 1.3 - Financial Statement Templates** (4 days)
   - User Story 1.3.1 - Balance sheet component
   - User Story 1.3.2 - Income statement builder
   - User Story 1.3.3 - PDF export functionality
   - User Story 1.3.4 - Data validation schemas


4. **Feature 1.4 - Local Data Management** (3 days)
   - User Story 1.4.1 - Local storage integration
   - User Story 1.4.2 - Data encryption setup
   - User Story 1.4.3 - Historical versioning
   - User Story 1.4.4 - CSV export (basic)


5. **Feature 1.5 - UI/UX Foundation** (3 days)
   - User Story 1.5.1 - Mobile-first responsive layout
   - User Story 1.5.2 - Accessible form components
   - User Story 1.5.3 - Data visualization (Recharts)
   - User Story 1.5.4 - Dark mode support
   - User Story 1.5.5 - Loading/error states


6. **Feature 1.6 - Basic Security** (2 days)
   - User Story 1.6.1 - Input sanitization
   - User Story 1.6.2 - Audit logging
   - User Story 1.6.3 - Rate limiting
   - User Story 1.6.4 - Error boundaries


### Epic 2 - Data Management (1-2 weeks)
**Priority**: ★★★☆☆
**Implementation Order**:
1. **Feature 2.1 - Authentication System** (3 days)

   - User Story 2.1.1 - Supabase auth setup
   - User Story 2.1.2 - User profile management
   - User Story 2.1.3 - Session management
   - User Story 2.1.4 - Basic RBAC roles


2. **Feature 2.2 - Cloud Data Migration** (4 days)
   - User Story 2.2.1 - Supabase database schema
   - User Story 2.2.2 - Local → Cloud migration tool
   - User Story 2.2.3 - Data encryption at rest
   - User Story 2.2.4 - Conflict resolution


3. **Feature 2.3 - Advanced CSV Handling** (3 days)
   - User Story 2.3.1 - Bulk import/export
   - User Story 2.3.2 - Data validation rules
   - User Story 2.3.3 - Template system
   - User Story 2.3.4 - Error reporting


### Epic 3 - Collaboration Features (2 weeks)
**Priority**: ★★☆☆☆
**Implementation Order**:
1. **Feature 3.1 - Realtime Foundation** (3 days)

   - User Story 3.1.1 - Supabase Realtime setup
   - User Story 3.1.2 - Presence indicators
   - User Story 3.1.3 - Basic co-editing
   - User Story 3.1.4 - Connection status


2. **Feature 3.2 - Version Control** (4 days)
   - User Story 3.2.1 - Change tracking
   - User Story 3.2.2 - Version history
   - User Story 3.2.3 - Snapshot system
   - User Story 3.2.4 - Rollback functionality



3. **Feature 3.3 - Collaboration Tools** (3 days)
   - User Story 3.3.1 - Comments system
   - User Story 3.3.2 - @mentions
   - User Story 3.3.3 - Notifications
   - User Story 3.3.4 - Activity feed


------`don't read and implement this phase 4, this is just for you to know the future features that we will implement`------
### Phase 4 - Advanced Features (Optional)
**Priority**: ★☆☆☆☆
**Implementation Order**:
1. **Feature 4.1 - Bank Integrations** (5 days)
   - User Story 4.1.1 - Plaid sandbox setup
   - User Story 4.1.2 - Transaction import
   - User Story 4.1.3 - Reconciliation tools
   - User Story 4.1.4 - Webhook handlers


2. **Feature 4.2 - Multi-currency** (3 days)
   - User Story 4.2.1 - Exchange rate system
   - User Story 4.2.2 - Currency converter
   - User Story 4.2.3 - Localization
   - User Story 4.2.4 - FX gain/loss calc


3. **Feature 4.3 - Automation** (4 days)
   - User Story 4.3.1 - Tax rule engine
   - User Story 4.3.2 - Scheduled reports
   - User Story 4.3.3 - Compliance checks
   - User Story 4.3.4 - Audit trails


4. **Feature 4.4 - Advanced Reporting** (3 days)
   - User Story 4.4.1 - Custom templates
   - User Story 4.4.2 - Data visualization
   - User Story 4.4.3 - Executive dashboards
   - User Story 4.4.4 - Export formats


------`don't read and implement this phase 4, this is just for you to know the future features that we will implement`------

## Cost Analysis
| Feature          | Supabase Service         | Free Tier Limits              |
|------------------|--------------------------|-------------------------------|
| Database         | PostgreSQL               | 500MB database + 1GB bandwidth|
| Auth             | Authentication           | 50k MAUs                      |
| Realtime         | Realtime Updates         | 50 concurrent connections     |
| Storage          | File Storage             | 1GB storage, 1M downloads     |
| Edge Functions   | Serverless Functions     | 500k invocations/month        |
| Vector           | PostgreSQL Extensions    | Free with database            |

## Implementation Benefits
1. Single provider for all backend needs
2. Unified authentication system
3. Direct database <> storage integration
4. Simplified billing and monitoring
5. Built-in rate limiting and security

## Architecture Guidelines

### 1. File and Folder Structure
```
src/
├── app/               # Next.js app router
│   ├── (auth)/        # Authentication routes
│   │   ├── login.tsx  # Login page
│   │   ├── register.tsx # Registration page
│   │   └── reset-password.tsx # Password reset page
│   ├── (dashboard)/   # Protected dashboard routes
│   │   ├── index.tsx  # Dashboard home
│   │   ├── reports.tsx # Reports page
│   │   └── settings.tsx # Settings page
│   ├── api/           # API route handlers
│   │   ├── auth.ts    # Auth API handler
│   │   └── data.ts    # Data API handler
│   └── layout.tsx     # Root layout
├── components/        # Reusable UI components
│   ├── core/          # Base components (buttons, inputs)
│   │   ├── Button/    # Button variants
│   │   │   ├── PrimaryButton.tsx
│   │   │   └── SecondaryButton.tsx
│   │   ├── Input/     # Form inputs
│   │   │   ├── TextInput.tsx
│   │   │   └── PasswordInput.tsx
│   │   └── Modal/     # Dialog components
│   │       ├── Modal.tsx
│   │       └── ConfirmModal.tsx
│   ├── accounting/    # Domain-specific components
│   │   ├── Ledger/    # Ledger components
│   │   │   ├── LedgerEntry.tsx
│   │   │   └── LedgerSummary.tsx
│   │   ├── Reports/   # Report components
│   │   │   ├── ReportTable.tsx
│   │   │   └── ReportChart.tsx
│   │   └── Journal/   # Journal entry components
│   │       ├── JournalEntry.tsx
│   │       └── JournalList.tsx
│   └── shared/        # Cross-feature components
│       ├── Layout/    # Layout components
│       │   ├── Header.tsx
│       │   └── Sidebar.tsx
│       ├── Nav/       # Navigation components
│       │   ├── NavBar.tsx
│       │   └── NavItem.tsx
│       └── Footer/    # Footer components
│           └── Footer.tsx
├── lib/
│   ├── api/           # API clients
│   │   ├── auth/      # Auth API functions
│   │   │   ├── login.ts
│   │   │   └── register.ts
│   │   └── supabase/  # Supabase client
│   │       └── client.ts
│   ├── hooks/         # Custom hooks
│   │   ├── auth/      # Authentication hooks
│   │   │   ├── useAuth.ts
│   │   │   └── useSession.ts
│   │   └── form/      # Form handling hooks
│   │       ├── useForm.ts
│   │       └── useValidation.ts
│   ├── utils/         # Helper functions
│   │   ├── date/      # Date formatting
│   │   │   ├── formatDate.ts
│   │   │   └── parseDate.ts
│   │   └── currency/  # Currency helpers
│   │       ├── formatCurrency.ts
│   │       └── convertCurrency.ts
│   └── validation/    # Zod schemas
│       ├── auth/      # Auth schemas
│       │   ├── loginSchema.ts
│       │   └── registerSchema.ts
│       └── forms/     # Form schemas
│           ├── contactFormSchema.ts
│           └── feedbackFormSchema.ts
├── types/             # Global TS types
    ├── api.ts         # API types
    ├── auth.ts        # Auth types
    └── supabase.ts    # Database types
   
### 2. Server/Client Separation
- **Server Components**: Default to server components for:
  - Data fetching
  - Sensitive operations
  - Static content
- **Client Components**: Only use when needed for:
  - Interactivity
  - Browser APIs
  - State management

### 3. Reusable Components
1. Create atomic components with:
   - PropTypes using TypeScript interfaces
   - Storybook stories for documentation
   - Accessibility attributes by default
2. Follow naming convention:
   - `FeatureComponentName.tsx` (e.g. `DepreciationCalculator.tsx`)
   - `CoreComponentName.tsx` (e.g. `FormInput.tsx`)

### 4. API Design Rules
- Versioned endpoints: `/api/v1/...`
- RESTful structure for resources
- Error format standardization:
  ```ts
  interface APIError {
    code: string;
    message: string;
    details?: Record<string, unknown>;
  }
  ```
