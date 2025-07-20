# python-algorithm
python algorithm examples

<h1>🧠 Python Algoritma Örnekleri</h1>

<p>Bu belgede temel Python algoritmalarına dair örnekler yer almaktadır. Her örnek açıklamalı şekilde hazırlanmıştır.</p>

<hr>

<details>
  <summary><strong>🔁 1. Faktöriyel Hesaplama (Recursive)</strong></summary>

  <pre><code class="language-python">
def faktoriyel(n):
    if n == 0 or n == 1:
        return 1
    return n * faktoriyel(n - 1)

print(faktoriyel(5))  # Çıktı: 120
  </code></pre>
</details>

<details>
  <summary><strong>🔁 2. Fibonacci Serisi (İteratif)</strong></summary>

  <pre><code class="language-python">
def fibonacci(n):
    a, b = 0, 1
    for _ in range(n):
        print(a, end=" ")
        a, b = b, a + b

fibonacci(10)  # Çıktı: 0 1 1 2 3 5 8 13 21 34
  </code></pre>
</details>

<details>
  <summary><strong>🔁 3. Asal Sayı Kontrolü</strong></summary>

  <pre><code class="language-python">
def asal_mi(sayi):
    if sayi <= 1:
        return False
    for i in range(2, int(sayi ** 0.5) + 1):
        if sayi % i == 0:
            return False
    return True

print(asal_mi(13))  # Çıktı: True
  </code></pre>
</details>

<details>
  <summary><strong>🔁 4. Dizi Elemanlarını Ters Çevirme</strong></summary>

  <pre><code class="language-python">
def ters_cevir(liste):
    return liste[::-1]

print(ters_cevir([1, 2, 3, 4]))  # Çıktı: [4, 3, 2, 1]
  </code></pre>
</details>

<details>
  <summary><strong>🔁 5. En Büyük Ortak Bölen (EBOB)</strong></summary>

  <pre><code class="language-python">
def ebob(a, b):
    while b:
        a, b = b, a % b
    return a

print(ebob(24, 36))  # Çıktı: 12
  </code></pre>
</details>

<details>
  <summary><strong>🔁 6. Palindrom Kontrolü</strong></summary>

  <pre><code class="language-python">
def palindrom_mu(metin):
    return metin == metin[::-1]

print(palindrom_mu("kayak"))  # Çıktı: True
  </code></pre>
</details>

<details>
  <summary><strong>🔁 7. Liste Elemanlarını Toplama</strong></summary>

  <pre><code class="language-python">
def toplam(liste):
    return sum(liste)

print(toplam([1, 2, 3, 4]))  # Çıktı: 10
  </code></pre>
</details>

<details>
  <summary><strong>🔁 8. Bubble Sort (Kabarcık Sıralama)</strong></summary>

  <pre><code class="language-python">
def bubble_sort(liste):
    n = len(liste)
    for i in range(n):
        for j in range(0, n-i-1):
            if liste[j] > liste[j+1]:
                liste[j], liste[j+1] = liste[j+1], liste[j]
    return liste

print(bubble_sort([5, 2, 9, 1]))  # Çıktı: [1, 2, 5, 9]
  </code></pre>
</details>

<details>
  <summary><strong>🔁 9. Binary Search (İkili Arama)</strong></summary>

  <pre><code class="language-python">
def binary_search(liste, hedef):
    low = 0
    high = len(liste) - 1

    while low <= high:
        mid = (low + high) // 2
        if liste[mid] == hedef:
            return mid
        elif liste[mid] < hedef:
            low = mid + 1
        else:
            high = mid - 1
    return -1

print(binary_search([1, 3, 5, 7, 9], 5))  # Çıktı: 2
  </code></pre>
</details>

<details>
  <summary><strong>🔁 10. Anagram Kontrolü</strong></summary>

  <pre><code class="language-python">
def anagram_mi(s1, s2):
    return sorted(s1) == sorted(s2)

print(anagram_mi("elma", "amel"))  # Çıktı: True
  </code></pre>
</details>

<hr>

<hr>

<p><strong>✍️ Hazırlayan:</strong> Ömer Faruk<br>
📁 <a href="https://github.com/omerfaruk-shp" target="_blank">GitHub: omerfaruk-shp</a></p>

