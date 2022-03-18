# Patika Homework Week 6

[Use Local Storage](https://usehooks-ts.com/react-hook/use-local-storage) ornegi baz alinarak gelistirilmis tarayici cookie'sini yoneten bir React hook'udur. TypeScript ile React icin yazilmistir.

## React Icerisinde Kullanimi

### Ilk tanimlama ve mevcut degeri alma

```JS
    // Import
    import useCookie from './useCookie.ts';

    // React state gibi tanimlanir
    // Cookie ismi ve baslangic degeri alir.
    // Her iki deger string type olmalidir.
    // Bu tanimlama eger ayni isimle bir cookie mevcutsa bu cookie'nin degerini dondurur.
    // Eger mevcut bir cookie yoksa verilen baslangic degerini doner.
    const [token, setToken, deleteToken] = useCookie('token', '');
```

### Yeni bir Cookie degeri ve suresi tanimlama

```JS
    // Var olan bir cookie'ye yeni bir deger tanimlama
    // Ilk arguman cookie degeridir. Ikinci arguman cookie'nin gecerli olacagi gun sayisidir.
    setToken('1234', 2);
```

### Var olan bir Cookie Silme

```JS
    // Method cagirilarak bu state icin tanimlanmis cookie temizlenir.
    deleteToken();
```
