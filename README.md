# Οργάνωση Αποθετηρίων Διπλωματικής Εργασίας – SCORM Engine

## Γενικές Πληροφορίες

Το παρόν GitHub Organization περιλαμβάνει το τελικό παραδοτέο της Διπλωματικής Εργασίας του Ευάγγελου Κομνή (Evangelos Komnis), ΑΕΜ `ict20009`.

**Επιβλέπων Καθηγητής:** Μπασαγιάννης Στυλιανός  
**Πανεπιστήμιο:** Διεθνές Πανεπιστήμιο της Ελλάδος (International Hellenic University)  
**Τμήμα:** Τμήμα Μηχανικών Πληροφορικής, Υπολογιστών και Τηλεπικοινωνιών (Department of Computer, Informatics & Telecommunications Engineering)

### Τίτλος Διπλωματικής Εργασίας
Σχεδίαση και υλοποίηση διαδικτυακής μηχανής διαχείρισης περιεχομένου με έμφαση σε ασφάλεια και διαλειτουργικότητα (ΠΑΝ)

## Περίληψη

Η διπλωματική εργασία εστιάζει στον σχεδιασμό και την υλοποίηση μιας ασφαλούς και επεκτάσιμης μηχανής SCORM, με στόχο τη διαλειτουργική ενσωμάτωση με LMS, την αξιόπιστη αποθήκευση/συγχρονισμό προόδου και την υποστήριξη των SCORM 1.2 και SCORM 2004.

## Δομή Οργάνωσης Αποθετηρίων

1. `scorm-engine`  
   Backend REST engine (Spring Boot) για import μαθημάτων, launches, runtime commits, progress persistence και reporting.
2. `player`  
   Runtime player (Node.js/TypeScript) για launch rendering, SCO serving και runtime bridge προς engine.
3. `scorm-engine-php-sdk`  
   Framework-agnostic PHP SDK (PSR-18) για κατανάλωση του `scorm-engine` API.
4. `example-lms-client`  
   Laravel reference LMS client που ενσωματώνει το PHP SDK και υλοποιεί admin/learner flows.
5. `central-docker-infrastructure`  
   Ενοποιημένη containerized υποδομή (Compose) για engine, player, LMS και supporting services (Postgres, Redis, MinIO, ELK).
6. `github-actions-template`  
   Πρότυπα/συμβάσεις GitHub Actions workflows για ομοιομορφία CI/CD.
7. `thesis-document-latex`  
   Κείμενο διπλωματικής σε LaTeX (συγγραφή/τεκμηρίωση).

### Α. Πυρήνας Συστήματος (Core System Components)

- `scorm-engine`
- `player`
- `scorm-engine-php-sdk`
- `example-lms-client`

### Β. Υποδομή και Αυτοματοποίηση (Infrastructure & Automation)

- `central-docker-infrastructure`
- `github-actions-template`

### Γ. Τεκμηρίωση και Ακαδημαϊκό Υλικό (Documentation & Academic Material)

- `thesis-document-latex`

## Σχέσεις Μεταξύ Repos

- `example-lms-client` -> χρησιμοποιεί `scorm-engine-php-sdk`.
- `scorm-engine-php-sdk` -> καταναλώνει API του `scorm-engine`.
- `player` -> επικοινωνεί runtime με `scorm-engine`.
- `central-docker-infrastructure` -> ορχηστρώνει `scorm-engine`, `player`, `example-lms-client` και data/observability services.

## Σκοπός

Το organization συγκεντρώνει το σύνολο του ερευνητικού, σχεδιαστικού και υλοποιητικού έργου της διπλωματικής, με στόχο:

- διαφάνεια στην αρχιτεκτονική και την εξέλιξη,
- αναπαραγωγιμότητα μέσω CI/CD και containerized υποδομής,
- συστηματική τεκμηρίωση και ακαδημαϊκή πληρότητα.

---

# Thesis Organization – SCORM Engine Project

## General Information

This GitHub Organization contains the final deliverable of the Diploma Thesis of Evangelos Komnis, Student ID `ict20009`.

**Supervisor:** Stylianos Basagiannis  
**University:** International Hellenic University  
**Department:** Department of Computer, Informatics & Telecommunications Engineering

### Thesis Title
Design and Implementation of a Web-Based Content Management Engine with Emphasis on Security and Interoperability (PAN)

## Abstract

This thesis focuses on the design and implementation of a secure and extensible SCORM Engine platform, targeting interoperable LMS integration, resilient learner-progress synchronization, and support for SCORM 1.2 and SCORM 2004.

## Repository Structure

1. `scorm-engine`  
   Spring Boot backend engine for course import, launches, runtime commits, persistence, and reporting.
2. `player`  
   Node.js/TypeScript runtime player for launch rendering, SCO delivery, and runtime API bridging.
3. `scorm-engine-php-sdk`  
   Framework-agnostic PHP SDK (PSR-18) for consuming `scorm-engine` APIs.
4. `example-lms-client`  
   Laravel reference LMS client integrating the PHP SDK for admin and learner flows.
5. `central-docker-infrastructure`  
   Unified Docker Compose stack for the full platform and supporting services.
6. `github-actions-template`  
   Reusable CI/CD workflow conventions and templates.
7. `thesis-document-latex`  
   Thesis writing and maintenance repository (LaTeX).

### A. Core System Components

- `scorm-engine`
- `player`
- `scorm-engine-php-sdk`
- `example-lms-client`

### B. Infrastructure & Automation

- `central-docker-infrastructure`
- `github-actions-template`

### C. Documentation & Academic Material

- `thesis-document-latex`

## Inter-Repository Relationships

- `example-lms-client` depends on `scorm-engine-php-sdk`.
- `scorm-engine-php-sdk` targets `scorm-engine` API endpoints.
- `player` exchanges runtime data with `scorm-engine`.
- `central-docker-infrastructure` orchestrates engine, player, LMS, and supporting data/observability services.

## Purpose

This organization consolidates the complete research, design, and implementation output of the thesis to ensure:

- architectural transparency,
- reproducibility through CI/CD and containerized deployment,
- systematic technical and academic documentation.
