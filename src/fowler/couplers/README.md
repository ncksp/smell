# Couplers

Semua smell di dalam grup ini berkaitan dengan coupling yang tinggi. 

Seperti yang telah Anda pelajari di matakuliah Program Design Methods di semester sebelumnya, code yang baik memiliki coupling yang dibuat serendah mungkin antar modulnya, dan memiliki cohesion yang dibuat setinggi mungkin di dalam modulnya. Untuk review, silakan baca [link ini](https://www.geeksforgeeks.org/software-engineering-coupling-and-cohesion/).

- [Feature Envy](feature_envy) -> kelas lain lebih sering pake drpd kelas itu sendiri
- [Inappropriate Intimacy](inappropriate_intimacy) -> kelas lain bisa pake method kelas itu yang sifatnya pribadi (add, edit dll)
- [Message Chains](message_chains) -> method beruntun
- [Middle Man](middle_man) -> cuma delegasi class lain
