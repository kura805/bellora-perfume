<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>Bellora | Helsia of Dawn - Extrait de Parfum</title>
  <link href="https://fonts.googleapis.com/css2?family=Cormorant+Garamond:wght@500;600;700&family=Montserrat:wght@300;400&display=swap" rel="stylesheet">
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">
  <style>
    :root {
      --gold: #c6a972;
      --dawn-pink: #e8c8c8;
      --sunrise: #d4a373;
      --twilight: #7a5d6e;
      --text: #4a3e3c;
      --green-tea: #d1d9c7;
      --silver-bell: #e8e8e8;
    }
    
    body {
      background: linear-gradient(135deg, #fdf6f8 0%, #f9e9e9 100%);
      font-family: 'Cormorant Garamond', serif;
      color: var(--text);
      margin: 0;
      padding: 0;
      min-height: 100vh;
      position: relative;
      overflow-x: hidden;
    }
    
    .gold-accent {
      color: var(--gold);
    }
    
    .container {
      max-width: 1000px;
      margin: 0 auto;
      padding: 60px 30px;
      position: relative;
    }
    
    .header {
      text-align: center;
      margin-bottom: 50px;
      position: relative;
    }
    
    .brand-name {
      font-size: 24px;
      letter-spacing: 5px;
      color: var(--twilight);
      margin-bottom: 10px;
      text-transform: uppercase;
      font-family: 'Montserrat', sans-serif;
    }
    
    h1 {
      font-size: 72px;
      font-weight: 300;
      margin: 10px 0;
      color: var(--twilight);
      letter-spacing: 2px;
      line-height: 1.1;
    }
    
    .subtitle {
      font-size: 24px;
      font-style: italic;
      color: var(--sunrise);
      margin-top: 15px;
    }
    
    .divider {
      width: 150px;
      height: 1px;
      background: linear-gradient(to right, transparent, var(--gold), transparent);
      margin: 40px auto;
      position: relative;
    }
    
    .divider:before, .divider:after {
      content: "❀";
      position: absolute;
      color: var(--gold);
      top: -12px;
      font-size: 20px;
    }
    
    .divider:before {
      left: -5px;
    }
    
    .divider:after {
      right: -5px;
    }
    
    .product-showcase {
      display: flex;
      align-items: center;
      gap: 60px;
      margin: 60px 0;
    }
    
    .product-image-container {
      flex: 1;
      position: relative;
      min-width: 350px;
    }
    
    .product-image {
      width: 100%;
      border-radius: 5px;
      box-shadow: 0 30px 60px -20px rgba(122, 93, 110, 0.3);
      border: 15px solid white;
      transition: transform 0.5s ease;
      object-fit: cover;
      height: 500px;
    }
    
    .product-image:hover {
      transform: scale(1.02);
    }
    
    .product-details {
      flex: 1;
    }
    
    .detail-section {
      margin-bottom: 40px;
    }
    
    h2 {
      font-size: 28px;
      color: var(--twilight);
      margin-bottom: 20px;
      position: relative;
      display: inline-block;
    }
    
    h2:after {
      content: "";
      position: absolute;
      bottom: -8px;
      left: 0;
      width: 60%;
      height: 1px;
      background: var(--gold);
    }
    
    p {
      font-size: 18px;
      line-height: 1.8;
      margin-bottom: 20px;
    }
    
    .fragrance-notes {
      display: flex;
      justify-content: space-between;
      margin-top: 30px;
    }
    
    .note-column {
      flex: 1;
      text-align: center;
      padding: 0 15px;
      position: relative;
    }
    
    .note-column:not(:last-child):after {
      content: "";
      position: absolute;
      right: 0;
      top: 20%;
      height: 60%;
      width: 1px;
      background: linear-gradient(to bottom, transparent, var(--gold), transparent);
    }
    
    .note-title {
      font-size: 20px;
      margin-bottom: 15px;
      font-weight: 600;
      position: relative;
      display: inline-block;
    }
    
    .top-notes .note-title {
      color: var(--sunrise);
    }
    
    .heart-notes .note-title {
      color: var(--twilight);
    }
    
    .base-notes .note-title {
      color: var(--gold);
    }
    
    .note-list {
      list-style: none;
      padding: 0;
      font-family: 'Montserrat', sans-serif;
      font-size: 15px;
    }
    
    .note-list li {
      margin-bottom: 12px;
      position: relative;
      padding-left: 20px;
    }
    
    .top-notes .note-list li:before {
      content: "☀️";
      position: absolute;
      left: 0;
    }
    
    .heart-notes .note-list li:before {
      content: "🌸";
      position: absolute;
      left: 0;
    }
    
    .base-notes .note-list li:before {
      content: "🌙";
      position: absolute;
      left: 0;
    }
    
    .specs-grid {
      display: grid;
      grid-template-columns: repeat(2, 1fr);
      gap: 15px;
      margin-top: 20px;
    }
    
    .spec-item {
      font-family: 'Montserrat', sans-serif;
    }
    
    .spec-label {
      font-weight: 600;
      color: var(--twilight);
    }
    
    .price-container {
      background: rgba(255, 255, 255, 0.7);
      padding: 40px;
      border-radius: 5px;
      text-align: center;
      margin: 50px 0;
      border: 1px solid rgba(198, 169, 114, 0.3);
    }
    
    .price {
      font-size: 42px;
      color: var(--twilight);
      margin: 10px 0;
      font-weight: 300;
    }
    
    .price small {
      font-size: 24px;
      color: var(--sunrise);
    }
    
    button {
      background-color: var(--twilight);
      color: white;
      border: none;
      padding: 16px 45px;
      font-size: 18px;
      letter-spacing: 1px;
      margin-top: 30px;
      cursor: pointer;
      transition: all 0.3s ease;
      font-family: 'Cormorant Garamond', serif;
      border-radius: 3px;
    }
    
    button:hover {
      background-color: var(--sunrise);
      transform: translateY(-3px);
    }
    
    .floral-decoration {
      position: absolute;
      opacity: 0.05;
      z-index: -1;
      font-size: 200px;
      color: var(--gold);
    }
    
    .floral-1 {
      top: 50px;
      left: -50px;
      transform: rotate(-15deg);
    }
    
    .floral-2 {
      bottom: 50px;
      right: -50px;
      transform: rotate(15deg);
    }
    
    @media (max-width: 900px) {
      .product-showcase {
        flex-direction: column;
      }
      
      .product-image-container {
        min-width: auto;
      }
      
      .product-image {
        height: 400px;
      }
      
      h1 {
        font-size: 56px;
      }
      
      .note-column:not(:last-child):after {
        display: none;
      }
    }
  </style>
</head>
<body>
  <div class="container">
    <i class="fas fa-spa floral-decoration floral-1"></i>
    <i class="fas fa-spa floral-decoration floral-2"></i>
    
    <div class="header">
      <div class="brand-name">Bellora</div>
      <h1>Helsia <span class="gold-accent">of Dawn</span></h1>
      <div class="subtitle">Extrait de Parfum • 20-30% Concentration</div>
      <div class="divider"></div>
      <p>A luminous ode to morning's first light, where silver bell flowers glisten with dew and the air hums with the promise of a new day.</p>
    </div>
    
    <div class="product-showcase">
      <div class="product-image-container">
        <img src="https://www.dropbox.com/scl/fi/mtdpmckljxogygqyvcgb2/1745654439068.jpg?rlkey=7l1m4r431gfc6rjr0g66uyufr&st=a0svkrtk&dl=0&raw=1" alt="Helsia of Dawn Perfume Bottle" class="product-image">
      </div>
      
      <div class="product-details">
        <div class="detail-section">
          <h2>The Essence</h2>
          <p>Helsia of Dawn captures the magical moment when night transitions to day. The fragrance opens with the crispness of morning dew, unfolds into a delicate floral heart kissed by the first sunlight, and settles into a warm, skin-like embrace as the day awakens.</p>
          <p>This 20-30% concentration extrait de parfum by Bellora features rare Halesia Carolina (silver bell flower) at its heart, creating a uniquely luminous floral signature that lasts from dawn till dusk.</p>
        </div>
        
        <div class="detail-section">
          <h2>Fragrance Notes</h2>
          <div class="fragrance-notes">
            <div class="note-column top-notes">
              <div class="note-title">Top Notes</div>
              <ul class="note-list">
                <li>Bergamot</li>
                <li>Green Tea</li>
                <li>Orange Blossom</li>
              </ul>
            </div>
            <div class="note-column heart-notes">
              <div class="note-title">Heart Notes</div>
              <ul class="note-list">
                <li>Halesia Carolina</li>
                <li>Jasmine Sambac</li>
                <li>Lily of the Valley</li>
              </ul>
            </div>
            <div class="note-column base-notes">
              <div class="note-title">Base Notes</div>
              <ul class="note-list">
                <li>Sandalwood</li>
                <li>White Musk</li>
              </ul>
            </div>
          </div>
        </div>
        
        <div class="detail-section">
          <h2>Technical Details</h2>
          <div class="specs-grid">
            <div class="spec-item">
              <div class="spec-label">Concentration</div>
              <div>Extrait de Parfum (20-30%)</div>
            </div>
            <div class="spec-item">
              <div class="spec-label">Volume</div>
              <div>50ml | 1.7oz</div>
            </div>
            <div class="spec-item">
              <div class="spec-label">Longevity</div>
              <div>10-12 hours</div>
            </div>
            <div class="spec-item">
              <div class="spec-label">Sillage</div>
              <div>Moderate to Strong</div>
            </div>
            <div class="spec-item">
              <div class="spec-label">Season</div>
              <div>Spring, Summer</div>
            </div>
            <div class="spec-item">
              <div class="spec-label">Occasion</div>
              <div>Daytime, Weddings, Special Events</div>
            </div>
          </div>
        </div>
      </div>
    </div>
    
    <div class="price-container">
      <h2>Pricing</h2>
      <div class="price">$158 <small>USD</small></div>
      <p>50ml handcrafted bottle with silver-plated cap</p>
      <p>Presented in Bellora's signature dawn-inspired packaging</p>
      <button onclick="getInstagramLink()">
        <i class="fas fa-envelope"></i> Inquire for Purchase
      </button>
    </div>
  </div>

  <script>
    function getInstagramLink() {
      window.location.href = "https://www.instagram.com/kura.nilson/";
    }
  </script>
</body>
</html>
