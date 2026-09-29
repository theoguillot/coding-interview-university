# Mon plan — Big tech (SWE fullstack) + Python + Cybersécu dev

**Durée** : 44 semaines (~10 mois), dont 5 semaines tampon
**Rythme** : 13 h / semaine = 3 jours courts (1 h) + 2 jours longs (5 h)
**Langage d'entretien** : Python — **Liste de problèmes** : [NeetCode 150](https://neetcode.io/practice) (vidéo de solution pour chaque problème)
**Postes visés en priorité** : Frontend / Fullstack SWE (là où ~5 ans d'expérience front comptent pleinement)

Coche les cases au fur et à mesure (`[x]`), comme le recommande le README.

| Piste | Semaines | Heures |
|---|---|---|
| Algo (y compris entretien du niveau et mocks en phase 4) | 1-44 | ~295 h |
| [Projet perso](#piste-projet) | 1-44 | ~95 h |
| [Cybersécu dev](#piste-cyber) | 3-35 | ~62 h |
| System design (dont ~15 h de frontend system design) | 23-44 | ~50 h |
| [Rounds frontend](#piste-rounds-frontend) | 3-22 | ~30 h |
| Réseau, design OO, testing | 34 | ~5 h |
| Observabilité | 35 | ~6 h |
| Behavioral | 36-44 | ~10 h |
| Installation et Python | 1-2 | ~7 h |
| [Journal d'impact](#journal-dimpact) | 1-44 | 10 min / semaine |

En cas de retard : voir [l'ordre de coupe](#si-tu-prends-du-retard).

---

## La méthode (tirée du README)

| Principe du repo | Ce que ça donne concrètement |
|---|---|
| **Daily Plan** : un sujet → vidéos → implémentation | Jour long 1 : vidéos du repo puis implémentation en Python avec tests |
| **« Do coding interview questions while you're learning »** : 2-3 questions par sujet, puis y revenir plus tard | Jour long 1 : problèmes du sujet en cours. Jours courts et jour long 2 : problèmes **ratés** et sujets **anciens** |
| **« You won't remember it all »** + **flashcards** (Anki, tes propres cartes, pas celles de l'auteur) | 10 min d'Anki au début de **chaque** jour. 5-10 cartes créées par sujet |
| **Coding Question Practice** : papier/tableau d'abord, puis ordinateur | 1 problème par semaine résolu sur papier, en parlant à voix haute, puis tapé et testé |
| **Final Review** : vidéos courtes de révision | Une vidéo `[Review]` / Michael Sambol d'un sujet ancien chaque semaine |

### Semaine type (phases 0 à 3, semaines 1-30)

Les jours courts servent à la **répétition espacée** (peu de temps mais fréquent, c'est ce qui fait retenir). Les jours longs servent à **apprendre du neuf** et à **construire**.

| Jour | Durée | Contenu |
|---|---|---|
| Court A | 1 h | Anki · refaire **de zéro** 1-2 problèmes ratés (J+3 / J+7 / J+30) |
| Court B | 1 h | Anki · 1 problème d'un sujet ancien, ou vidéo `[Review]` + 1 problème facile |
| Court C | 1 h | Anki · [cyber](#piste-cyber) : 1 lab PortSwigger |
| **Long 1** | 5 h | Anki · **Algo — apprendre** (2 h) : vidéos du repo + implémentation · pause · **Algo — pratiquer** (2 h) : 3 problèmes NeetCode du sujet · pause · **Cyber** (1 h) : théorie du sujet de la semaine |
| **Long 2** | 5 h | Anki · **Algo** (1 h) : 1 problème sur papier + 1 problème du sujet · pause · **[Projet](#piste-projet)** (2h30) · pause · **[Rounds frontend](#piste-rounds-frontend)** (1h30) · **[Journal d'impact](#journal-dimpact)** (10 min) |

**Répartition** : algo ~7 h · projet 2h30 · cyber 2 h · frontend 1h30.

**Conseils pour les jours longs** :
- Travaille par blocs de 1h30 max avec 15 min de pause. Au-delà de ~5 h de travail concentré, le rendement chute nettement : « pas de limite » ne veut pas dire faire 8 h.
- L'algo le matin, le projet plus tard dans la journée (moins coûteux mentalement).
- Évite deux jours longs consécutifs : espacés, ils profitent mieux de la répétition espacée. Exemple : lun court · mar court · **mer long** · jeu court · **sam long**.

### Semaine type (phase 4, semaines 31-44)

| Jour | Durée | Contenu |
|---|---|---|
| Court A | 1 h | Anki · refaire 1-2 problèmes |
| Court B | 1 h | Anki · 1 problème tagué entreprise |
| Court C | 1 h | Cyber (jusqu'à S35), puis behavioral (répéter une histoire STAR à voix haute) |
| **Long 1** | 5 h | **Thème de la semaine** (2h30) · **mock** ou problèmes chronométrés (2h30) |
| **Long 2** | 5 h | Algo (1h30) · projet : finitions et démo (1h30) · thème de la semaine (2 h) · journal d'impact (10 min) |

### Règles pour un problème

1. Lis l'énoncé, reformule, donne un exemple et les cas limites.
2. **25 min max** de recherche. Bloqué → vidéo NeetCode, puis recode sans regarder.
3. Donne la complexité temps/mémoire.
4. Note-le dans le [journal](#journal-des-problèmes) : pattern, réussi seul ? À refaire à J+3, J+7, J+30 si raté.
5. Une carte Anki « signal → pattern » (ex. : *« sous-tableau contigu + contrainte » → fenêtre glissante*).

Les semaines chargées en problèmes (ex. : Linked Lists, DP 1D) : ce qui ne tient pas passe dans la semaine suivante ou dans la prochaine semaine tampon.

### Si tu prends du retard

Coupe dans cet ordre :
1. Cyber : logique métier, upload, API (S23-25)
2. Projet : jalon 7 (finitions de la vitrine)
3. Rounds frontend : 4 utilitaires au lieu de 8
4. Problèmes *hard* et bonus de NeetCode

**Ne jamais couper** : les révisions (jours courts, refaire les ratés), le system design, les mocks.

---

## Piste algo

### Phase 0 — Mise en place, Python, Big-O (semaines 1-2)

#### Semaine 1 — Installation et Python
- [ ] Forker le repo et travailler sur une branche ([How to use it](README.md#how-to-use-it))
- [ ] Python 3 + `pytest` installés, dossier `practice/` pour tes implémentations
- [ ] Comptes LeetCode + NeetCode, Anki installé
- [ ] [Python in One Video](https://www.youtube.com/watch?v=N4mEzFDjqtA) (en accéléré, tu connais déjà la programmation)
- [ ] Lire [Coding Interview Python Language Essentials](extras/cheat%20sheets/Coding%20Interview%20Python%20Language%20Essentials.pdf) et le [Python cheat sheet](extras/cheat%20sheets/python-cheat-sheet-v1.pdf)
- [ ] [10 Tips for Pythonic Code](https://www.youtube.com/watch?v=_O23jIXsshs)
- [ ] Maîtriser : `list` (slicing, compréhensions), `dict`, `set`, `tuple`, `sorted(key=...)`, `enumerate`, `zip`
- [ ] `collections` : `deque`, `Counter`, `defaultdict` · `heapq` · `bisect`

#### Semaine 2 — Big-O ([section du repo](README.md#algorithmic-complexity--big-o--asymptotic-analysis))
- [ ] [Harvard CS50 - Asymptotic Notation](https://www.youtube.com/watch?v=iOq5kSKqeR4)
- [ ] [Big O Notations (general quick tutorial)](https://www.youtube.com/watch?v=V6mKVRU1evU)
- [ ] [Skiena](https://www.youtube.com/watch?v=z1mkCe3kVUA)
- [ ] [Amortized Analysis](https://www.youtube.com/watch?v=B3SpQZaAZP4&index=10&list=PL1BaGV1cIH4UhkL8a9bJGG356covJ76qN)
- [ ] [Big-O cheat sheet](extras/cheat%20sheets/big-o-cheatsheet.pdf)
- [ ] Problèmes : Contains Duplicate, Valid Anagram, Two Sum, Group Anagrams, Top K Frequent Elements

### Phase 1 — Structures de données (semaines 3-9)

#### Semaine 3 — Tableaux ([Arrays](README.md#arrays)) + Two Pointers
- [ ] Vidéos : [Arrays CS50](https://www.youtube.com/watch?v=tI_tIZFyKBw&t=3009s) · [Arrays (Coursera)](https://www.coursera.org/lecture/data-structures/arrays-OsBSF) · [Dynamic Arrays (Coursera)](https://www.coursera.org/lecture/data-structures/dynamic-arrays-EwbnV)
- [ ] **Implémenter** un tableau dynamique (liste de taille fixe en interne) : `size`, `capacity`, `is_empty`, `at`, `push`, `insert`, `prepend`, `pop`, `delete`, `remove`, `find`, `resize` (×2 quand plein, ÷2 à 1/4)
- [ ] Problèmes : Product of Array Except Self, Valid Sudoku, Encode and Decode Strings, Longest Consecutive Sequence
- [ ] Problèmes Two Pointers : Valid Palindrome, Two Sum II, 3Sum, Container With Most Water, Trapping Rain Water

#### Semaine 4 — Table de hachage ([Hash table](README.md#hash-table)) + Sliding Window
- [ ] Vidéos : [Hashing with Chaining (MIT)](https://www.youtube.com/watch?v=0M_kIqhwbFo&list=PLUl4u3cNGP61Oq3tWYp6V_F-5jb5L2iHb&index=8) · [PyCon 2010: The Mighty Dictionary](https://www.youtube.com/watch?v=C4Kc8xzcA68) · [[Review] Hash tables in 4 minutes](https://youtu.be/knV86FlSXJ8)
- [ ] Optionnel : [Open Addressing (MIT)](https://www.youtube.com/watch?v=rvdJDijO2Ro&index=10&list=PLUl4u3cNGP61Oq3tWYp6V_F-5jb5L2iHb)
- [ ] **Implémenter** une table de hachage à sondage linéaire : `hash(k, m)`, `add`, `exists`, `get`, `remove`
- [ ] Problèmes : Best Time to Buy and Sell Stock, Longest Substring Without Repeating Characters, Longest Repeating Character Replacement, Permutation in String, Minimum Window Substring, Sliding Window Maximum

#### Semaines 5-6 — Listes chaînées ([Linked Lists](README.md#linked-lists))
- [ ] Vidéos : [Linked Lists CS50](https://www.youtube.com/watch?v=2T-A_GFuoTo&t=650s) · [Singly Linked Lists (Coursera)](https://www.coursera.org/lecture/data-structures/singly-linked-lists-kHhgK) · [Why you should avoid linked lists](https://www.youtube.com/watch?v=YQs6IC-vgmo) · [[Review] Linked lists in 4 minutes](https://youtu.be/F8AbOfQwl1c)
- [ ] Vidéo doubly-linked : [Description (Coursera)](https://www.coursera.org/lecture/data-structures/doubly-linked-lists-jpGKD)
- [ ] **Implémenter** (avec pointeur de queue) : `size`, `empty`, `value_at`, `push_front`, `pop_front`, `push_back`, `pop_back`, `front`, `back`, `insert`, `erase`, `value_n_from_end`, `reverse`, `remove_value`
- [ ] Caches ([section du repo](README.md#caches)) : [The Magic of LRU Cache](https://www.youtube.com/watch?v=R5ON3iwx78M) · [Implementing LRU](https://www.youtube.com/watch?v=bq6N7Ym81iI)
- [ ] Problèmes : Reverse Linked List, Merge Two Sorted Lists, Linked List Cycle, Reorder List, Remove Nth Node From End, Copy List With Random Pointer, Add Two Numbers, Find the Duplicate Number, **LRU Cache**

#### Semaine 7 — Pile et file ([Stack](README.md#stack), [Queue](README.md#queue))
- [ ] Vidéos : [Stacks (Coursera)](https://www.coursera.org/lecture/data-structures/stacks-UdKzQ) · [Queue (Coursera)](https://www.coursera.org/lecture/data-structures/queues-EShpq) · [Circular buffer](https://en.wikipedia.org/wiki/Circular_buffer) · [[Review] Stacks](https://youtu.be/KcT3aVgrrpU) · [[Review] Queues](https://youtu.be/D6gu-_tmEpQ)
- [ ] **Implémenter** une file avec ta liste chaînée (`enqueue`, `dequeue`, `empty`) et une file circulaire à tableau fixe (+ `full`)
- [ ] Problèmes : Valid Parentheses, Min Stack, Evaluate Reverse Polish Notation, Generate Parentheses, Daily Temperatures, Car Fleet, Largest Rectangle in Histogram

#### Semaine 8 — Recherche binaire ([Binary search](README.md#binary-search)) + bits en survol ([Bitwise](README.md#bitwise-operations))
- [ ] Vidéos : [Binary Search](https://www.youtube.com/watch?v=D5SrAga1pno) · [[Review] Binary search in 4 minutes](https://youtu.be/fDKIpRe8GW4)
- [ ] Lire le [template de recherche binaire (LeetCode)](https://leetcode.com/discuss/general-discussion/786126/python-powerful-ultimate-binary-search-template-solved-many-problems)
- [ ] **Implémenter** : recherche binaire itérative + récursive
- [ ] Problèmes : Binary Search, Search a 2D Matrix, Koko Eating Bananas, Find Minimum in Rotated Sorted Array, Search in Rotated Sorted Array, Time Based Key-Value Store
- [ ] Bits : [Bits cheat sheet](extras/cheat%20sheets/bits-cheat-sheet.pdf) (puissances de 2 jusqu'à 2^16 et 2^32) · [Bit Manipulation](https://www.youtube.com/watch?v=7jkIUgLC29I) · [Why We Use Two's Complement](https://www.youtube.com/watch?v=lKTsv6iVxV4)
- [ ] Problèmes bits : Single Number, Number of 1 Bits, Counting Bits, Missing Number

#### Semaine 9 — 🟡 Tampon + bilan phase 1
- [ ] Rattraper ce qui est en retard (algo, projet, cyber)
- [ ] Refaire de zéro 8 problèmes tirés au hasard des semaines 2-8 (chronométré, 25 min chacun)
- [ ] 2 problèmes sur papier en parlant à voix haute

### Phase 2 — Arbres, heaps, tris, récursion (semaines 10-17)

#### Semaine 10 — Récursion + arbres ([Recursion](README.md#recursion), [Trees - Intro](README.md#trees---intro))
- [ ] Vidéos récursion : [5 Simple Steps for Solving Any Recursive Problem](https://youtu.be/ngCos392W4w) · [Stanford Lecture 8](https://www.youtube.com/watch?v=gl3emqCuueQ&list=PLFE6E58F856038C69&index=8)
- [ ] Vidéos arbres : [Intro to Trees (Coursera)](https://www.coursera.org/lecture/data-structures/trees-95qda) · [Tree Traversal (Coursera)](https://www.coursera.org/lecture/data-structures/tree-traversal-fr51b) · [BFS and DFS](https://www.youtube.com/watch?v=uWL6FJhq5fM) · [[Review] Tree Traversal](https://www.youtube.com/playlist?list=PL9xmBV_5YoZO1JC2RgEi04nLy6D-rKk6b)
- [ ] Problèmes : Invert Binary Tree, Maximum Depth of Binary Tree, Same Tree, Subtree of Another Tree, Diameter of Binary Tree, Balanced Binary Tree

#### Semaines 11-12 — Arbres binaires de recherche ([BSTs](README.md#binary-search-trees-bsts))
- [ ] Vidéos : [Binary Search Tree Review](https://www.youtube.com/watch?v=x6At0nzX92o&index=1&list=PLA5Lqm4uh9Bbq-E0ZnqTIa8LRaL77ica6) + la série mycodeschool de la section (C/C++, mais les concepts s'appliquent) : implémentation, min/max, hauteur, parcours, is BST, suppression, successeur
- [ ] **Implémenter** un BST : `insert`, `get_node_count`, `print_values`, `delete_tree`, `is_in_tree`, `get_height`, `get_min`, `get_max`, `is_binary_search_tree`, `delete_value`, `get_successor`
- [ ] Problèmes : Lowest Common Ancestor of a BST, Binary Tree Level Order Traversal, Binary Tree Right Side View, Count Good Nodes, Validate BST, Kth Smallest Element in a BST, Construct Binary Tree from Preorder and Inorder
- [ ] Bonus (difficiles) : Binary Tree Maximum Path Sum, Serialize and Deserialize Binary Tree

#### Semaine 13 — Heap / file de priorité ([Heap](README.md#heap--priority-queue--binary-heap))
- [ ] Vidéos : [Introduction (Coursera)](https://www.coursera.org/lecture/data-structures/introduction-2OpTs) · [MIT 6.006 Binary Heaps](https://www.youtube.com/watch?v=Xnpo1atN-Iw&list=PLUl4u3cNGP63EdVPNLG3ToM6LaEUuStEY&index=12) · [Linear Time BuildHeap](https://www.youtube.com/watch?v=MiyLo8adrWw) · [[Review] Heap](https://www.youtube.com/playlist?list=PL9xmBV_5YoZNsyqgPW-DNwUeT8F8uhWc6)
- [ ] **Implémenter** un max-heap : `insert`, `sift_up`, `get_max`, `get_size`, `is_empty`, `extract_max`, `sift_down`, `remove`, `heapify`, `heap_sort`
- [ ] Problèmes : Kth Largest Element in a Stream, Last Stone Weight, K Closest Points to Origin, Kth Largest Element in an Array, Task Scheduler, Merge K Sorted Lists, Find Median from Data Stream

#### Semaine 14 — Tris ([Sorting](README.md#sorting)) + Intervals
- [ ] Vidéos : [Insertion Sort, Merge Sort (MIT)](https://www.youtube.com/watch?v=Kg4bqzAqRBM&index=3&list=PLUl4u3cNGP61Oq3tWYp6V_F-5jb5L2iHb) · [Quicksort](https://www.youtube.com/watch?v=y_G9BkAm6B8&index=4&list=PL89B61F78B552C1AB) · [[Review] Sorting in 18 minutes](https://www.youtube.com/playlist?list=PL9xmBV_5YoZOZSbGAXAPIq1BeUf4j20pl)
- [ ] Stabilité : [Sorting Algorithm Stability](https://en.wikipedia.org/wiki/Sorting_algorithm#Stability) — savoir répondre à « Quicksort est-il stable ? »
- [ ] **Implémenter** : mergesort, quicksort (+ insertion et selection en 15 min chacun)
- [ ] Problèmes : Insert Interval, Merge Intervals, Non-overlapping Intervals, Meeting Rooms, Meeting Rooms II, Sort Colors

#### Semaine 15 — Tries ([Tries](README.md#tries)) + début backtracking
- [ ] Vidéos : [Introduction To Tries](https://www.coursera.org/learn/data-structures-optimizing-performance/lecture/08Xyf/core-introduction-to-tries) · [Implementing A Trie](https://www.coursera.org/learn/data-structures-optimizing-performance/lecture/DFvd3/core-implementing-a-trie) · [TopCoder - Using Tries](https://www.topcoder.com/thrive/articles/Using%20Tries)
- [ ] Problèmes : Implement Trie, Design Add and Search Words, Word Search II
- [ ] Vidéos backtracking : [Stanford Lecture 9](https://www.youtube.com/watch?v=uFJhEPrbycQ&list=PLFE6E58F856038C69&index=9) · [Lecture 10](https://www.youtube.com/watch?v=NdF1QDTRkck&index=10&list=PLFE6E58F856038C69)
- [ ] Lire le [Backtracking Blueprint (Python)](https://leetcode.com/problems/combination-sum/discuss/429538/General-Backtracking-questions-solutions-in-Python-for-reference-%3A)

#### Semaine 16 — Backtracking
- [ ] Vidéo : [Stanford Lecture 11](https://www.youtube.com/watch?v=p-gpaIGRCQI&list=PLFE6E58F856038C69&index=11)
- [ ] Problèmes : Subsets, Combination Sum, Permutations, Subsets II, Combination Sum II, Word Search, Palindrome Partitioning, Letter Combinations of a Phone Number, N-Queens

#### Semaine 17 — 🟡 Tampon + bilan phase 2
- [ ] Rattraper ce qui est en retard (algo, projet, cyber, frontend)
- [ ] Refaire de zéro 8 problèmes des phases 1-2
- [ ] **Premier mock** : 45 min chronométré, énoncé inconnu, en parlant à voix haute (seul ou avec un ami)

### Phase 3 — Graphes, programmation dynamique, greedy (semaines 18-30)

#### Semaines 18-20 — Graphes ([Graphs](README.md#graphs))
- [ ] Vidéos : [MIT BFS](https://www.youtube.com/watch?v=oFVYVzlvk9c&t=14s&ab_channel=MITOpenCourseWare) · [MIT DFS](https://www.youtube.com/watch?v=IBfWDYSffUU&t=32s&ab_channel=MITOpenCourseWare) · [Skiena L10 - Graph Data Structures](https://www.youtube.com/watch?v=Sjk0xqWWPCc&list=PLOtl7M3yp-DX6ic0HGT0PUX_wiNmkWkXx&index=10) · [Skiena L11 - Graph Traversal](https://www.youtube.com/watch?v=ZTwjXj81NVY&list=PLOtl7M3yp-DX6ic0HGT0PUX_wiNmkWkXx&index=11) · [Skiena L12 - DFS](https://www.youtube.com/watch?v=KyordYB3BOs&list=PLOtl7M3yp-DX6ic0HGT0PUX_wiNmkWkXx&index=12)
- [ ] Vidéos : [Aduni L6 - Topological Sorting](https://www.youtube.com/watch?v=i_AQT_XfvD8&index=6&list=PLFDnELG9dpVxQCxuD-9BSy2E7BWY3t5Sm) · [Aduni L7 - DFS, BFS, Union Find](https://www.youtube.com/watch?v=ufj5_bppBsA&list=PLFDnELG9dpVxQCxuD-9BSy2E7BWY3t5Sm&index=7)
- [ ] **Implémenter** (liste d'adjacence) : DFS récursif, DFS itératif, BFS, détection de cycle, tri topologique, composantes connexes, graphe biparti, union-find
- [ ] Problèmes : Number of Islands, Max Area of Island, Clone Graph, Rotting Oranges, Pacific Atlantic Water Flow, Surrounded Regions, Course Schedule, Course Schedule II, Graph Valid Tree, Number of Connected Components, Redundant Connection, Word Ladder

#### Semaine 21 — Graphes avancés
- [ ] Vidéos : [6.006 Dijkstra](https://www.youtube.com/watch?v=NSHizBK9JD8&t=1731s&ab_channel=MITOpenCourseWare) · [Skiena L13 - Minimum Spanning Trees](https://www.youtube.com/watch?v=oolm2VnJUKw&list=PLOtl7M3yp-DX6ic0HGT0PUX_wiNmkWkXx&index=13) · [[Review] Shortest Path](https://www.youtube.com/playlist?list=PL9xmBV_5YoZO-Y-H3xIC9DGSfVYJng9Yw) · [[Review] MST](https://www.youtube.com/playlist?list=PL9xmBV_5YoZObEi3Hf6lmyW-CBfs7nkOV)
- [ ] **Implémenter** : Dijkstra (avec `heapq`), Prim
- [ ] Problèmes : Network Delay Time, Min Cost to Connect All Points, Cheapest Flights Within K Stops, Swim in Rising Water

#### Semaine 22 — 🟡 Tampon + 🎯 premières candidatures
- [ ] Refaire de zéro 8 problèmes (dont 3 de graphes)
- [ ] Mettre à jour le CV ([Update Your Resume](README.md#update-your-resume), [guide Tech Interview Handbook](https://www.techinterviewhandbook.org/resume/guide)) à partir du [journal d'impact](#journal-dimpact) :
    - réalisations chiffrées plutôt que tâches
    - le **backend du poste actuel** mis en avant (API, base de données, CI)
    - l'**accessibilité** (RGAA) mise en avant : compétence rare et recherchée
    - le projet perso (lien vers la démo et le repo)
- [ ] 🎯 **Candidater dans 2-3 scale-ups pour s'entraîner** (entretiens plus pratiques, TS/React valorisés)

#### Semaines 23-25 — Programmation dynamique 1D ([Dynamic Programming](README.md#dynamic-programming))
- [ ] Vidéos : [Skiena L19 - Introduction to DP](https://www.youtube.com/watch?v=wAA0AMfcJHQ&list=PLOtl7M3yp-DX6ic0HGT0PUX_wiNmkWkXx&index=18) · [Skiena L21 - DP](https://www.youtube.com/watch?v=2xPE4Wq8coQ&list=PLOtl7M3yp-DX6ic0HGT0PUX_wiNmkWkXx&index=21) · [Skiena L22 - DP and Review](https://www.youtube.com/watch?v=Yh3RzqQGsyI&list=PLOtl7M3yp-DX6ic0HGT0PUX_wiNmkWkXx&index=22)
- [ ] Piocher dans la [playlist de problèmes DP courts](https://www.youtube.com/playlist?list=PLrmLmBdmIlpsHaNTPP_jHHDx_os9ItYXr)
- [ ] Méthode : récursion → mémoïsation (`@cache`) → tableau bottom-up
- [ ] Problèmes : Climbing Stairs, Min Cost Climbing Stairs, House Robber, House Robber II, Longest Palindromic Substring, Palindromic Substrings, Decode Ways, Coin Change, Maximum Product Subarray, Word Break, Longest Increasing Subsequence, Partition Equal Subset Sum

#### Semaine 26 — 🟡 Tampon DP
La DP est le sujet le plus dur du plan : cette semaine sert à consolider avant la 2D.
- [ ] Rattraper les problèmes DP 1D en retard
- [ ] Refaire de zéro 5 problèmes DP 1D ratés, en écrivant d'abord la relation de récurrence sur papier
- [ ] Refaire 3 problèmes anciens (arbres, graphes)

#### Semaines 27-28 — Programmation dynamique 2D
- [ ] Vidéos : [Skiena L20 - Edit Distance](https://www.youtube.com/watch?v=T3A4jlHlhtA&list=PLOtl7M3yp-DX6ic0HGT0PUX_wiNmkWkXx&index=19) · [Edit Distance (continued)](https://www.youtube.com/watch?v=iPnPVcZmRbE&list=PLOtl7M3yp-DX6ic0HGT0PUX_wiNmkWkXx&index=20)
- [ ] Problèmes : Unique Paths, Longest Common Subsequence, Best Time to Buy and Sell Stock with Cooldown, Coin Change II, Target Sum, Interleaving String, Longest Increasing Path in a Matrix, Edit Distance

#### Semaine 29 — Greedy, maths et survols
- [ ] Problèmes greedy : Maximum Subarray, Jump Game, Jump Game II, Gas Station, Hand of Straights, Partition Labels, Valid Parenthesis String
- [ ] Problèmes maths : Rotate Image, Spiral Matrix, Set Matrix Zeroes, Pow(x, n)
- [ ] Survol NP-complet ([section](README.md#np-np-complete-and-approximation-algorithms)) : [Skiena L23 - NP-Completeness](https://www.youtube.com/watch?v=ItHp5laE1VE&list=PLOtl7M3yp-DX6ic0HGT0PUX_wiNmkWkXx&index=23) — savoir reconnaître le voyageur de commerce et le sac à dos déguisés
- [ ] Survol processus / threads ([section](README.md#processes-and-threads)) : différence processus/thread, mutex, deadlock + [Understanding the Python GIL](https://www.youtube.com/watch?v=Obt-vMVdM8s)

#### Semaine 30 — 🟡 Tampon + grande révision ([Final Review](README.md#final-review))
- [ ] Vidéos [Michael Sambol](https://www.youtube.com/@MichaelSambol) sur tous les sujets faibles
- [ ] Refaire de zéro 10 problèmes, 1 par pattern
- [ ] ✅ Objectif : ~150 problèmes faits, au moins 70 % réussis seul à la 2e tentative

### Phase 4 — Préparation aux entretiens (semaines 31-44)

Voir la [semaine type de la phase 4](#semaine-type-phase-4-semaines-31-44) : l'algo passe en entretien du niveau (problèmes « à refaire » + problèmes tagués par entreprise). Le **thème de la semaine** a ~4h30 (2h30 le jour long 1 + 2 h le jour long 2).

À ~5 ans d'expérience, **le system design décide souvent du niveau** (intermédiaire ou senior) : c'est le thème le plus gros de la phase.

#### Semaines 31-33 — System design ([System Design](README.md#system-design-scalability-data-handling)) — ~14 h
- [ ] **START HERE** du repo : [The System Design Primer](https://github.com/donnemartin/system-design-primer)
- [ ] Scalability for dummies : [Clones](http://www.lecloud.net/post/7295452622/scalability-for-dummies-part-1-clones) · [Database](http://www.lecloud.net/post/7994751381/scalability-for-dummies-part-2-database) · [Cache](http://www.lecloud.net/post/9246290032/scalability-for-dummies-part-3-cache) · [Asynchronism](http://www.lecloud.net/post/9699762917/scalability-for-dummies-part-4-asynchronism)
- [ ] [Numbers Everyone Should Know](http://everythingisdata.wordpress.com/2009/10/17/numbers-everyone-should-know/) · [CAP Theorem](http://ksat.me/a-plain-english-introduction-to-cap-theorem) · [Consistent Hashing](http://www.tom-e-white.com/2007/11/consistent-hashing.html) · [cheat sheet](extras/cheat%20sheets/system-design.pdf)
- [ ] Complément moderne : livre *System Design Interview* (Alex Xu, vol. 1) ou [Hello Interview](https://www.hellointerview.com/)
- [ ] Appliquer le **flow du repo** (scope → contraintes et estimations → design abstrait → goulots) aux exercices : URL shortener, générateur d'ID unique, cache, key-value store, partage de photos
- [ ] Refaire l'exercice sur **ton propre projet** : comment il tiendrait 1 M d'utilisateurs ?

#### Semaine 34 — Réseau + design OO (survol) — ~5 h
- [ ] Réseau ([Networking](README.md#networking)) : [UDP and TCP](https://www.youtube.com/watch?v=Vdc8TCESIg8) · [HTTP](https://www.youtube.com/watch?v=WGJrLqtX7As) · [HTTP 2.0](https://www.youtube.com/watch?v=E9FxNzv1Tr8)
- [ ] Design patterns ([section](README.md#design-patterns)), les plus utiles en entretien : strategy, observer, factory, singleton, decorator, adapter (référence : [sourcemaking](https://sourcemaking.com/design-patterns-and-tips))
- [ ] Testing ([section](README.md#testing)) : mocks, tests d'intégration, injection de dépendances — à relier à ton projet

#### Semaine 35 — Observabilité — ~6 h
Un atout pour Datadog, et utile en system design pour toutes les entreprises (la question « comment tu le surveilles ? » revient souvent).
- [ ] Les 3 piliers : logs structurés, métriques, traces distribuées · SLI / SLO / alerting
- [ ] Instrumenter le projet avec **OpenTelemetry** (traces de l'API, métriques, logs corrélés) et les afficher dans un outil (Grafana, ou l'essai gratuit de Datadog)
- [ ] Côté front : Web Vitals et erreurs remontés depuis le navigateur (RUM)
- [ ] Reprendre 2 exercices de system design et y ajouter une section monitoring

#### Semaine 36 — Behavioral ([Be thinking of…](README.md#be-thinking-of-for-when-the-interview-comes)) — ~5 h + jours courts
La matière vient de ton poste actuel et du [journal d'impact](#journal-dimpact) : il s'agit surtout de la mettre en forme.
- [ ] Vidéos : [How to Get a Job at the Big 4](https://www.youtube.com/watch?v=YJZCUhxNCv8) · [Cracking the Facebook Coding Interview - The Approach](https://www.youtube.com/watch?v=wCl9kvQGHPI)
- [ ] Écrire 6-8 histoires **STAR** à partir du journal d'impact, qui répondent aux ~20 questions de la section. Au moins 3 où tu **mènes** : décision technique, feature de bout en bout, mentorat
- [ ] Leadership Principles d'Amazon : relier chaque histoire à 1-2 principes
- [ ] Préparer tes [questions pour l'intervieweur](README.md#have-questions-for-the-interviewer)
- [ ] Jours courts des semaines 37-44 : répéter une histoire à voix haute (en anglais)

#### Semaines 37-38 — System design approfondi (niveau senior) — ~9 h
- [ ] Exercices plus ouverts : rate limiter, système de notifications, fil d'actualité, chat en temps réel, stockage de fichiers, moteur de recherche avec autocomplete
- [ ] Pour chacun : estimations chiffrées, **au moins 2 options comparées** avec leurs compromis, points de défaillance, monitoring
- [ ] S'entraîner à mener la discussion (poser les questions, cadrer, gérer le temps) plutôt que d'attendre les questions
- [ ] 1 mock system design chronométré (45 min) par semaine, enregistré puis réécouté

#### Semaines 39-44 — Mocks et candidatures big tech — ~27 h + algo
- [ ] 1 mock par semaine ([Mock Interviews](README.md#interview-process--general-interview-prep)) : [Pramp](https://www.pramp.com/) (gratuit, entre pairs), [interviewing.io](https://interviewing.io), [Hello Interview](https://www.hellointerview.com/)
- [ ] Au moins 3 mocks system design (dont 1 frontend), 2 mocks machine coding frontend et 1 mock behavioral
- [ ] Thème de la semaine : alterner system design générique et [frontend system design](#piste-rounds-frontend)
- [ ] Problèmes tagués par entreprise cible (Google, Datadog, Amazon…)
- [ ] 🎯 **Candidatures** sur des postes **Frontend / Fullstack SWE**, par cooptation si possible (LinkedIn, anciens collègues). Viser large : 2-3 big tech (Datadog, Google, Amazon…) + 5-6 scale-ups solides. Si mobilité possible : Londres ou remote européen (beaucoup plus de postes)
- [ ] Un refus est normal au premier essai : noter les retours, délai de 6-12 mois avant de recandidater dans la même entreprise

---

## Piste projet

**Jour long 2, ~2h30 / semaine puis 1h30 en phase 4 (~95 h au total).** Un seul projet qui prouve ce que le plan d'algo ne montre pas : fullstack, backend Python, LLM, Docker, CI/CD, déploiement, sécurité.

**Idée proposée** — un *assistant de révision* : tu y déposes tes notes et ton journal de problèmes, tu lui poses des questions (RAG) et il génère des quiz et des cartes à partir de tes points faibles. Tu t'en sers pendant le plan, donc tu trouveras toi-même ce qui manque. N'importe quelle autre idée convient si elle coche les mêmes cases.

| Semaines | Jalon | Ce que ça entraîne |
|---|---|---|
| 1-4 | Cadrage + API **FastAPI** + **PostgreSQL** (schéma, migrations, jointures, index, transactions) + authentification | Révision backend et SQL |
| 5-9 | Front **React/TS** branché sur l'API · tests (pytest + Vitest) · **Docker Compose** (API, base, front) | Fullstack, tests, Docker |
| 10-14 | **CI/CD** (GitHub Actions : lint, tests, build d'image) · **déploiement** sur un cloud (AWS ou GCP) · variables d'env et secrets | Révision CI/CD, cloud |
| 15-21 | **LLM** : appels d'API, réponses en streaming dans l'UI, **RAG** (embeddings + pgvector), gestion des erreurs et des coûts | Compétence la plus demandée du marché |
| 22-28 | **Évaluation** simple des réponses LLM · **audit de sécurité** avec la piste cyber (OWASP, prompt injection) · corrections | Lien direct avec la cyber |
| 29-34 | Corrections de l'audit, **sécurité de la chaîne** (secrets, dépendances, en-têtes) avec la piste cyber | Lien direct avec la cyber |
| 35 | **Observabilité** : OpenTelemetry, traces, métriques, RUM côté front | Atout Datadog, argument en system design |
| 36-44 | Finitions, README soigné, schéma d'architecture, démo en ligne · sert de support en system design et en behavioral | Vitrine pour le CV et les entretiens |

- [ ] Jalon 1 — API + base + auth
- [ ] Jalon 2 — Front + tests + Docker Compose
- [ ] Jalon 3 — CI/CD + déploiement
- [ ] Jalon 4 — Fonctionnalités LLM + RAG
- [ ] Jalon 5 — Évaluation + audit sécurité + corrections
- [ ] Jalon 6 — Observabilité
- [ ] Jalon 7 — Vitrine (README, démo, architecture)

---

## Piste rounds frontend

**Jour long 2, 1h30 / semaine, semaines 3-22 (~30 h).** Les postes frontend/fullstack en big tech ont des rounds spécifiques en plus de l'algo. Ressources : [javascript.info](https://javascript.info/), [GreatFrontEnd](https://www.greatfrontend.com/), [BFE.dev](https://bigfrontend.dev/).

| Semaines | Sujet | Exercices |
|---|---|---|
| 3-6 | Fondamentaux JS | Event loop, closures, `this`, prototypes, promesses et `async`/`await` : savoir les expliquer et prédire la sortie d'un code |
| 7-11 | Utilitaires à coder en temps limité | `debounce`, `throttle`, `Promise.all`, `deepClone`, `EventEmitter`, `curry`, `flatten`, `memoize` |
| 12-18 | *Machine coding* (composant UI en 45-60 min) | Autocomplete, modal, onglets, accordéon, scroll infini, todo list, carrousel — en React **et** en JS natif pour 2-3 d'entre eux |
| 19-22 | Performance | Mémoïsation React, re-renders, virtualisation de listes, Web Vitals, profiling. L'accessibilité est déjà un point fort : juste préparer 2-3 exemples concrets à citer en entretien |

### Frontend system design (semaines 23-30, même créneau, ~12 h, + phase 4)

C'est ce qui distingue un profil front intermédiaire d'un profil senior. Ressource : [GreatFrontEnd — Front End System Design](https://www.greatfrontend.com/front-end-system-design-playbook).

| Semaines | Sujet |
|---|---|
| 23-24 | Méthode (cadrage, architecture, modèle de données, API client/serveur, optimisations) · stratégies de rendu : CSR, SSR, SSG, streaming |
| 25-26 | Gestion d'état à grande échelle, cache côté client, temps réel (WebSocket, SSE), pagination |
| 27-28 | Design system, architecture d'une grosse SPA (modules, micro-frontends : quand oui, quand non), stratégie de tests, i18n, **accessibilité à l'échelle** (ton point fort à mettre en avant) |
| 29-30 | Exercices complets : fil d'actualité, autocomplete, éditeur collaboratif, tableau de bord de monitoring (clin d'œil Datadog) |

---

## Piste cyber

**Jour court C (1 h, un lab) + fin du jour long 1 (1 h, théorie) jusqu'à S30, puis jour court C seul jusqu'à S35 (~62 h).**
**Objectif** : cybersécurité orientée dev (AppSec) — coder de façon sécurisée, savoir l'expliquer en entretien et en system design.
**Ressource principale** : [PortSwigger Web Security Academy](https://portswigger.net/web-security) (gratuit, avec labs pratiques).

| Semaines | Sujet | Ressources |
|---|---|---|
| 3-4 | Modèle de menace, vue d'ensemble | [OWASP Top 10](https://owasp.org/www-project-top-ten/) · [MIT - Introduction, Threat Models](https://www.youtube.com/watch?v=GqmQg-cszw4&index=1&list=PLUl4u3cNGP62K2DjQLRxDNRi0z2IRWnNh) (repo, [Computer Security](README.md#computer-security)) |
| 5-6 | Bases réseau | Repo [Networking](README.md#networking) : [TCP/IP and the OSI Model](https://www.youtube.com/watch?v=e5DEVa9eSN0) · [SSL and HTTPS](https://www.youtube.com/watch?v=S2iBR2ZlZf0) · [SSL/TLS](https://www.youtube.com/watch?v=Rp3iZUvXWlM) |
| 7-8 | Cryptographie appliquée | Repo [Cryptography](README.md#cryptography) : [Khan Academy](https://www.khanacademy.org/computing/computer-science/cryptography) · [Hash Functions (MIT)](https://www.youtube.com/watch?v=KqqOXndnvic&list=PLUl4u3cNGP6317WaSNfmCvGym2ucw3oGp&index=30) · en pratique : hash de mots de passe (bcrypt/argon2), signatures, JWT |
| 9-11 | Injections SQL, authentification | PortSwigger : *SQL injection*, *Authentication* — à appliquer à l'auth du projet |
| 12-15 | XSS, CSRF, CORS, clickjacking (ton terrain en frontend) | PortSwigger : *Cross-site scripting*, *CSRF*, *CORS*, *Clickjacking* · [MIT - Web Security Model](https://www.youtube.com/watch?v=chkFBigodIw&index=7&list=PLUl4u3cNGP62K2DjQLRxDNRi0z2IRWnNh) |
| 16-19 | Contrôle d'accès, IDOR, SSRF, path traversal | PortSwigger : *Access control*, *SSRF*, *Path traversal* · [MIT - Securing Web Applications](https://www.youtube.com/watch?v=EBQIGy1ROLY&index=8&list=PLUl4u3cNGP62K2DjQLRxDNRi0z2IRWnNh) |
| 20-22 | OAuth 2.0 / OIDC, attaques JWT | PortSwigger : *OAuth authentication*, *JWT attacks* |
| 23-25 | Logique métier, upload de fichiers, API | PortSwigger : *Business logic vulnerabilities*, *File upload*, *API testing* |
| 26-28 | Sécurité des applis LLM | [OWASP Top 10 for LLM Applications](https://genai.owasp.org/) · PortSwigger : *Web LLM attacks* (prompt injection) — en parallèle du jalon 5 du projet |
| 29-30 | Chaîne d'approvisionnement et configuration | Gestion des secrets, dépendances (`npm audit`, `pip-audit`, Dependabot), en-têtes de sécurité (CSP, HSTS), gestion des tokens côté front |
| 31-35 | Audit du projet + consolidation | Appliquer tout le parcours au projet · refaire les labs ratés |

Optionnel après le plan : certification PortSwigger **BSCP**.

---

## Journal d'impact

**10 min / semaine, dès la semaine 1.** C'est la matière première du CV (S22) et des histoires STAR (S36).

**Au travail, pendant ces 10 mois** (le plus gros levier, hors programme) :
- [ ] Prendre des tâches backend : API, base de données, CI/CD — et le noter ici
- [ ] Mener au moins une feature de bout en bout (du cadrage à la mise en prod)
- [ ] Porter au moins une décision technique (proposition, comparaison d'options, adoption)
- [ ] Accompagner un collègue (onboarding, revue de code, mentorat)
- [ ] Chiffrer ce qui peut l'être : performance, score d'accessibilité, bugs évités, temps gagné

| Date | Ce que j'ai fait | Mon rôle | Impact (chiffré si possible) | Front / back / a11y / lead |
|---|---|---|---|---|
| | | | | |

---

## Journal des problèmes

| Date | Problème | Pattern | Seul ? | Temps | À refaire le |
|---|---|---|---|---|---|
| | | | | | |

## Points d'étape

- [ ] **Semaine 9** : je résous seul la plupart des problèmes *easy* en moins de 20 min · projet : API + base en place
- [ ] **Semaine 17** : je reconnais le pattern d'un problème *medium* d'arbre ou de pile en moins de 5 min · projet déployé avec CI/CD
- [ ] **Semaine 22** : premières candidatures scale-ups envoyées · fonctionnalités LLM en cours
- [ ] **Semaine 30** : ~150 problèmes faits, 70 % réussis seul à la 2e tentative · projet audité · 4 exercices de frontend system design faits
- [ ] **Semaine 38** : 10+ exercices de system design faits · projet instrumenté (observabilité) · 6-8 histoires STAR prêtes
- [ ] **Semaine 44** : 6+ mocks faits (dont 3 system design), candidatures envoyées · journal d'impact avec au moins 3 éléments backend et 1 feature menée de bout en bout
