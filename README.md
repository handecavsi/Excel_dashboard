# Excel_dashboard
Sık Kullandığım excel formülleri ile dashboard hazırlama

Kullanılan genel formül tipleri:

=ÇOKETOPLA(data!$S:$S;data!$E:$E;'1'!$E$11;data!$F:$F;'1'!$C$19;data!$G:$G;'1'!$B22;data!$N:$N;'1'!$G$11)
=İNDİS(J20:J22;KAÇINCI(MAK(K20:K22);K20:K22;0))
=EĞERHATA(İNDİS(B23:B34;KAÇINCI(V10;C23:C34;0));İNDİS(B23:B34;KAÇINCI(V10;L23:L34;0)))
=EĞERHATA(ÇOKEĞERORTALAMA(data!$R:$R;data!$V:$V;'4'!$C$20;data!$W:$W;'4'!$B23;data!$N:$N;'4'!$E$15);0)
=DÜŞEYARA($A2;order_location!$A$1:$E$51291;3;0)
=METNEÇEVİR($H2;"aaaa")

2012'de en çok shipping_cost'a sahip kategori
V = Yıl sütunu, T = Shipping_cost sütunu
Maksimum shipping_cost'a sahip ürün kategorisi verilerine ARA fonksiyosu ile 2012 yıl filtresi eklendi:
=ARA(2;1/(MAK((data!$V$2:$V$51291='İç görü çıkarma'!$N$18)*data!$T$2:$T$51291)=data!$T$2:$T$51291);data!$N$2:$N$51291)


