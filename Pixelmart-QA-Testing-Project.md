# Pixelmart QA Testing Project (Task 03)

## TEST SUITE 1: Login

---

**Test Case ID:** TC_LOGIN_01  

**Title:** "Sign In" düyməsinə klik edildikdə istifadəçinin login səhifəsinə yönləndirilməsi  

**Prioritet:** Yüksək  

**Pre-condition:** İstifadəçi Pixelmart saytının əsas səhifəsindədir  

**Description:** "Sign In" düyməsinə klik edildikdən sonra istifadəçinin login səhifəsinə yönləndirilməsi yoxlanılır  

**Test Steps:**  
1. "Sign In" düyməsini tap  
2. "Sign In" düyməsinə klik et  

**Expected Result:** İstifadəçi login səhifəsinə yönləndirilməlidir  

**Actual Result:** Login səhifəsi uğurla açıldı  

**Status:** Passed  

---

**Test Case ID:** TC_LOGIN_02  

**Title:** Düzgün email və parol daxil edildikdə istifadəçinin şəxsi hesaba daxil olması  

**Prioritet:** Yüksək  

**Pre-condition:** stifadəçi login səhifəsindədir  

**Description:** İstifadəçinin düzgün (valid) email və parol daxil edərək sistemə uğurla daxil olması yoxlanılır  

**Test Steps:**  
1. Email input sahəsinə klik et  
2. Düzgün (valid) email daxil et  
3. Parol input sahəsinə klik et  
4. Düzgün (valid) parol daxil et  
5. "Sign In" düyməsinə klik et  

**Expected Result:** İstifadəçi uğurla şəxsi hesabına daxil olmalıdır və əsas səhifəyə yönləndirilməlidir  

**Actual Result:** İstifadəçi uğurla şəxsi hesabına daxil oldu və əsas səhifə açıldı  

**Status:** Passed  

---

**Test Case ID:** TC_LOGIN_03  

**Title:** Yanlış email və parol daxil edildikdə istifadəçinin hesaba daxil ola bilməməsi  

**Prioritet:** Yüksək  

**Pre-condition:** İstifadəçi login səhifəsindədir  

**Description:** Yanlış (invalid) email və parol daxil edildikdə sistemin istifadəçinin hesaba girişinə icazə verməməsi yoxlanılır  

**Test Steps:**  
1. Email input sahəsinə klik et  
2. Yanlış (invalid) email daxil et  
3. Parol input sahəsinə klik et  
4. Yanlış (invalid) parol daxil et  
5. "Sign In" düyməsinə klik et  

**Expected Result:**  İstifadəçi hesaba daxil olmamalıdır  

**Actual Result:**  İstifadəçi yanlış email və parol ilə hesaba daxil ola bildi  

**Status:** Failed (Bug)  

---

**Test Case ID:** TC_LOGIN_04  

**Title:** Yanlış (format baxımından uyğun olmayan) email və parol daxil edildikdə istifadəçinin hesaba daxil ola bilməməsi  

**Prioritet:** Yüksək  

**Pre-condition:** İstifadəçi login səhifəsindədir  

**Description:** Yanlış formatda email və parol daxil edildikdə sistemin girişə icazə verməməsi yoxlanılır  

**Test Steps:**  
1. Email input sahəsinə klik et  
2. Yanlış formatda email daxil et. məsələn: 123456  
3. Parol input sahəsinə klik et  
4. Yanlış parol daxil et.məsələn: 123456789  
5. “Daxil ol” düyməsinə klik et  

**Expected Result:** İstifadəçi hesaba daxil olmamalıdır və Sistem uyğun xəta mesajı göstərməlidir  

**Actual Result:** İstifadəçi yanlış formatda məlumatlarla sistemə daxil ola bildi  

**Status:** Failed (Bug)  

---

## TEST SUITE 2: Səbət (Cart)

---

**Test Case ID:** TC_CART_01  

**Title:** "Səbət" düyməsinə klik edildikdə istifadəçinin səbət səhifəsinə yönləndirilməsi  

**Prioritet:** Yüksək  

**Pre-condition:** İstifadəçi Pixelmart saytının əsas səhifəsindədir  

**Description:** "Səbət" düyməsinə klik edildikdə istifadəçinin səbət səhifəsinə düzgün yönləndirilməsi yoxlanılır  

**Test Steps:**  
1. Səhifədə "Səbət" düyməsini tap  
2. "Səbət" düyməsinə klik et  

**Expected Result:** İstifadəçi səbət səhifəsinə yönləndirilməlidir  

**Actual Result:** "Səbət" düyməsinə klik edildikdə səbət səhifəsi uğurla açıldı  

**Status:** Passed  

---

**Test Case ID:** TC_CART_02  

**Title:** Bir neçə məhsul səbətə əlavə edildikdə səbət ikonunda məhsul sayının düzgün göstərilməsi  

**Prioritet:** Yüksək  

**Pre-condition:** İstifadəçi Pixelmart saytının əsas səhifəsindədir  

**Description:**  İstifadəçinin bir neçə məhsulu səbətə əlavə etdikdə səbət səhifəsində və səbət ikonunda məhsul sayının düzgün göstərilməsi yoxlanılır  

**Test Steps:**  
1. İstənilən məhsul səhifəsini aç  
2. “Səbətə əlavə et” düyməsinə klik et  
3. Başqa bir məhsul seç və onun səhifəsini aç  
4. Yenidən “Səbətə əlavə et” düyməsinə klik et  
5. Səhifənin yuxarı hissəsindəki səbət ikonunu yoxla  
6. Səbət səhifəsinə keç  

**Expected Result:** Səbət ikonunda əlavə olunan məhsulların sayı düzgün göstərilməlidir və səbət səhifəsində bütün əlavə olunmuş məhsullar siyahı şəklində görünməlidir  

**Actual Result:** Səbət ikonunda və səbət səhifəsində əlavə olunan məhsullar düzgün şəkildə göstərildi  

**Status:** Passed  

---

**Test Case ID:** TC_CART_03  

**Title:** Səbətdə məhsul sayının “+” və “−” düymələri ilə artırılması və azaldılması  

**Prioritet:** Yüksək  

**Pre-condition:** İstifadəçi Pixelmart saytının əsas səhifəsindədir  

**Description:**  
 Səbətə əlavə olunmuş məhsulun sayının “+” və “−” düymələri vasitəsilə düzgün artırılıb-azaldılması yoxlanılır  

**Test Steps:**  
1. İstənilən məhsulu seç və səhifəsini aç  
2. “Səbətə əlavə et” düyməsinə klik et  
3. Səbət səhifəsinə keç  
4. Məhsulun qarşısındakı “+” düyməsinə klik et  
5. Məhsul sayının artdığını yoxla  
6. “−” düyməsinə klik et  
7. Məhsul sayının azaldığını yoxla  
8. Məhsul sayını 1-dən 0-a endir  

**Expected Result:**  
“+” düyməsi ilə məhsul sayı artmalıdır və “−” düyməsi ilə məhsul sayı azalmalıdır   

**Actual Result:** Məhsul sayı azaldılarkən mənfi dəyərə qədər azaldı  

**Status:** Failed (Bug)  

---

## TEST SUITE 3: Sign Up

---

**Test Case ID:** TC_SIGNUP_03  

**Title:** Password və Confirm Password eyni olduqda istifadəçinin uğurla qeydiyyatdan keçməsi  

**Prioritet:** Yüksək  

**Pre-condition:**  İstifadəçi Pixelmart saytının əsas səhifəsindədir  

**Description:** İstifadəçi bütün sahələrə düzgün məlumatlar daxil etdikdə və Password ilə Confirm Password eyni olduqda sistemin uğurla qeydiyyat yaratması yoxlanılır  

**Test Steps:**  
1. Pixelmart saytının əsas səhifəsini aç  
2. “Sign In” düyməsinə klik et  
3. Açılan səhifədə “Create account” linkinə klik et  
4. Name sahəsinə düzgün ad daxil et  
5. Email sahəsinə düzgün email daxil et  
6. Phone sahəsinə düzgün nömrə daxil et  
7. Password sahəsinə düzgün parol daxil et  
8. Confirm Password sahəsinə eyni parolu daxil et  
9. “Create Account” düyməsinə klik et  

**Expected Result:**  
İstifadəçi uğurla qeydiyyatdan keçməlidir və Sistem yeni hesab yaratmalıdır,İstifadəçi şəxsi hesab səhifəsinə yönləndirilməlidir  

**Actual Result:**  İstifadəçi uğurla qeydiyyatdan keçdi və şəxsi hesab səhifəsi açıldı  

**Status:** Passed  

---

**Test Case ID:** TC_SIGNUP_08  

**Title:** Name sahəsinə yalnız rəqəmlər daxil edildikdə qeydiyyatın mümkün olmaması  

**Prioritet:** Yüksək  

**Pre-condition:** İstifadəçi Sign Up səhifəsindədir  

**Description:**  Name sahəsinə yalnız rəqəmlər daxil edildikdə sistemin bunu qəbul etməməsi yoxlanılır  

**Test Steps:**  
1. Name sahəsinə 123456 daxil et  
2. Email sahəsinə düzgün email daxil et  
3. Phone sahəsinə düzgün nömrə daxil et  
4. Password sahəsinə düzgün parol daxil et  
5. Confirm Password sahəsinə eyni parolu daxil et  
6. “Create Account” düyməsinə klik et  

**Expected Result:** Sistem qeydiyyata icazə verməməlidir  

**Actual Result:** Sistem yalnız rəqəmlərlə daxil edilmiş name ilə qeydiyyata icazə verdi  

**Status:** Failed (Bug)  

---

**Test Case ID:**  TC_SIGNUP_09  

**Title:** Name sahəsinə xüsusi simvollar daxil edildikdə qeydiyyatın mümkün olmaması  

**Prioritet:** Yüksək  

**Pre-condition:**  
 İstifadəçi Sign Up səhifəsindədir  

**Description:**  
 Name sahəsinə xüsusi simvollar daxil edildikdə sistemin bunu qəbul etməməsi yoxlanılır  

**Test Steps:**  
1. Name sahəsinə @#$%^&* daxil et  
2. Email sahəsinə düzgün email daxil et  
3. Phone sahəsinə düzgün nömrə daxil et  
4. Password sahəsinə düzgün parol daxil et  
5. Confirm Password sahəsinə eyni parolu daxil et  
6. “Create Account” düyməsinə klik et  

**Expected Result:** Sistem qeydiyyata icazə verməməlidir  

**Actual Result:**  Sistem xüsusi simvollarla qeydiyyata icazə verdi  

**Status:** Failed (Bug)  

---

**Test Case ID:**  TC_SIGNUP_10  

**Title:** Name sahəsinə yalnız boşluq daxil edildikdə qeydiyyatın mümkün olmaması  

**Prioritet:** Yüksək  

**Pre-condition:** İstifadəçi Sign Up səhifəsindədir  

**Description:** Name sahəsinə yalnız boşluqlardan ibarət dəyər daxil edildikdə sistemin bunu qəbul etməməsi yoxlanılır  

**Test Steps:**  
1. Name sahəsinə yalnız boşluq daxil et  
2. Email sahəsinə düzgün email daxil et  
3. Phone sahəsinə düzgün nömrə daxil et  
4. Password sahəsinə düzgün parol daxil et  
5. Confirm Password sahəsinə eyni parolu daxil et  
6. “Create Account” düyməsinə klik et  

**Expected Result:** Sistem qeydiyyata icazə verməməlidir  

**Actual Result:** Sistem boş name ilə qeydiyyata icazə verdi  

**Status:** Failed (Bug)  

---

## Pixelmart tətbiqində aşkarlanmış bug-ların siyahısı

---

Bug ID: BUG_LOGIN_01  
 Test Case ID: TC_LOGIN_03  
 Title: Yanlış email və parol ilə login mümkündür  
 Status: Açıq  

---

Bug ID: BUG_LOGIN_02  
 Test Case ID: TC_LOGIN_04  
 Title: İstifadəçi yanlış formatda məlumatlarla sistemə daxil ola bildi   
 Status: Açıq  

---

Bug ID: BUG_CART_01  
 Test Case ID: TC_CART_03  
 Title: Məhsul sayı mənfi dəyərə qədər azaldılır  
 Status: Açıq  

---

Bug ID: BUG_SIGNUP_01  
 Test Case ID: TC_SIGNUP_08  
 Title: Name sahəsinə yalnız rəqəmlərlə qeydiyyat mümkündür  
 Status: Açıq  

---

Bug ID: BUG_SIGNUP_02  
 Test Case ID: TC_SIGNUP_09  
 Title: Name sahəsinə xüsusi simvollarla qeydiyyat mümkündür  
 Status: Açıq  

---

Bug ID: BUG_SIGNUP_03  
 Test Case ID: TC_SIGNUP_10  
 Title: Name sahəsinə boşluq ilə qeydiyyat mümkündür  
 Status: Açıq  
