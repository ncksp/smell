# Wide


Smell ini hierarchy nya class sub class yang extend terlalu melebar ke sambil jadi minim immediate class ditengah tengah nya. Yang bakalan bikin duplicate di subclass subclass nya


misal:

```
             Base

       /     /    \     \
    Deri1 Deri2  DeriA DeriB

    Class deri ngambil semua nya dari base, tapi diliat kalo Deri1, Deri2 punya kemiripan data, tapi DeriA sama DeriB punya kemiripan juga

    Maka akan dibuat

            Base
        /           \
    DeriN         DeriX
Deri1,Deri2     DeriA,DeriB

```
