# Siswa
### Create Siswa
<details>
<summary> Klik Untuk Detail </summary>
<table>
<tr>
    <td><b> URL <b></td>
    <td> {{baseURL}}/api/v1/Siswa</td>
</tr>
<tr>
    <td> <b> Method <b></td>
    <td> POST </td>
</tr>
<tr>
    <td><b> Header <b></td>
    <td> Authorization : Bearer Token </td>
</tr>
<tr>
    <td><b> Body <b></td>
    <td> 

``` json
{
    "nama" : "Dino",
    "alamat" : "Cisarua",
    "hobi" : "Animasi"
}
```
</td>
</tr>

<tr>
    <td><b> Respon Success <b></td>
    <td> 

``` json
{
    "code" : 201,
    "message" : "Data Siswa Berhasil diinput",
    "data" : {
    "id" : 1234,
    "nama" : "Dino",
    "alamat" : "Cisarua",
    "hobi" : "Animasi"
    }
}
```

<tr>
    <td><b> Respon Conflict <b></td>
    <td> 

``` json
{
    "code" : 409,
    "message" : "Data Siswa Telah digunakan",
    "data" : {

    "value" : "Dino",
    "property" : "nama",
    "location" : "body"
    }
}
```
</td>
</tr>

</table>
</details>

### Read Siswa By ID

<details>
<summary> Klik Untuk Detail </summary>
<table>
<tr>
    <td><b> URL <b></td>
    <td> {{baseURL}}/api/v1/Siswa</td>
</tr>
<tr>
    <td><b> EXAMPLE <b></td>
    <td> {{baseURL}}/api/v1/Siswa/?id=1234</td>
</tr>
<tr>
    <td> <b> Method <b></td>
    <td> GET </td>
</tr>
<tr>
    <td><b> Header <b></td>
    <td> Authorization : Bearer Token </td>
</tr>
<tr>
    <td><b> Query <b></td>
    <td> id=1234</td>

</tr>
<tr>
    <td><b> Respon Success with Query <b></td>
    <td> 

``` json
{
    "code" : 201,
    "message" : "Sukses",
    "data" : {
    "id" : 1234,
    "nama" : "Dino",
    "alamat" : "Cisarua",
    "hobi" : "Animasi"
    }
}
```
</tr>

<tr>
    <td><b> Respon Not Found <b></td>
    <td> 

``` json
{
    "code" : 404,
    "message" : "Data Siswa Tidak Ditemukan",
    "data" : {

    "value" : "1234",
    "property" : "id",
    "location" : "query"
    }
}
```
</td>
</tr>
</table>
</details>

### Read Siswa By ALL

<details>
<summary> Klik Untuk Detail </summary>
<table>
<tr>
    <td><b> URL <b></td>
    <td> {{baseURL}}/api/v1/Siswa</td>
</tr>

<tr>
    <td> <b> Method <b></td>
    <td> GET </td>
</tr>
<tr>
    <td><b> Header <b></td>
    <td> Authorization : Bearer Token </td>
</tr>
<tr>
    <td><b> Respon Success with Query <b></td>
    <td> 

``` json
{
    "code" : 200,
    "message" : "Sukses",
    "data" : {
    "id" : 1234,
    "nama" : "Dino",
    "alamat" : "Cisarua",
    "hobi" : "Animasi"
    },
    {
    "id" : 1235,
    "nama" : "Ari",
    "alamat" : "Bogor",
    "hobi" : "Tidur"
    }
}
```
</tr>



</table>
</details>

### Update Siswa

<details>
<summary> Klik Untuk Detail </summary>
<table>
<tr>
    <td><b> URL <b></td>
    <td> {{baseURL}}/api/v1/Siswa</td>
</tr>
<tr>
    <td> <b> Method <b></td>
    <td> POST </td>
</tr>
<tr>
    <td><b> Header <b></td>
    <td> Authorization : Bearer Token </td>
</tr>
<tr>
    <td><b> Body <b></td>
    <td> 

``` json
{
    "nama" : "Dino",
    "alamat" : "Cisarua",
    "hobi" : "Animasi"
}
```
</td>
</tr>

<tr>
    <td><b> Respon Success <b></td>
    <td> 

``` json
{
    "code" : 201,
    "message" : "Data Siswa Berhasil Dirubah",
    "data" : {
    "id" : 1234,
    "nama" : "Dino Saurus",
    "alamat" : "Megamendung",
    "hobi" : "Jogging"
    }
}
```

<tr>
    <td><b> Respon Conflict <b></td>
    <td> 

``` json
{
    "code" : 409,
    "message" : "Data Siswa Telah digunakan",
    "data" : {

    "value" : "Dino Saurus",
    "property" : "nama",
    "location" : "body"
    }
}
```
</td>
</tr>

<tr>
    <td><b> Respon Not Found <b></td>
    <td> 

``` json
{
    "code" : 404,
    "message" : "Data Siswa Tidak Ditemukan",
    "data" : {

    "value" : "Dino Saurus",
    "property" : "nama",
    "location" : "query"
    }
}
```
</td>
</tr>

</table>
</details>

### Delete Siswa

<details>
<summary> Klik Untuk Detail </summary>
<table>
<tr>
    <td><b> URL <b></td>
    <td> {{baseURL}}/api/v1/Siswa</td>
</tr>
<tr>
    <td><b> EXAMPLE <b></td>
    <td> {{baseURL}}/api/v1/Siswa/?id=1234</td>
</tr>
<tr>
    <td> <b> Method <b></td>
    <td> DELETE </td>
</tr>
<tr>
    <td><b> Header <b></td>
    <td> Authorization : Bearer Token </td>
</tr>
<tr>
    <td><b> Query <b></td>
    <td> id=1234</td>

</tr>
<tr>
    <td><b> Respon Success with Query <b></td>
    <td> 

``` json
{
    "code" : 201,
    "message" : "Sukses Dihapus",
    "data" : []
}
```
</tr>

<tr>
    <td><b> Respon Not Found <b></td>
    <td> 

``` json
{
    "code" : 404,
    "message" : "Data Siswa Tidak Ditemukan",
    "data" : {

    "value" : "1234",
    "property" : "id",
    "location" : "query"
    }
}
```
</td>
</tr>
</table>
</details>

# Guru
### Create Guru
<details>
<summary> Klik Untuk Detail </summary>
<table>
<tr>
    <td><b> URL <b></td>
    <td> {{baseURL}}/api/v1/Guru</td>
</tr>
<tr>
    <td> <b> Method <b></td>
    <td> POST </td>
</tr>
<tr>
    <td><b> Header <b></td>
    <td> Authorization : Bearer Token </td>
</tr>
<tr>
    <td><b> Body <b></td>
    <td> 

``` json
{
    "nama" : "Aldi",
    "alamat" : "Cisarua",
    "hobi" : "Animasi"
}
```
</td>
</tr>

<tr>
    <td><b> Respon Success <b></td>
    <td> 

``` json
{
    "code" : 201,
    "message" : "Data Guru Berhasil diinput",
    "data" : {
    "id" : 123,
    "nama" : "Aldi",
    "alamat" : "Cisarua",
    "hobi" : "Animasi"
    }
}
```

<tr>
    <td><b> Respon Conflict <b></td>
    <td> 

``` json
{
    "code" : 409,
    "message" : "Data Guru Telah digunakan",
    "data" : {

    "value" : "Aldi",
    "property" : "nama",
    "location" : "body"
    }
}
```
</td>
</tr>

</table>
</details>

### Read Guru By ID

<details>
<summary> Klik Untuk Detail </summary>
<table>
<tr>
    <td><b> URL <b></td>
    <td> {{baseURL}}/api/v1/Guru</td>
</tr>
<tr>
    <td><b> EXAMPLE <b></td>
    <td> {{baseURL}}/api/v1/Guru/?id=123</td>
</tr>
<tr>
    <td> <b> Method <b></td>
    <td> GET </td>
</tr>
<tr>
    <td><b> Header <b></td>
    <td> Authorization : Bearer Token </td>
</tr>
<tr>
    <td><b> Query <b></td>
    <td> id=123</td>

</tr>
<tr>
    <td><b> Respon Success with Query <b></td>
    <td> 

``` json
{
    "code" : 201,
    "message" : "Sukses",
    "data" : {
    "id" : 123,
    "nama" : "Aldi",
    "alamat" : "Cisarua",
    "hobi" : "Animasi"
    }
}
```
</tr>

<tr>
    <td><b> Respon Not Found <b></td>
    <td> 

``` json
{
    "code" : 404,
    "message" : "Data Guru Tidak Ditemukan",
    "data" : {

    "value" : "123",
    "property" : "id",
    "location" : "query"
    }
}
```
</td>
</tr>
</table>
</details>

### Read Guru By ALL

<details>
<summary> Klik Untuk Detail </summary>
<table>
<tr>
    <td><b> URL <b></td>
    <td> {{baseURL}}/api/v1/Guru</td>
</tr>

<tr>
    <td> <b> Method <b></td>
    <td> GET </td>
</tr>
<tr>
    <td><b> Header <b></td>
    <td> Authorization : Bearer Token </td>
</tr>
<tr>
    <td><b> Respon Success with Query <b></td>
    <td> 

``` json
{
    "code" : 200,
    "message" : "Sukses",
    "data" : {
    "id" : 123,
    "nama" : "Aldi",
    "alamat" : "Cisarua",
    "hobi" : "Animasi"
    },
    {
    "id" : 124,
    "nama" : "Odi",
    "alamat" : "Bogor",
    "hobi" : "Tidur"
    }
}
```
</tr>



</table>
</details>

### Update Guru

<details>
<summary> Klik Untuk Detail </summary>
<table>
<tr>
    <td><b> URL <b></td>
    <td> {{baseURL}}/api/v1/Guru</td>
</tr>
<tr>
    <td> <b> Method <b></td>
    <td> POST </td>
</tr>
<tr>
    <td><b> Header <b></td>
    <td> Authorization : Bearer Token </td>
</tr>
<tr>
    <td><b> Body <b></td>
    <td> 

``` json
{
    "nama" : "Aldi",
    "alamat" : "Cisarua",
    "hobi" : "Animasi"
}
```
</td>
</tr>

<tr>
    <td><b> Respon Success <b></td>
    <td> 

``` json
{
    "code" : 201,
    "message" : "Data Guru Berhasil Dirubah",
    "data" : {
    "id" : 123,
    "nama" : "Aldi Ogi",
    "alamat" : "Megamendung",
    "hobi" : "Jogging"
    }
}
```

<tr>
    <td><b> Respon Conflict <b></td>
    <td> 

``` json
{
    "code" : 409,
    "message" : "Data Guru Telah digunakan",
    "data" : {

    "value" : "Aldi Ogi",
    "property" : "nama",
    "location" : "body"
    }
}
```
</td>
</tr>

<tr>
    <td><b> Respon Not Found <b></td>
    <td> 

``` json
{
    "code" : 404,
    "message" : "Data Guru Tidak Ditemukan",
    "data" : {

    "value" : "Aldi Ogi",
    "property" : "nama",
    "location" : "query"
    }
}
```
</td>
</tr>

</table>
</details>

### Delete Guru

<details>
<summary> Klik Untuk Detail </summary>
<table>
<tr>
    <td><b> URL <b></td>
    <td> {{baseURL}}/api/v1/Guru</td>
</tr>
<tr>
    <td><b> EXAMPLE <b></td>
    <td> {{baseURL}}/api/v1/Guru/?id=123</td>
</tr>
<tr>
    <td> <b> Method <b></td>
    <td> DELETE </td>
</tr>
<tr>
    <td><b> Header <b></td>
    <td> Authorization : Bearer Token </td>
</tr>
<tr>
    <td><b> Query <b></td>
    <td> id=123</td>

</tr>
<tr>
    <td><b> Respon Success with Query <b></td>
    <td> 

``` json
{
    "code" : 201,
    "message" : "Sukses Dihapus",
    "data" : []
}
```
</tr>

<tr>
    <td><b> Respon Not Found <b></td>
    <td> 

``` json
{
    "code" : 404,
    "message" : "Data Guru Tidak Ditemukan",
    "data" : {

    "value" : "123",
    "property" : "id",
    "location" : "query"
    }
}
```
</td>
</tr>
</table>
</details>