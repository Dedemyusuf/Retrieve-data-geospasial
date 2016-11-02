RESUME RETRIEVE DATA GEOSPASIAL PERTEMUAN 3

Ada beberapa cara untuk menentukan titik koordinat menggunakan softwarem, ada 2 software yaitu Python dan QGS (Quantum Global Sulition). Di antara 2 sotware ini sangat di andalkan saat mencari titik koordinat, nah tutorialnya ada di bawah ini cara membaca file shp atau bisa membuat suatu class.

SHP adalah file yang berada dalam shapefile yang menyimpan data geometri.

Dalam file shp terdapat beberapa data :

1.  Bbox

2.  Point

3.  Shapetype

Membaca jumlah data geometri dengan PYTHON

&gt;&gt; import shapefile

&gt;&gt; sf = shapefile.Reader(“namafile.shp”)

&gt;&gt; sf.shapes()

&gt;&gt;a = sf.shapes()

&gt;&gt;len(a)

DBF adalah sebuah file menyimpan file tabular yang menyimpan data tersebut bisa menggunakan variabel dan juga bisa tidak menggunakan variable

Membac file DBF dengan variable

> &gt;&gt; import shapefile

&gt;&gt; geom = sf.records()

&gt;&gt; geom

Membac file DBF tanpa variable

> &gt;&gt; import shapefile

&gt;&gt; sf.records()

Dibawah ini koding membuat class

Import shapefile

> Class Gede(object):
>
> Def hitungbaris(self.namafile):
>
> Sf = shapefile.Reader(namafile)
>
> Rec = sf.shapes()
>
> Return len(rec)

Dengan mendapatan data shp telah disediakan belum tentu dapat membaca data tersebut secara langsung oleh software untuk melihat data tersebut
