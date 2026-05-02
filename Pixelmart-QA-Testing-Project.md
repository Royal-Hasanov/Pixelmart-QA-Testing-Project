# Pixelmart QA Testing Project (Task 03)

# TEST SUITE 1: Login

Test Case ID: TC_LOGIN_01
Title: "Sign In" düyməsinə klik edildikdə istifadəçinin login səhifəsinə yönləndirilməsi
Prioritet: Yüksək
Pre-condition: İstifadəçi Pixelmart saytının əsas səhifəsindədir
Description: "Sign In" düyməsinə klik edildikdən sonra istifadəçinin login səhifəsinə yönləndirilməsi yoxlanılır
Test Steps:
"Sign In" düyməsini tap
"Sign In" düyməsinə klik et
Expected Result: İstifadəçi login səhifəsinə yönləndirilməlidir Actual Result: Login səhifəsi uğurla açıldı
Status: Passed

Test Case ID: TC_LOGIN_02
Title: Düzgün email və parol daxil edildikdə istifadəçinin şəxsi hesaba daxil olması
 Prioritet: Yüksək
Pre-condition: stifadəçi login səhifəsindədir
Description: İstifadəçinin düzgün (valid) email və parol daxil edərək sistemə uğurla daxil olması yoxlanılır
Test Steps:
Email input sahəsinə klik et
Düzgün (valid) email daxil et
Parol input sahəsinə klik et
Düzgün (valid) parol daxil et
"Sign In" düyməsinə klik et
Expected Result: İstifadəçi uğurla şəxsi hesabına daxil olmalıdır və əsas səhifəyə yönləndirilməlidir
Actual Result: İstifadəçi uğurla şəxsi hesabına daxil oldu və əsas səhifə açıldı
Status: Passed

Test Case ID: TC_LOGIN_03
Title: Yanlış email və parol daxil edildikdə istifadəçinin hesaba daxil ola bilməməsi
 Prioritet: Yüksək
Pre-condition: İstifadəçi login səhifəsindədir
Description: Yanlış (invalid) email və parol daxil edildikdə sistemin istifadəçinin hesaba girişinə icazə verməməsi yoxlanılır
Test Steps:
Email input sahəsinə klik et
Yanlış (invalid) email daxil et
Parol input sahəsinə klik et
Yanlış (invalid) parol daxil et
"Sign In" düyməsinə klik et
Expected Result:  İstifadəçi hesaba daxil olmamalıdır
Actual Result:  İstifadəçi yanlış email və parol ilə hesaba daxil ola bildi
Status: Failed (Bug)

Test Case ID: TC_LOGIN_04
Title: Yanlış (format baxımından uyğun olmayan) email və parol daxil edildikdə istifadəçinin hesaba daxil ola bilməməsi
 Prioritet: Yüksək
Pre-condition: İstifadəçi login səhifəsindədir
Description: Yanlış formatda email və parol daxil edildikdə sistemin girişə icazə verməməsi yoxlanılır
Test Steps:
Email input sahəsinə klik et
Yanlış formatda email daxil et. məsələn: 123456
Parol input sahəsinə klik et
Yanlış parol daxil et.məsələn: 123456789
“Daxil ol” düyməsinə klik et
Expected Result: İstifadəçi hesaba daxil olmamalıdır və Sistem uyğun xəta mesajı göstərməlidir
Actual Result: İstifadəçi yanlış məlumatlarla sistemə daxil ola bildi
Status: Failed (Bug)

# TEST SUITE 2: Səbət (Cart)

Test Case ID:TC_CART_01
Title: "Səbət" düyməsinə klik edildikdə istifadəçinin səbət səhifəsinə yönləndirilməsi
 Prioritet: Yüksək
Pre-condition: İstifadəçi Pixelmart saytının əsas səhifəsindədir
Description: "Səbət" düyməsinə klik edildikdə istifadəçinin səbət səhifəsinə düzgün yönləndirilməsi yoxlanılır
Test Steps:
Səhifədə "Səbət" düyməsini tap
"Səbət" düyməsinə klik et
Expected Result: İstifadəçi səbət səhifəsinə yönləndirilməlidir
Actual Result: "Səbət" düyməsinə klik edildikdə səbət səhifəsi uğurla açıldı
Status: Passed

Test Case ID: TC_CART_02
Title: Bir neçə məhsul səbətə əlavə edildikdə səbət ikonunda məhsul sayının düzgün göstərilməsi
 Prioritet: Yüksək
Pre-condition: İstifadəçi Pixelmart saytının əsas səhifəsindədir
Description:  İstifadəçinin bir neçə məhsulu səbətə əlavə etdikdə səbət səhifəsində və səbət ikonunda məhsul sayının düzgün göstərilməsi yoxlanılır
Test Steps:
İstənilən məhsul səhifəsini aç
“Səbətə əlavə et” düyməsinə klik et
Başqa bir məhsul seç və onun səhifəsini aç
Yenidən “Səbətə əlavə et” düyməsinə klik et
Səhifənin yuxarı hissəsindəki səbət ikonunu yoxla
Səbət səhifəsinə keç
Expected Result: Səbət ikonunda əlavə olunan məhsulların sayı düzgün göstərilməlidir və səbət səhifəsində bütün əlavə olunmuş məhsullar siyahı şəklində görünməlidir
Actual Result: Səbət ikonunda və səbət səhifəsində əlavə olunan məhsullar düzgün şəkildə göstərildi
Status: Passed

Test Case ID: TC_CART_03
Title: Səbətdə məhsul sayının “+” və “−” düymələri ilə artırılması və azaldılması
 Prioritet: Yüksək
Pre-condition: İstifadəçi Pixelmart saytının əsas səhifəsindədir
Description:
 Səbətə əlavə olunmuş məhsulun sayının “+” və “−” düymələri vasitəsilə düzgün artırılıb-azaldılması yoxlanılır
Test Steps:
İstənilən məhsulu seç və səhifəsini aç
“Səbətə əlavə et” düyməsinə klik et
Səbət səhifəsinə keç
Məhsulun qarşısındakı “+” düyməsinə klik et
Məhsul sayının artdığını yoxla
“−” düyməsinə klik et
Məhsul sayının azaldığını yoxla
Məhsul sayını 1-dən 0-a endir
Expected Result:
“+” düyməsi ilə məhsul sayı artmalıdır və “−” düyməsi ilə məhsul sayı azalmalıdır 
Actual Result: Məhsul sayı azaldılarkən mənfi dəyərə qədər azaldı
Status: Failed (Bug)

# TEST SUITE 3: Sign Up

Test Case ID: TC_SIGNUP_03
Title: Password və Confirm Password eyni olduqda istifadəçinin uğurla qeydiyyatdan keçməsi
 Prioritet: Yüksək
Pre-condition:  İstifadəçi Pixelmart saytının əsas səhifəsindədir
Description: İstifadəçi bütün sahələrə düzgün məlumatlar daxil etdikdə və Password ilə Confirm Password eyni olduqda sistemin uğurla qeydiyyat yaratması yoxlanılır
Test Steps:
Pixelmart saytının əsas səhifəsini aç
“Sign In” düyməsinə klik et
Açılan səhifədə “Create account” linkinə klik et
Name sahəsinə düzgün ad daxil et
Email sahəsinə düzgün email daxil et
Phone sahəsinə düzgün nömrə daxil et
Password sahəsinə düzgün parol daxil et
Confirm Password sahəsinə eyni parolu daxil et
“Create Account” düyməsinə klik et
Expected Result:
İstifadəçi uğurla qeydiyyatdan keçməlidir və Sistem yeni hesab yaratmalıdır,İstifadəçi şəxsi hesab səhifəsinə yönləndirilməlidir
Actual Result:  İstifadəçi uğurla qeydiyyatdan keçdi və şəxsi hesab səhifəsi açıldı
Status: Passed

Test Case ID: TC_SIGNUP_08
Title: Name sahəsinə yalnız rəqəmlər daxil edildikdə qeydiyyatın mümkün olmaması
 Prioritet: Yüksək
Pre-condition: İstifadəçi Sign Up səhifəsindədir
Description:  Name sahəsinə yalnız rəqəmlər daxil edildikdə sistemin bunu qəbul etməməsi yoxlanılır
Test Steps:
Name sahəsinə 123456 daxil et
Email sahəsinə düzgün email daxil et
Phone sahəsinə düzgün nömrə daxil et
Password sahəsinə düzgün parol daxil et
Confirm Password sahəsinə eyni parolu daxil et
“Create Account” düyməsinə klik et
Expected Result: Sistem qeydiyyata icazə verməməlidir
Actual Result: Sistem yalnız rəqəmlərlə daxil edilmiş name ilə qeydiyyata icazə verdi
Status: Failed (Bug)

Test Case ID:  TC_SIGNUP_09
Title: Name sahəsinə xüsusi simvollar daxil edildikdə qeydiyyatın mümkün olmaması
 Prioritet: Yüksək
Pre-condition:
 İstifadəçi Sign Up səhifəsindədir
Description:
 Name sahəsinə xüsusi simvollar daxil edildikdə sistemin bunu qəbul etməməsi yoxlanılır
Test Steps:
Name sahəsinə @#$%^&* daxil et
Email sahəsinə düzgün email daxil et
Phone sahəsinə düzgün nömrə daxil et
Password sahəsinə düzgün parol daxil et
Confirm Password sahəsinə eyni parolu daxil et
“Create Account” düyməsinə klik et
Expected Result: Sistem qeydiyyata icazə verməməlidir
Actual Result:  Sistem xüsusi simvollarla qeydiyyata icazə verdi
Status: Failed (Bug)

Test Case ID:  TC_SIGNUP_10
Title: Name sahəsinə yalnız boşluq daxil edildikdə qeydiyyatın mümkün olmaması
 Prioritet: Yüksək
Pre-condition: İstifadəçi Sign Up səhifəsindədir
Description: Name sahəsinə yalnız boşluqlardan ibarət dəyər daxil edildikdə sistemin bunu qəbul etməməsi yoxlanılır
Test Steps:
Name sahəsinə yalnız boşluq daxil et
Email sahəsinə düzgün email daxil et
Phone sahəsinə düzgün nömrə daxil et
Password sahəsinə düzgün parol daxil et
Confirm Password sahəsinə eyni parolu daxil et
“Create Account” düyməsinə klik et
Expected Result: Sistem qeydiyyata icazə verməməlidir
Actual Result: Sistem boş name ilə qeydiyyata icazə verdi
Status: Failed (Bug)

# Pixelmart tətbiqində aşkarlanmış bug-ların siyahısı

Bug ID: BUG_LOGIN_01
 Test Case ID: TC_LOGIN_03
 Title: Yanlış email və parol ilə login mümkündür
 Status: Açıq

Bug ID: BUG_LOGIN_02
 Test Case ID: TC_LOGIN_04
 Title: Yanlış formatlı email ilə login mümkündür
 Status: Açıq

Bug ID: BUG_CART_01
 Test Case ID: TC_CART_03
 Title: Məhsul sayı mənfi dəyərə qədər azaldılır
 Status: Açıq

Bug ID: BUG_SIGNUP_01
 Test Case ID: TC_SIGNUP_08
 Title: Name sahəsinə yalnız rəqəmlərlə qeydiyyat mümkündür
 Status: Açıq

Bug ID: BUG_SIGNUP_02
 Test Case ID: TC_SIGNUP_09
 Title: Name sahəsinə xüsusi simvollarla qeydiyyat mümkündür
 Status: Açıq

Bug ID: BUG_SIGNUP_03
 Test Case ID: TC_SIGNUP_10
 Title: Name sahəsinə boşluq ilə qeydiyyat mümkündür
 Status: Açıq
