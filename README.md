# Οργάνωση Αποθετηρίων Διπλωματικής Εργασίας – SCORM Engine

## Γενικές Πληροφορίες

Το παρόν GitHub Organization περιλαμβάνει το τελικό παραδοτέο της Διπλωματικής Εργασίας του Ευάγγελου Κομνή (Evangelos Komnis), ΑΕΜ ict20009.

### Τίτλος Διπλωματικής Εργασίας
Σχεδίαση και υλοποίηση διαδικτυακής μηχανής διαχείρισης περιεχομένου με έμφαση σε ασφάλεια και διαλειτουργικότητα (ΠΑΝ)

## Περίληψη

Η παρούσα διπλωματική εργασία ασχολείται με τον σχεδιασμό και την ανάπτυξη μιας ασφαλούς και αποδοτικής μηχανής SCORM (SCORM Engine), η οποία υποστηρίζει τα πλέον διαδεδομένα πρότυπα SCORM και ενσωματώνει μηχανισμούς αποθήκευσης και συγχρονισμού της προόδου των χρηστών.

Το σύστημα έχει σχεδιαστεί ώστε να επικοινωνεί με Συστήματα Διαχείρισης Μάθησης (Learning Management Systems – LMS) για τη μετάδοση και διαχείριση δεδομένων προόδου. Ιδιαίτερη έμφαση δίνεται στην ασφάλεια, τη διαλειτουργικότητα, την επεκτασιμότητα και την αποδοτική διαχείριση εκπαιδευτικών δεδομένων.

## Δομή Οργάνωσης Αποθετηρίων

Τα αποθετήρια της οργάνωσης ομαδοποιούνται με βάση το λειτουργικό και επιστημονικό τους πλαίσιο ως εξής:

### Α. Πυρήνας Συστήματος (Core System Components)

#### Α.1 Backend Application – SCORM Engine  
Το κύριο αποθετήριο του συστήματος, το οποίο περιλαμβάνει την υλοποίηση του backend της μηχανής SCORM. Αποτελεί τον βασικό πυρήνα του συστήματος και διαχειρίζεται την επεξεργασία SCORM πακέτων, την αποθήκευση και τον συγχρονισμό προόδου, καθώς και την επικοινωνία με εξωτερικά LMS μέσω κατάλληλων διεπαφών προγραμματισμού (APIs).

#### Α.2 Player / Client Εφαρμογή  
Αποθετήριο που περιλαμβάνει την υλοποίηση της εφαρμογής πελάτη (frontend), υπεύθυνης για την απόδοση των SCORM πακέτων και την αλληλεπίδραση με το backend σύστημα.

---

### Β. Υποδομή Ανάπτυξης και Ανάπτυξης Λογισμικού (Infrastructure & Deployment)

#### Β.1 Docker Infrastructure  
Αποθετήριο το οποίο ενοποιεί τα επιμέρους Docker components των επιμέρους αποθετηρίων και επιτρέπει τη συγκρότηση και ανάπτυξη της πλήρους στοίβας της εφαρμογής σε περιβάλλον containerized deployment.

---

### Γ. Τεκμηρίωση και Ακαδημαϊκό Υλικό (Documentation & Academic Material)

#### Γ.1 Συγγραφή Διπλωματικής (LaTeX – MudLaTeX)  
Αποθετήριο για την ανάπτυξη, επιμέλεια και συντήρηση του κειμένου της διπλωματικής εργασίας σε περιβάλλον LaTeX, σύμφωνα με το πρότυπο MudLaTeX.

#### Γ.2 Παραρτήματα Διπλωματικής  
Αποθετήριο που περιλαμβάνει τα παραρτήματα της εργασίας, συμπληρωματικό υλικό, τεχνικά διαγράμματα και υποστηρικτική τεκμηρίωση.

#### Γ.3 Βιβλιογραφία ()  
Αποθετήριο που περιλαμβάνει τη βιβλιογραφία της εργασίας σε ψηφιακή μορφή (PDF, επιστημονικά άρθρα και λοιπές πηγές), οργανωμένη σε περιβάλλον Docker για λόγους αναπαραγωγιμότητας και αρχειοθέτησης.

## Σκοπός

Το παρόν organization συγκεντρώνει το σύνολο του ερευνητικού, σχεδιαστικού και υλοποιητικού έργου της διπλωματικής εργασίας, διασφαλίζοντας τη διαφάνεια, την αναπαραγωγιμότητα και τη συστηματική τεκμηρίωση του αναπτυγμένου συστήματος.

---

# Thesis Organization – SCORM Engine Project

## General Information

This GitHub Organization contains the final deliverable of the Diploma Thesis of Evangelos Komnis, Student ID: ict20009.

### Thesis Title
Design and Implementation of a Web-Based Content Management Engine with Emphasis on Security and Interoperability (PAN)

## Abstract

This diploma thesis focuses on the design and development of a secure and efficient SCORM Engine that supports the most widely adopted SCORM standards and integrates mechanisms for storing and synchronizing user progress.

The system is designed to communicate with Learning Management Systems (LMS) for the transmission and management of learner progress data. Particular emphasis is placed on security, interoperability, scalability, and efficient management of educational data.

## Repository Structure

The repositories within this organization are grouped according to their functional and academic context as follows:

### A. Core System Components

#### A.1 Backend Application – SCORM Engine  
The primary repository of the system, containing the backend implementation of the SCORM Engine. It constitutes the core component of the project and is responsible for SCORM package processing, progress storage and synchronization, as well as communication with external LMS platforms via appropriate APIs.

#### A.2 Player / Client Application  
Repository containing the frontend implementation responsible for rendering SCORM packages and interacting with the backend system.

---

### B. Infrastructure & Deployment

#### B.1 Docker Infrastructure  
Repository that integrates the individual Docker components of the respective repositories and enables the build and deployment of the complete application stack in a containerized environment.

---

### C. Documentation & Academic Material

#### C.1 Thesis Writing (LaTeX – MudLaTeX)  
Repository dedicated to the development, editing, and maintenance of the thesis text using LaTeX, following the MudLaTeX template format.

#### C.2 Thesis Appendices  
Repository containing the appendices of the thesis, supplementary material, technical diagrams, and supporting documentation.

#### C.3 Bibliography (Dockerized Archive)  
Repository containing the thesis bibliography in digital form (PDF files, academic papers, and related sources), organized within a Docker environment to ensure reproducibility and archival consistency.

## Purpose

This organization consolidates the entirety of the research, design, and implementation work conducted in the context of the diploma thesis, ensuring transparency, reproducibility, and systematic documentation of the developed system.
