# Cryptography

This project is developed during the course of "Cryptography" in University of Macedonia.

I developed some python scripts, using [Sage math cloud version](https://cloud.sagemath.com/).

There are two files. One for each Task that I had to complete.

In the Task 1 I had to work with classic Cryptosystems.

In the Task 2 I had to face more recent Cryptosystems.


##TASK 1: 
###Κρυπταλγόριθμος Μετατόπισης (Shift Cipher)  <br>
Υλοποιούνται οι παρακάτω συναρτήσεις. <br>

**shiftCipherEnc(pl, k)**: Η συνάρτηση υλοποιεί την κρυπτογράφηση με τον κρυπταλγόριθμο μετατόπισης<br>
**shiftCipherDec(ct,k)**: Η συνάρτηση υλοποιεί την αποκρυπτογράφηση με τον κρυπταλγόριθμο μετατόπισης<br>

####Βοηθητικές συναρτήσεις
**str2lst(s)**: παίρνει ένα αλφαριθμητικό και επιστρέφει σε λίστα τις αριθμητικές τιμές των χαρακτήρων του αλφαριθμητικού.<br>
**lst2str(lst)**: αντίθετη λειτουργία της **str2lst(s)**.<br>

###---------------------------------------------------<br>

###Κρυπταλγόριθμος Αντικατάστασης (Transposition Cipher) <br>
Υλοποιούνται οι παρακάτω συναρτήσεις. <br>

**subCipherDec(c, key)**: Η subCipherDec αποκρυπτογραφεί το κείμενο c με βάση το κλειδί key.<br>

####Βοηθητικές συναρτήσεις
**CreateKey(sorted_freq, engFreq)**:  Η CreateKey, δοσμένης της λίστας με τις συχνότητες (ταξινομημένες) καθώς και με τα πιο συχνά γράμματα της αγγλικής, κάνει την αντιστοίχηση ώστε να παραχθεί το κλειδί.<br>
**replaceChar(li, old, new)**:Η replaceChar αντικαθιστά έναν χαρακτήρα (old) σε μια λίστα (li) με έναν άλλο χαρακτήρα (new)<br>
**findFreqs(freq)**: Η findFreqs, παίρνει ως είσοδο τις συχνότητες εμφάνισης τωνς γραμμάτων σε ένα κείμενο αλφαβητικά και τις ταξινομεί με φθίσουσα σειρά.<br>

###---------------------------------------------------<br>

###Ομοπαραλληλικός κρυπταλγόριθμος (Affine Cipher)  <br>
Υλοποιούνται οι παρακάτω συναρτήσεις. <br>

**affine_enc(m, key1, key2)**: Κρυπτογράφηση Ομοποραλληλικού κρυπταλγορίθμου.<br>
**affine_dec(c, key1, key2)**: Αποκρυπτογράφηση Ομοπαραλληλικού κρυπταλγορίθμου.<br>
**affine_number_enc(m, k1, k2, mod)**: Ορίζω ξανά την κρυπτογράφηση για αριθμούς.<br>
**affine_number_dec(c, k1, k2, mod)**: Ορίζω ξανά την αποκρυπτογράφηση για αριθμούς.<br>

####Βοηθητικές συναρτήσεις
**affine_analysis(plaintext, ciphertext)**: Λύση συστήματος εξισώσεων για εύρεση κλειδιών.<br>
**affine_analysis_num(p1, p2, c1, c2)**: Ορίζω ξανά την ανάλυση για αριθμούς.<br>

###---------------------------------------------------<br>

###Βάση εκφώνησης Ομοπαραλληλικός Κρυπταλγόριθμος (Custom Affine Cipher) <br>
Υλοποιούνται οι παρακάτω συναρτήσεις. <br>

**custom_affine_enc(m, k1, k2, k3)**: Κρυπτογράφηση<br>
**custom_affine_dec(ct, k1, k2, k3)**: Αποκρυπτογράφηση<br>

####Βοηθητικές συναρτήσεις
**check_b(b)**: Ελέγχει αν το b είναι σχετικά πρώτος με το 26. Στην ουσία αν κάνει για κλειδί.<br>
**custom_affine_analysis(plaintext, ciphertext)**: Ανάλυση κρυπτοσυστήματος για εύρεση πιθανών κλειδιών.<br>

###---------------------------------------------------<br>

###Κρυπταλγόριθμος Hill (Hill Cipher)  <br>
Υλοποιούνται οι παρακάτω συναρτήσεις. <br>

**Hill_enc(m, K)**: Η συνάρτηση υλοποιεί την κρυπτογράφηση με τον κρυπταλγόριθμο Hill.<br>
**Hill_dec(c, K)**: Η συνάρτηση υλοποιεί την αποκρυπτογράφηση με τον κρυπταλγόριθμο Hill.<br>

####Βοηθητικές συναρτήσεις
**check_valid(K)**: Ελέγχει αν ο πίνακας K είναι αντιστρέψιμος, στην ουσία αν είναι δυνατό (πιθανό) κλειδί.<br>

###---------------------------------------------------<br>
