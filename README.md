# Moleküler Grafik Oluşturma Projesi

Bu proje, derin öğrenme modelleri kullanarak moleküler grafiklerin (moleküler yapıların temsili) üretimini amaçlar. Aşağıda, kullanılan algoritmalar ve veri setleri hakkında bilgi bulabilirsiniz:

## Kullanılan Algoritmalar

### WGAN-GP (Wasserstein Generative Adversarial Network with Gradient Penalty)
- WGAN-GP, generative adversarial network (GAN) türlerinden biridir. WGAN-GP, GAN'ların eğitim istikrarını artırmak ve modellerin daha iyi öğrenmesini sağlamak için bir tür gradyan cezası tekniği olan gradient penalty'yi kullanır.

### R-GCN (Relational Graph Convolutional Network)
- R-GCN, ilişkisel grafik yapılarını modellemek için kullanılan bir tür grafik konvolüsyon ağıdır. Moleküler grafiklerdeki atomlar arasındaki ilişkileri modellemek için kullanılır.

## Kullanılan Veri Setleri

### QM9 Veri Seti
- QM9 veri seti, MoleculeNet veri setinden elde edilmiştir. Bu veri seti, küçük organik moleküllerin kuantum mekanik hesaplamaları sonuçlarını içerir. Moleküler grafiklerin üretilmesi için SMILES formatında molekül yapıları kullanılmıştır.

### QM8 Veri Seti
- QM8 veri seti, MoleculeNet benchmark'ının bir parçasıdır ve küçük moleküllerin elektronik spektrum ve uyarılmış durum enerjisi kuantum mekanik hesaplamaları sonuçlarını içerir. En fazla sekiz ağır atom içeren moleküller üzerinde bir koleksiyona uygulanan çeşitli yöntemleri içerir.

## Uygulama Detayları

Bu projede, WGAN-GP ve R-GCN'nin birleştirilmesiyle yeni moleküler grafiklerin üretilmesi amaçlanmaktadır. İlk olarak, veri seti üzerinde eğitilmiş bir WGAN-GP modeli kullanılarak yeni moleküller üretilir. Daha sonra, bu moleküller R-GCN ile işlenir ve analiz edilir.


---


# Molecular Graph Generation Project

This project aims to generate molecular graphs (representations of molecular structures) using deep learning models. Below, you can find information about the algorithms and datasets used:

## Algorithms Used

### WGAN-GP (Wasserstein Generative Adversarial Network with Gradient Penalty)
- WGAN-GP is one type of generative adversarial network (GAN). WGAN-GP uses a gradient penalty technique, a type of regularization, to improve the training stability of GANs and allow models to learn better.

### R-GCN (Relational Graph Convolutional Network)
- R-GCN is a type of graph convolutional network used to model relational graph structures. It is used to model relationships between atoms in molecular graphs.

## Datasets Used

### QM9 Dataset
- The QM9 dataset is obtained from the MoleculeNet dataset. This dataset contains quantum mechanical calculations results of small organic molecules. Molecular structures in SMILES format are used for generating molecular graphs.

### QM8 Dataset
- The QM8 dataset is part of the MoleculeNet benchmark and contains quantum mechanical calculations results of electronic spectra and excited state energy of small molecules. It includes multiple methods applied to a collection of molecules with up to eight heavy atoms.

## Application Details

This project aims to generate new molecular graphs by combining WGAN-GP and R-GCN. Initially, new molecules are generated using a WGAN-GP model trained on the dataset. Then, these molecules are processed and analyzed with R-GCN.
