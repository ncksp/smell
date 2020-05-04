# Leaky

Access modifier sebuah method atau field yang udah sesuai dengan kebutuhan tetapi ada method lain yang public mengekspos atau ngebocorin implementasi detail nya

### Penyebab 

1. **Lack of awareness of what should be “hidden”** : Biasanya developernya ceroboh dan gak dasar yang itu harus disembunyiin. Atau designner nya kurang berpengalaman yang bikin datanya bisa bocor dan bisa di leak
    #### Solusi
        - Jangan pernah return sesuatu yang shallow copy, kayak return list. Karna reference nya akan sama, ubah menjadi deep copy

2. **Viscosity**: Developer dan designer dikejar deadline jadi buru buru

3. **Use of fine-grained interface**: Terlalu lengkap bisa set dan get apapun


### When to ignore
