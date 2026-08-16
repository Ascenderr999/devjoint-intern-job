
# Mənzil Qiyməti Proqnozu — Biznes Hesabatı

Tarix: 16.08.2026
Data mənbəyi: Bina.az satış elanları
Analiz edilən elan sayı: 99,870

## 1. Hansı problemi həll edirik?

Platformada qiyməti elan sahibi özü təyin edir. Bunun iki nəticəsi var: bazardan baha
qoyulan elanlar aylarla satılmır, ucuz qoyulanlar isə satıcıya birbaşa itki verir.
Alıcı üçün də hansı elanın sərfəli olduğunu anlamaq çətindir.

Biz mənzilin obyektiv xüsusiyyətlərinə əsaslanaraq bazar qiymətini avtomatik hesablayan
bir sistem hazırladıq.

## 2. Nə etdik?

Keçmiş elanların 78,861-ni sistemi öyrətmək üçün istifadə etdik. Sistemin heç
vaxt görmədiyi 19,974 elanı isə kənara ayırdıq və yalnız işin sonunda, imtahan
kimi istifadə etdik. Buna görə aşağıdakı rəqəmlər real şəraitdə gözlənilən nəticələrdir,
sistemin öz məşq suallarındakı balı deyil.

Beş fərqli yanaşma sınaqdan keçirildi və tam eyni şərtlərlə müqayisə olundu; ən yaxşısı
seçilib əlavə olaraq incə tənzimləndi.

## 3. Sistem nə qədər dəqiqdir?

| Göstərici | Hazırkı yanaşma (orta qiymət) | Yeni sistem | Fərq |
|---|---|---|---|
| Orta səhv (AZN) | 192,875 | 23,156 | 88% daha az səhv |
| Faizlə orta səhv | 72% | 2% | — |
| İzah olunan qiymət fərqi | 0% | 58% | — |

Sadə dillə: sistem bir mənzilin qiymətini orta hesabla 23,156 AZN xəta ilə
təxmin edir.

- Elanların 99%-də proqnoz faktiki qiymətdən ±10% aralığındadır
- Elanların 99%-də ±20% aralığındadır
- Elanların 99%-də ±30% aralığındadır

## 4. Qiyməti ən çox nə müəyyən edir?

Analiz göstərdi ki, qiymətə ən güclü təsir edən amillər bunlardır: total_price, Kateqoriya, Sahə.
Bu, məhsul komandası üçün birbaşa istifadəyə yararlı məlumatdır: elan formasında məhz bu
sahələrin doldurulmasını məcburi etmək proqnozun keyfiyyətini artırar.

## 5. Sistemi harada istifadə edə bilərik?

1. Elan yerləşdirərkən satıcıya "bu xüsusiyyətlərdə mənzillər adətən X–Y AZN aralığında
   satılır" tövsiyəsini göstərmək.
2. Proqnozdan xeyli aşağı qiymətli elanları alıcılara əlverişli təklif kimi təqdim etmək.
3. Proqnozdan kəskin fərqlənən elanları moderasiyaya yönləndirmək.
4. Rayonlar üzrə qiymət dinamikasını izləmək.

## 6. Məhdudiyyətlər

- Sistem yalnız elan formasındakı məlumatları görür. Mənzilin real vəziyyəti, mənzərəsi,
  qonşuluq və binanın nüfuzu datada yoxdur; səhvlərin bir hissəsi məhz bundan gəlir.
- Elanlarda göstərilən qiymət təklif qiymətidir, real satış qiyməti deyil.
- Sistem keçmiş data üzərində öyrənib. Bazarda kəskin dəyişiklik olarsa proqnozlar
  köhnələcək, ona görə modelin hər 3 ayda bir yeni data ilə yenilənməsini tövsiyə edirik.
- Çox baha və qeyri-standart obyektlərdə səhv daha yüksəkdir, çünki belə elanların sayı azdır.

## 7. Tövsiyə

Sistemi pilot rejimdə, satıcıya tövsiyə olunan qiymət aralığını göstərən köməkçi alət kimi
işə salmağı təklif edirik. Tam avtomatik qiymət təyini üçün hələ tövsiyə etmirik; o mərhələ
üçün real satış qiymətləri və mənzil şəkillərindən alınan əlavə məlumat lazımdır.

Növbəti addımlar: real satış qiymətlərinin toplanması, elan tarixinin əlavə edilməsi ilə
bazar trendinin nəzərə alınması və 3 aylıq pilotdan sonra yenidən qiymətləndirmə.
