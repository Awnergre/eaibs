body {
  font-family: Arial, sans-serif;
  background: #040720;
  margin: 0;
  padding: 20px;
  text-align: center;
}

h1 {
  color: #000;
}

.produk-container {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  gap: 15px;
  margin-top: 30px;
}

.produk-card {
  background: #040720;
  width: calc(100% / 6 - 15px);
  border-radius: 12px;
  box-shadow: 0 0 10px rgba(0,0,0,0.1);
  overflow: hidden;
  transition: transform 0.3s ease;
  border: 2px solid white;
  box-sizing: border-box;
}

.produk-card:hover {
  transform: scale(1.03);
}

.produk-card img {
  width: 100%;
  height: 250px;
  object-fit: cover;
}

.produk-info {
  padding: 15px;
}

.produk-info h2 {
  font-size: 20px;
  margin: 10px 0 5px;
  color: #fff;
}

.produk-info p {
  color: #FFA500;
  margin: 5px 0 10px;
  font-weight: bold;
  font-size: 18px;
}

.produk-info a {
  display: inline-block;
  padding: 10px 20px;
  background-color: #25d366;
  color: white;
  text-decoration: none;
  border-radius: 6px;
  font-weight: bold;
  transition: background-color 0.3s ease;
}

.produk-info a:hover {
  background-color: #1ebe57;
}

/* Responsive */
@media (max-width: 1200px) {
  .produk-card {
    width: calc(100% / 4 - 15px); /* 4 kartu per baris */
  }
}

@media (max-width: 900px) {
  .produk-card {
    width: calc(100% / 3 - 15px); /* 3 kartu per baris */
  }
}

@media (max-width: 600px) {
  .produk-card {
    width: calc(100% / 3 - 15px); /* tetap 3 kartu per baris di HP */
  }
  .produk-container {
    justify-content: flex-start;
  }
}
