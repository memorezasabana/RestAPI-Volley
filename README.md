[![Android RestAPI](https://img.shields.io/badge/Android%20RestAPI-Volley--Library-brightgreen.svg?style=flat)](https://developer.android.com/training/volley?hl=id)

## What is Volley?
Volley adalah library HTTP yang mempermudah dan, yang terpenting, mempercepat networking untuk aplikasi Android.

## Volley menawarkan manfaat-manfaat berikut:
- [x] Penjadwalan otomatis permintaan jaringan.
- [x] Beberapa koneksi jaringan serentak.
- [x] Caching respons disk dan memori transparan dengan koherensi cache HTTP standar.
- [x] Dukungan untuk pemrioritasan permintaan.
- [x] API permintaan pembatalan. Anda bisa membatalkan satu permintaan, atau menetapkan blok atau cakupan permintaan untuk dibatalkan.
- [x] Kemudahan kustomisasi, misalnya, untuk mencoba ulang dan backoff.
- [x] Pemesanan kuat yang memudahkan pengisian UI Anda dengan benar menggunakan data yang diambil secara asinkron dari jaringan.
- [x] Fitur proses debug dan penelusuran.

##  Cara menambahkan Volley ke project:
1. Create new project.
2. Open build.gradle(Module: app) and add the following dependency:
```java
  dependencies {
        ...
        implementation 'com.android.volley:volley:1.1.1'
    }
```
3. In AndroidManifest.xml add the internet permission:
```java
 <uses-permission
    android:name="android.permission.INTERNET />"
```

## Classes in Volley Library:
- Request Queue:
> Digunakan untuk mengirimkan permintaan ke jaringan. Seseorang dapat membuat Request Queue sesuai permintaan jika diperlukan, 
tetapi biasanya dibuat sejak dini, pada waktu mulai, dan menyimpannya dan menggunakannya sebagai Singleton.
- Request: 
>  Semua informasi yang diperlukan untuk melakukan panggilan API web disimpan di dalamnya. Ini adalah dasar untuk membuat permintaan jaringan (GET, POST).

## Types of Request using Volley Library:
- String Request
```java
String url = "https:// string_url/";
StringRequest
	stringRequest
	= new StringRequest(
		Request.Method.GET,
		url,
		new Response.Listener() {
			@Override
			public void onResponse(String response)
			{
			}
		},
		new Response.ErrorListener() {
			@Override
			public void onErrorResponse(VolleyError error)
			{
			}
		});
requestQueue.add(stringRequest);
</pre>
```
- JSONArray Request
```java
JsonArrayRequest
	jsonArrayRequest
	= new JsonArrayRequest(
		Request.Method.GET,
		url,
		null,
		new Response.Listener() {
			@Override
			public void onResponse(JSONArray response)
			{
			}
		},
		new Response.ErrorListener() {
			@Override
			public void onErrorResponse(VolleyError error)
			{
			}
		});
requestQueue.add(jsonArrayRequest);
```

## JSON
> JSON (JavaScript Object Notation) adalah format pertukaran data yang ringan, mudah
dibaca dan ditulis oleh manusia, serta mudah diterjemahkan dan dibuat (generate) oleh komputer.
Format ini dibuat berdasarkan bagian dari Bahasa Pemprograman JavaScript. JSON merupakan
format teks yang tidak bergantung pada bahasa pemprograman apapun karena menggunakan
gaya bahasa yang umum digunakan oleh programmer keluarga C termasuk C, C++, C#, Java,
JavaScript, Perl, Python dll. Oleh karena sifat-sifat tersebut, menjadikan JSON ideal sebagai
bahasa pertukaran-data.

## DotaAPI Project
SplashScreen | Menu Utama | Full Project
--- | --- | ---
![splashscreen] | ![menu_utama] | ![full_project]

[splashscreen]: https://github.com/memorezasabana/abcd/blob/main/DotaApi/ss.jpg
[menu_utama]: https://github.com/memorezasabana/abcd/blob/main/DotaApi/menuawal.jpg
[full_project]: https://github.com/memorezasabana/abcd/blob/main/DotaApi/Video.gif
