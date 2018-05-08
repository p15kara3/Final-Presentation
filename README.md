# Μάθημα: Τεχνολογίες Λογισμικού 
# Τελική Αναφορά  

## Εργασία: Οπτικοποίηση δεδομένων χορηγιών (UK) 

 * Ονοματεπώνυμο: **Καραντζή Παναγιώτα**  
 * Αριθμός Μητρώου: **Π2015130**  
 * e-mail: **p15kara3@ionio.gr** 
 * Προσωπικό αποθετήριο του κώδικα, *στο οποίο έγιναν αλλαγές*: [Link αποθετηρίου του κώδικα](https://github.com/p15kara3/D3js-uk-political-donations/tree/gh-pages)  
 * Link για το εκτελέσιμο: [Link εκτελέσιμου](https://p15kara3.github.io/D3js-uk-political-donations/)    
 * Link για τα παραδοτέα 1 και 2: [Παραδοτέα 1&2](https://github.com/courses-ionio/sw/tree/master/projects/2015130)
 

## Εισαγωγή  
Η συγκεκριμένη github-page αποτελεί την τελική αναφορά της εξαμηνιαίας εργασίας στο μάθημα Τεχνολογίες Λογισμικού του ΣΤ εξαμήνου. Στόχος της εργασίας ήταν η γνωριμία και η εκμάθηση των γλωσσών javascript, html και css. Παρακάτω περιγράφονται αναλυτικά οι διαδικασίες και οι αλλαγές που έγιναν σε κάθε παραδοτέο, στον δοθέντα κώδικα για την εκπλήρωση της εργασίας.   
  
## Σύνοψη  
Η εργασία αφορά την οπτικοποίηση των στατιστικών στοιχείων δωρεών που έχουν γίνει σε πολιτικά κομματα της Μεγάλης Βρετανίας.Σκοπός της εργασίας είναι η γνωριμία με τη βιβλιοθήκη D3 της javascript (οπτικοποίηση δεδομένων), καθώς και η αξιοποίηση των δυνατοτήτων της γλώσσας javascript για λειτουργίες μεγένθυνσης κειμένου και text-to-speech Επίσης, έχει στόχο την εξοικείωση με το περιβάλλον του github αλλά και την χρήση των github pages .Τέλος, εκτός από την javascript στοχεύει και στην επαφή με άλλες γλώσσες όπως η html  και η css.  

## Εργαλεία και ανάλυση σχετικών έργων  

Στα πλαίσια της εργασίας τα εργαλεία που χρησιμοποιήθηκαν ήταν το _jsfiddle_ και το _cloud9_ ώστε να μπορέσω να τεστάρω τις αλλαγές που έκανα στον κώδικα. Επίσης, χρησιμοποίησα διάφορες ιστοσελίδες όπως το W3schools, W3.org, javascript.com και  το tutorialspoint.com για εκμάθηση και συμβουλές σχετικά με τις γλώσσες που χρησιμποποιήθηκαν. 
Οι κώδικες που τροποπιήθηκαν: [Repository d3-uk-political-donations](https://github.com/neilhawkins/d3-uk-political-donations), [Link κώδικα για κινούμενη εικόνα](https://github.com/ioniodi/D3js-uk-political-donations/blob/master/participants/index.html)  

 ## Μέθοδος και τεχνικές ανάπτυξης  
 
 Οι μέθοδοι που χρησιμοποιήθηκαν και οι αλλαγές που έγιναν στο **πρώτο παραδοτέο** είναι οι εξής:  
 
  1) Έγιναν οι κατάλληλες αλλαγές ώστε να αλλάξει το url της εφαρμογής και να μην χρειάζεται να καταλήγει σε "full-viz.html".  
  ![image](https://user-images.githubusercontent.com/22661913/39729539-1dc91242-5265-11e8-9cf5-9dc2f351d63f.png)  
  
  2) Έγιναν αλλαγές στον κώδικα ώστε οι μπάλες με τα δεδομένα, καθώς και στα αντίστοιχα 3 πεδία της ομαδοποίησης Split by party να εμφανίζονται με διαφορετικό χρώμα. ( Γραμμή 24 [chart.js](https://github.com/p15kara3/D3js-uk-political-donations/blob/gh-pages/chart.js), γραμμές 100,104,108 [style.css](https://github.com/p15kara3/D3js-uk-political-donations/blob/gh-pages/style.css) )  
 ![image](https://user-images.githubusercontent.com/22661913/37311500-1dade2ba-2650-11e8-80f0-eae1cb94c2f6.png)  
 
 3) Έπειτα, για να ακούγεται ήχος κάθε φορά που ο χρήστης κάνει κλικ σε μία από τις επιλογές/κουμπιά ομαδοποίησης των δεδομένων έγιναν αλλαγές στο αρχείο [index](https://github.com/p15kara3/D3js-uk-political-donations/blob/gh-pages/index.html) (σειρές 33-36, 60-70) και η προσθήκη του click_sound.mp3. (Εδώ θα ήθελα να αναφέρω πως για κάποιο λόγο από mozilla ο ήχος λειτουργεί σωστά ενώ από άλλους browsers είναι απαραίτητο να γίνει reload ώστε να ακουστεί ο ήχος)  
 
 4) Ο κώδικας τροποποιήθηκε ώστε όταν γίνεται κλικ σε μια μπάλα να εμφανίζονται αποτελέσματα για τον αντίστοιχο δωρητή στο Google. Προστέθηκε η συνάρτηση search στο αρχείο [chart.js](https://github.com/p15kara3/D3js-uk-political-donations/blob/gh-pages/chart.js) (σειρές 357-360,113)  

![image](https://user-images.githubusercontent.com/22661913/37312052-2f99732a-2652-11e8-95d5-9938b1510a61.png)  

5) Έγινε τροποποίηση του κώδικα ώστε να λειτουργεί το ποντίκι ως μεγεθυντικός φακός όταν μεταφέρεται πάνω από τις λέξεις του κειμένου. Αλλαγές στο αρχείο [index](https://github.com/p15kara3/D3js-uk-political-donations/blob/gh-pages/index.html), σειρές 41-49.  

![image](https://user-images.githubusercontent.com/22661913/37312218-d42ed664-2652-11e8-866c-3933020f0d5a.png) 
  
6) Τροποποιήθηκε ο κώδικας της εφαρμογής έτσι ώστε το ποντίκι όταν βρίσκεται μέσα στον κύκλο κάποιου δωρητή, να ακούγεται η ονομασία του δωρητή και το ποσό της δωρεάς. (Σχετικός σύνδεσμος: https://responsivevoice.org/).  
Αλλαγές έγιναν στα αρχεία [chart.js](https://github.com/p15kara3/D3js-uk-political-donations/blob/gh-pages/chart.js)(σειρές 400,411) και [index](https://github.com/p15kara3/D3js-uk-political-donations/blob/gh-pages/index.html)(σειρά 259)  
  
 7) δημιουργήθηκε μια ακόμα επιλογή ομαδοποίησης των δεδομένων Split by the amount of the donation, όπου γίνεται ο διαχωρισμός σε δωρεές μέχρι 500.000, δωρεές μέχρι 1.000.000 και δωρεές πάνω από 1.000.000.  
Για να δημιουργηθεί η συγκεκριμένη επιλογή  ομαδοποίησης έγιναν αλλαγές και στα τρία αρχεία του κώδικα (chart.js,index.html,style.css) όπως φαίνεται στο προσωπικό μου λινκ.  

![image](https://user-images.githubusercontent.com/22661913/37313025-11a5dbb6-2656-11e8-8c63-030bed9b0dca.png)  

Επίσης, στα πλαίσια του πρώτου παραδοτέου έγινε δημιουργία φακέλου .csv στον φάκελο [participants](https://github.com/ioniodi/D3js-uk-political-donations/tree/master/participants) καθώς και η τοποθέτηση εικόνων των δωρητών Oscar Pinto-Hervia, John C Peake, Lord Alliance, The Halcyon Gallery, Richard D Harpin στον φάκελο [photos](https://github.com/ioniodi/D3js-uk-political-donations/tree/master/photos) του αποθετηρίου.  

Οι αλλαγές που έγιναν για το **δεύτερο παραδοτέο** αναφέρονται παρακάτω.  

1) Στο αρχείο index.html του φακέλου participants έγραψα τον κατάλληλο κώδικα ώστε να εμφανίζεται στην ιστοσελίδα με τους φοιτητές το όνομά και η εικόνα μου με κάποια κίνηση. Δέσμευσα την περιοχή του κώδικα "position#045" και έγιναν αλλαγές στον κώδικα στις γραμμές 1592-1640. ([index](https://github.com/ioniodi/D3js-uk-political-donations/blob/master/participants/index.html))  

![name](https://user-images.githubusercontent.com/22661913/39725136-8307aaae-5253-11e8-8778-7f0a1a8dab29.gif)  

2) από τα ζητούμενα που απαιτούνταν αλλαγές στο προσωπικό αποθετήριο πραγματοποίησα το πρώτο ερώτημα, δηλαδή να εμφανίζεται (και να επεκτείνεται δυναμικά) η σειρά των εικόνων με τους δωρητές πάνω από τους οποίους πέρασε ο δείκτης του ποντικιού στο γράφημα.
Έγιναν οι απαραίτητες αλλαγές στον κώδικα. Στο αρχείο [index](https://github.com/p15kara3/D3js-uk-political-donations/blob/gh-pages/index.html) στις γραμμές 76-78 [style.css](https://github.com/p15kara3/D3js-uk-political-donations/blob/gh-pages/style.css) στις 88-95 [chart.js](https://github.com/p15kara3/D3js-uk-political-donations/blob/gh-pages/chart.js) στις 404-411.  

![icons](https://user-images.githubusercontent.com/22661913/39725692-64d559a8-5255-11e8-9b02-918be1d8a88a.gif)  

## Συμπέρασμα  

Στα πλαίσια της εργασίας δόθηκε η ευκαιρία στους φοιτητές να έρθουν σε επαφή με τις γλώσσες html,css, javascript και πιο συγκεκριμένα με την βιβλιοθήκη D3 της javascript. Επιπλέον, έμαθαν να δημιουργούν ιστοσελίδες με τη βοήθεια των github-pages, καθώς και διαδικασίες του github όπως το fork και το pull-request. 
  
## Αναφορές  
https://www.w3schools.com/html/  
https://www.w3schools.com/css/  
https://www.javascript.com  
https://www.youtube.com/watch?v=VlwSz2dXK_8  
https://responsivevoice.org  
http://tobiasahlin.com/moving-letters/  
