# Cyclic

Smell ini terjadi kita ada class / dependencies yang bergantung satu sama lain secara langsung / tidak langsung yang mengakibatkan terjadi nya **Cyclic**. Biasanya melanggar [Acyclic Dependencies Principle (ADP)](https://en.wikipedia.org/wiki/Acyclic_dependencies_principle)

Dependency memiliki beberapa bentuk:
1. Sebagai member
    ```
    public class A{
        private B b;
    }
    ```
2. Sebagai parameter
    ```
    public class A{
        public void baz(B b){
            //...
        }
    }
    ```
3. Sebagai harcode
    ```
    public class A{
        public void foo(){
            B b = new B()
        }
    }
    ```

### Penyebab
1. Developer ga sadar
2. Passing self reference -> ``bar(this)``;
3. Mau pake callback function
4. Susah di visualisasi karga ga sengaja (cuma mikir di otak ga di gambar)
