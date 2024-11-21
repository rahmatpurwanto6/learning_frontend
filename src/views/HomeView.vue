<template>
  <html>
    <head>
      <title>Learning Management System</title>
      <link
        rel="stylesheet"
        href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.13.0/css/all.min.css"
        integrity="sha512-L7MWcK7FNPcwNqnLdZq86lTHYLdQqZaz5YcAgE+5cnGmlw8JT03QB2+oxL100UeB6RlzZLUxCGSS4/++mNZdxw=="
        crossorigin="anonymous"
        referrerpolicy="no-referrer"
      />

      <link
        href="https://fonts.googleapis.com/css2?family=Roboto:wght@400;500;700&amp;display=swap"
        rel="stylesheet"
      />
    </head>
    <body>
      <div class="container">
        <div class="sidebar">
          <h2>adhivasindo</h2>
          <ul>
            <li>
              <a href="#">
                <i class="fas fa-tachometer-alt"> </i>
                Dashboard
              </a>
            </li>
            <li>
              <a href="#">
                <i class="fas fa-book"> </i>
                Modul
              </a>
            </li>
            <li>
              <a href="#">
                <i class="fas fa-user"> </i>
                Peserta
              </a>
            </li>
            <li>
              <a href="#">
                <i class="fas fa-comments"> </i>
                Group Chat
              </a>
            </li>
            <li>
              <a href="#">
                <i class="fas fa-chalkboard-teacher"> </i>
                Pemateri
              </a>
            </li>
          </ul>
          <div class="profile">
            <ul>
              <li>
                <a href="#">
                  <i class="fas fa-cog"> </i>
                  Settings
                </a>
              </li>
              <li>
                <a href="#">
                  <i class="fas fa-calendar-alt"> </i>
                  Kalender
                </a>
              </li>
              <li>
                <a href="#" class="logout">
                  <i class="fas fa-sign-out-alt"> </i>
                  Log Out
                </a>
              </li>
            </ul>
          </div>
        </div>
        <div class="main-content">
          <div class="header">
            <h1>LEARNING MANAGEMENT SYSTEM</h1>
            <div class="search-bar">
              <input placeholder="Search..." type="text" />
              <i class="fas fa-search"> </i>
            </div>
          </div>
          <div class="banner">
            <div>
              <h2>Pemrograman Frontend Modern dengan React dan Angular</h2>
              <p>
                Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nullam
                scelerisque leo et libero fermentum, vitae commodo velit
                vehicula.
              </p>
              <div class="info">
                <span>
                  <i class="fas fa-user"> </i>
                  Pemateri By Josep
                </span>
                <span>
                  <i class="fas fa-calendar-alt"> </i>
                  14-06-2025
                </span>
              </div>
            </div>
            <button>MULAI LEARNING</button>
          </div>
          <div class="modules">
            <div class="module">
              <img
                alt="Image of a computer screen displaying code"
                height="200"
                src="https://storage.googleapis.com/a1aa/image/9ZXUf4ySNOyoVKOiDMjh1uvf66He9IN91w2WWVorgFDrUOmnA.jpg"
                width="300"
              />
              <h3>PEMROGRAMAN</h3>
              <p>Materi Kompetensi</p>
              <p>Pemrograman Frontend Modern</p>
              <p>Pemrograman Backend untuk Industri</p>
              <p>Pengembangan API Berstandar Industri</p>
              <p>
                Menerapkan Clean Code dan Design Pattern dalam Pengembangan
                Software
              </p>
            </div>
            <div class="module">
              <img
                alt="Image of a creative marketing concept"
                height="200"
                src="https://storage.googleapis.com/a1aa/image/2os8qhDL09JFCFflEuQu6s2UlyeBd6DXKdvjpr4bDidXKHzTA.jpg"
                width="300"
              />
              <h3>CREATIVE MARKETING</h3>
              <p>Materi Kompetensi</p>
              <p>Strategi Pemasaran Digital</p>
              <p>Mengoptimalkan SEO dan SEM</p>
              <p>Menggunakan Content Marketing</p>
              <p>Menerapkan User-Generated Content</p>
            </div>
            <div class="module">
              <img
                alt="Image of a management concept"
                height="200"
                src="https://storage.googleapis.com/a1aa/image/efw91c9NI6h3ep8le7wtdDGYCzUquHdhnNePbNLwmSTmS5YeE.jpg"
                width="300"
              />
              <h3>MANAGEMENT SDM</h3>
              <p>Materi Kompetensi</p>
              <p>Manajemen Sumber Daya Manusia</p>
              <p>Pengembangan Karyawan</p>
              <p>Manajemen Kinerja</p>
              <p>Menerapkan Sistem Reward dan Punishment</p>
            </div>
          </div>
          <div class="scores">
            <h3>NILAI PESERTA</h3>
            <table>
              <tr>
                <th>Rank</th>
                <th>Name</th>
                <th>Class</th>
                <th>Modul</th>
                <th>Point</th>
              </tr>
              <tr>
                <td>1</td>
                <td>Parjo Faiza</td>
                <td>L1</td>
                <td>PEMROGRAMAN</td>
                <td>
                  <a href="#"> 1,234 Point </a>
                </td>
              </tr>
              <tr>
                <td>2</td>
                <td>Juliana</td>
                <td>L1</td>
                <td>CREATIVE MARKETING</td>
                <td>
                  <a href="#"> 1,200 Point </a>
                </td>
              </tr>
              <tr>
                <td>3</td>
                <td>Ahmad</td>
                <td>L1</td>
                <td>MANAGEMENT SDM</td>
                <td>
                  <a href="#"> 1,150 Point </a>
                </td>
              </tr>
            </table>
          </div>
        </div>
        <div class="right-sidebar">
          <div class="welcome">
            <img
              alt="Profile picture of Juliana"
              height="80"
              src="https://storage.googleapis.com/a1aa/image/mesRPRyKJExMSaPI631Hd5aa4pNgif56dA4uixYTWGpYKHzTA.jpg"
              width="80"
            />
            <h3>SELAMAT DATANG, JULIANA</h3>
            <p>Di LMS by Adhivasindo</p>
          </div>
          <div class="calendar">
            <h3>April 2025</h3>
            <div class="days">
              <div>1</div>
              <div>2</div>
              <div>3</div>
              <div>4</div>
              <div>5</div>
              <div>6</div>
              <div>7</div>
              <div>8</div>
              <div>9</div>
              <div>10</div>
              <div>11</div>
              <div>12</div>
              <div>13</div>
              <div>14</div>
              <div>15</div>
              <div>16</div>
              <div>17</div>
              <div>18</div>
              <div>19</div>
              <div>20</div>
              <div>21</div>
              <div>22</div>
              <div>23</div>
              <div>24</div>
              <div>25</div>
              <div>26</div>
              <div>27</div>
              <div>28</div>
              <div>29</div>
              <div>30</div>
            </div>
          </div>
          <div class="schedule">
            <h3>JADWAL PEMATERI</h3>
            <div class="event">
              <div style="background-color: #7b61ff"></div>
              <p>
                Storytelling dalam Pemasaran
                <br />
                09:00 - 10:00 WIB / Irwan
              </p>
            </div>
            <div class="event">
              <div style="background-color: #ff6b6b"></div>
              <p>
                Pemrograman Frontend Modern
                <br />
                12:00 - 13:00 WIB / Irwan
              </p>
            </div>
            <div class="event">
              <div style="background-color: #1dd1a1"></div>
              <p>
                Pengembangan API
                <br />
                14:00 - 15:00 WIB / Irwan
              </p>
            </div>
            <img
              alt="Image of a computer screen displaying code"
              height="200"
              src="https://storage.googleapis.com/a1aa/image/9ZXUf4ySNOyoVKOiDMjh1uvf66He9IN91w2WWVorgFDrUOmnA.jpg"
              width="200"
            />
          </div>
        </div>
      </div>
    </body>
  </html>
</template>

<style>
body {
  font-family: "Roboto", sans-serif;
  margin: 0;
  padding: 0;
  background-color: #f5f5f5;
}
.container {
  display: flex;
  flex-wrap: wrap;
}
.sidebar {
  width: 250px;
  background-color: #2c2c54;
  color: white;
  padding: 20px;
  height: 100lvh;
}
.sidebar h2 {
  font-size: 24px;
  margin-bottom: 20px;
}
.sidebar ul {
  list-style: none;
  padding: 0;
}
.sidebar ul li {
  margin: 20px 0;
}
.sidebar ul li a {
  color: white;
  text-decoration: none;
  font-size: 18px;
}
.sidebar ul li a i {
  margin-right: 10px;
}
.main-content {
  flex: 1;
  padding: 20px;
}
.header {
  display: flex;
  justify-content: space-between;
  align-items: center;
}
.header h1 {
  font-size: 24px;
}
.header .search-bar {
  display: flex;
  align-items: center;
}
.header .search-bar input {
  padding: 10px;
  border: 1px solid #ccc;
  border-radius: 5px;
  margin-right: 10px;
}
.header .search-bar i {
  font-size: 20px;
  color: #ccc;
}
.banner {
  background-color: #7b61ff;
  color: white;
  padding: 20px;
  border-radius: 10px;
  margin: 20px 0;
  display: flex;
  justify-content: space-between;
  align-items: center;
  flex-wrap: wrap;
}
.banner h2 {
  font-size: 24px;
}
.banner p {
  font-size: 16px;
}
.banner .info {
  display: flex;
  align-items: center;
}
.banner .info i {
  margin-right: 10px;
}
.banner .info span {
  margin-right: 20px;
}
.banner button {
  background-color: white;
  color: #7b61ff;
  border: none;
  padding: 10px 20px;
  border-radius: 5px;
  cursor: pointer;
}
.modules {
  display: flex;
  justify-content: space-between;
  margin: 20px 0;
  flex-wrap: wrap;
}
.module {
  background-color: white;
  padding: 20px;
  border-radius: 10px;
  width: 30%;
  box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
  margin-bottom: 20px;
}
.module h3 {
  font-size: 18px;
  margin-bottom: 10px;
}
.module p {
  font-size: 14px;
  color: #666;
}
.module img {
  width: 100%;
  border-radius: 10px;
  margin-bottom: 10px;
}
.scores {
  background-color: white;
  padding: 20px;
  border-radius: 10px;
  box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
}
.scores table {
  width: 100%;
  border-collapse: collapse;
}
.scores table th,
.scores table td {
  padding: 10px;
  text-align: left;
  border-bottom: 1px solid #ccc;
}
.scores table th {
  background-color: #f5f5f5;
}
.scores table td a {
  color: #7b61ff;
  text-decoration: none;
}
.right-sidebar {
  width: 300px;
  padding: 20px;
}
.right-sidebar .welcome {
  background-color: white;
  padding: 20px;
  border-radius: 10px;
  box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
  text-align: center;
}
.right-sidebar .welcome img {
  width: 80px;
  height: 80px;
  border-radius: 50%;
  margin-bottom: 10px;
}
.right-sidebar .welcome h3 {
  font-size: 18px;
  margin-bottom: 5px;
}
.right-sidebar .welcome p {
  font-size: 14px;
  color: #666;
}
.right-sidebar .calendar {
  background-color: white;
  padding: 20px;
  border-radius: 10px;
  box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
  margin: 20px 0;
}
.right-sidebar .calendar h3 {
  font-size: 18px;
  margin-bottom: 10px;
}
.right-sidebar .calendar .days {
  display: flex;
  justify-content: space-between;
  flex-wrap: wrap;
}
.right-sidebar .calendar .days div {
  width: 30px;
  height: 30px;
  background-color: #f5f5f5;
  display: flex;
  justify-content: center;
  align-items: center;
  border-radius: 5px;
  margin-bottom: 5px;
}
.right-sidebar .schedule {
  background-color: white;
  padding: 20px;
  border-radius: 10px;
  box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
}
.right-sidebar .schedule h3 {
  font-size: 18px;
  margin-bottom: 10px;
}
.right-sidebar .schedule .event {
  display: flex;
  align-items: center;
  margin-bottom: 10px;
}
.right-sidebar .schedule .event div {
  width: 10px;
  height: 10px;
  border-radius: 50%;
  margin-right: 10px;
}
.right-sidebar .schedule .event p {
  font-size: 14px;
  color: #666;
}
.right-sidebar .schedule .event img {
  width: 100%;
  border-radius: 10px;
}
@media (max-width: 768px) {
  .sidebar {
    width: 100%;
    height: auto;
  }
  .main-content {
    width: 100%;
  }
  .right-sidebar {
    width: 100%;
  }
  .modules {
    flex-direction: column;
  }
  .module {
    width: 100%;
  }
}
</style>
