// Apa itu 8 puzzle? 8 puzzle adalah permainan sliding
// puzzle ciptaan Sam Loyd yang terdiri dari sebuah bingkai
// yang berisi kotak-kotak angka dalam keadaan teracak
// dimana sebuah kotak hilang. Karena permainan ini
// bernama 8 puzzle, maka ukuran bingkai adalah tiga kali
// tiga. Tujuan dari puzzle adalah dengan memakai gerakan
// geser yang menggunakan spasi kosong untuk mencapai
// goal state yang diinginkan.

// EightPuzzleSearch: sebuah class yang digunakan untuk mencari
// solusi dari permainan teka-teki delapan angka (Eight Puzzle).
// Algoritma pencarian yang umum digunakan di sini adalah algoritma
// pencarian berbasis graf, seperti Breadth-First Search (BFS) atau A* Search.
//  class EightPuzzleSearch mungkin memiliki metode-metode seperti:
// __init__(self, initial_state): Constructor untuk menginisialisasi objek pencarian dengan keadaan awal (initial state) dari teka-teki delapan angka.
// bfs(self): Metode yang menggunakan algoritma Breadth-First Search untuk mencari solusi.
// a_star(self): Metode yang menggunakan algoritma A* Search untuk mencari solusi dengan mempertimbangkan biaya langkah dan heuristik.

// EightPuzzleSpace: class yang mendefinisikan ruang pencarian untuk teka-teki delapan angka.
// Class ini mungkin berisi informasi tentang aturan permainan,
// langkah-langkah yang mungkin diambil dari suatu keadaan,
// serta fungsi heuristik yang membantu algoritma pencarian dalam menilai kualitas suatu keadaan.
// Contoh metode dalam EightPuzzleSpace:
// get_possible_moves(state): Metode yang mengembalikan langkah-langkah yang mungkin dilakukan dari suatu keadaan.
// is_goal_state(state): Metode yang memeriksa apakah suatu keadaan adalah keadaan tujuan (goal state).
// calculate_heuristic(state): Metode yang menghitung nilai heuristik dari suatu keadaan untuk membimbing algoritma pencarian (digunakan dalam algoritma A*).

// Node: struktur data yang merepresentasikan simpul dalam graf pencarian.
// Setiap simpul mungkin memiliki informasi seperti keadaan (state),
// langkah yang mengarah ke simpul tersebut, biaya langkah, dan nilai heuristik (jika digunakan).
// Nodes digunakan oleh algoritma pencarian untuk membangun jalur solusi dari simpul awal ke simpul tujuan.
// Contoh atribut dalam Node:
// state: Keadaan yang direpresentasikan oleh simpul.
// parent: Simpul induk yang mengarah ke simpul saat ini (simpul yang menghasilkan keadaan ini).
// action: Langkah yang diambil dari simpul induk untuk mencapai simpul saat ini.
// path_cost: Biaya total untuk mencapai simpul saat ini dari simpul awal.
// heuristic_value: Nilai heuristik (jika digunakan) dari simpul, membantu algoritma pencarian dalam memilih simpul selanjutnya.
