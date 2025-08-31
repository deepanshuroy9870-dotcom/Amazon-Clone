.scroll-container {
  width: 100%;
  overflow: hidden;
  background: #5c7c9a; 
  white-space: nowrap;
}

.scroll-text {
  display: inline-block;
  padding-left: 100%; 
  animation: scroll-left 6s linear infinite;
  font-size: 20px;
  color: white;
  font-weight: bold;
}

@keyframes scroll-left {
  0% {
    transform: translateX(30%);
  }
  100% {
    transform: translateX(-100%);
  }
}
    body {
      font-family: Arial, sans-serif;
      margin: 0;
      padding: 20px;
      background: #f4f4f4;
    }

    h1 {
      text-align: center;
      margin-bottom: 20px;
    }

    /* Container for Items */
    .Item-Container {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
      gap: 20px;
    }

    /* Card Style */
    .card {
      background: #fff;
      border-radius: 10px;
      overflow: hidden;
      box-shadow: 0px 2px 8px rgba(0,0,0,0.1);
      transition: transform 0.3s ease, box-shadow 0.3s ease;
      cursor: pointer;
    }

    /* Hover Effect on Card */
    .card:hover {
      transform: translateY(-10px) scale(1.03);
      box-shadow: 0px 6px 20px rgba(0,0,0,0.2);
    }

    /* Image Style */
    .card img {
      width: 100%;
      height: 200px;
      object-fit: cover;
      transition: transform 0.4s ease;
    }

    .card:hover img {
      transform: scale(1.1);
    }

    /* Card Body */
    .card-body {
      padding: 15px;
    }

    /* Offer Tag */
    .offer {
      background: linear-gradient(to right, #ffd700, #ffcc00);
      padding: 5px 10px;
      font-weight: bold;
      text-align: center;
      border-radius: 5px;
      margin-bottom: 10px;
    }

    /* Title */
    .title {
      font-size: 16px;
      font-weight: bold;
      margin: 10px 0;
      transition: all 0.3s ease;
    }

    /* Rating */
    .rating {
      margin: 5px 0;
      font-size: 14px;
    }

    .rating span {
      padding: 2px 5px;
      border-radius: 4px;
    }

    .rating .festival {
      background: blue;
      color: white;
    }

    .rating .star {
      color: gold;
    }

    /* Price Section */
    .price {
      font-size: 18px;
      font-weight: bold;
      color: #007bff;
      transition: all 0.3s ease;
    }

    .old-price {
      color: gray;
      margin-left: 10px;
      font-size: 14px;
    }

    .discount {
      color: brown;
      font-weight: bold;
    }

    /* Gold Membership */
    .gold {
      margin-top: 10px;
      background: #fff3cd;
      padding: 5px;
      border-radius: 5px;
      font-weight: bold;
      transition: all 0.3s ease;
    }

    /* Glow Effect on Hover (text) */
    .title:hover, .price:hover, .gold:hover, .offer:hover {
      color: #ffffff;
      text-shadow: 0 0 5px #000000, 0 0 10px #767575, 0 0 20px #fafafa;
      transform: scale(1.05);
    }

    /* Responsive */
    @media(max-width: 600px) {
      .card img {
        height: 150px;
      }
    }# Amazon-Clone
