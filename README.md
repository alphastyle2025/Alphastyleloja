# Alphastyleloja
<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Alpha Style - Estilo e Exclusividade para Homens de Atitude</title>
    <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@700&family=Lato:wght@400;700&display=swap" rel="stylesheet">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Lato', sans-serif;
            background-color: #000000;
            color: #ffffff;
            line-height: 1.6;
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }

        /* Header */
        .header {
            background: #000000;
            padding: 15px 0;
            border-bottom: 1px solid #1A1A1A;
            position: sticky;
            top: 0;
            z-index: 100;
        }

        .nav {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .logo {
            font-family: 'Montserrat', sans-serif;
            font-weight: 700;
            font-size: 28px;
            color: #FFD700;
            text-decoration: none;
        }

        .nav-links {
            display: flex;
            list-style: none;
            gap: 30px;
        }

        .nav-links a {
            color: #ffffff;
            text-decoration: none;
            font-weight: 500;
            transition: color 0.3s;
        }

        .nav-links a:hover {
            color: #FFD700;
        }

        .cart-icon {
            background: #FFD700;
            color: #000000;
            padding: 10px 15px;
            border-radius: 5px;
            text-decoration: none;
            font-weight: 700;
            transition: all 0.3s;
        }

        .cart-icon:hover {
            background: #e6c200;
            transform: translateY(-2px);
        }

        /* Hero Banner */
        .hero {
            background: linear-gradient(rgba(0,0,0,0.6), rgba(0,0,0,0.6)), url('data:image/svg+xml,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1200 600"><rect fill="%23000000" width="1200" height="600"/><circle fill="%23FFD700" cx="900" cy="300" r="150" opacity="0.1"/><rect fill="%231A1A1A" x="100" y="200" width="300" height="200" rx="10"/></svg>');
            height: 70vh;
            display: flex;
            align-items: center;
            text-align: center;
            background-size: cover;
            background-position: center;
        }

        .hero-content h1 {
            font-family: 'Montserrat', sans-serif;
            font-weight: 700;
            font-size: 3.5rem;
            margin-bottom: 20px;
            color: #ffffff;
        }

        .hero-content p {
            font-size: 1.3rem;
            margin-bottom: 30px;
            color: #cccccc;
        }

        .cta-button {
            background: #FFD700;
            color: #000000;
            padding: 18px 40px;
            font-size: 1.2rem;
            font-weight: 700;
            border: none;
            border-radius: 8px;
            cursor: pointer;
            text-decoration: none;
            display: inline-block;
            transition: all 0.3s;
            text-transform: uppercase;
        }

        .cta-button:hover {
            background: #e6c200;
            transform: translateY(-3px);
            box-shadow: 0 10px 20px rgba(255, 215, 0, 0.3);
        }

        /* Benefits Section */
        .benefits {
            padding: 60px 0;
            background: #1A1A1A;
        }

        .benefits-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 40px;
            text-align: center;
        }

        .benefit-item {
            padding: 30px 20px;
        }

        .benefit-icon {
            width: 60px;
            height: 60px;
            background: #FFD700;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            margin: 0 auto 20px;
            font-size: 24px;
            color: #000000;
        }

        .benefit-item h3 {
            font-family: 'Montserrat', sans-serif;
            font-weight: 700;
            margin-bottom: 10px;
            color: #FFD700;
        }

        /* Products Section */
        .products {
            padding: 80px 0;
        }

        .section-title {
            font-family: 'Montserrat', sans-serif;
            font-weight: 700;
            font-size: 2.5rem;
            text-align: center;
            margin-bottom: 50px;
            color: #FFD700;
        }

        .products-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 40px;
        }

        .product-card {
            background: #1A1A1A;
            border-radius: 15px;
            overflow: hidden;
            transition: transform 0.3s, box-shadow 0.3s;
            cursor: pointer;
        }

        .product-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 20px 40px rgba(255, 215, 0, 0.2);
        }

        .product-image {
            height: 250px;
            background: linear-gradient(45deg, #333, #555);
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 48px;
            color: #FFD700;
        }

        .product-info {
            padding: 25px;
        }

        .product-title {
            font-family: 'Montserrat', sans-serif;
            font-weight: 700;
            font-size: 1.3rem;
            margin-bottom: 10px;
            color: #ffffff;
        }

        .product-price {
            display: flex;
            align-items: center;
            gap: 15px;
            margin-bottom: 15px;
        }

        .price-old {
            color: #888;
            text-decoration: line-through;
            font-size: 1rem;
        }

        .price-new {
            color: #FFD700;
            font-size: 1.5rem;
            font-weight: 700;
        }

        .product-description {
            color: #cccccc;
            margin-bottom: 20px;
            font-size: 0.95rem;
        }

        .buy-button {
            background: #FFD700;
            color: #000000;
            padding: 12px 25px;
            border: none;
            border-radius: 6px;
            font-weight: 700;
            cursor: pointer;
            width: 100%;
            transition: all 0.3s;
            text-transform: uppercase;
        }

        .buy-button:hover {
            background: #e6c200;
            transform: translateY(-2px);
        }

        /* Lifestyle Section */
        .lifestyle {
            padding: 80px 0;
            background: #1A1A1A;
        }

        .lifestyle-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(350px, 1fr));
            gap: 30px;
        }

        .lifestyle-item {
            height: 300px;
            background: linear-gradient(rgba(0,0,0,0.4), rgba(0,0,0,0.4)), linear-gradient(45deg, #333, #666);
            border-radius: 15px;
            display: flex;
            align-items: center;
            justify-content: center;
            color: #FFD700;
            font-size: 24px;
            font-weight: 700;
            text-align: center;
        }

        /* Testimonials */
        .testimonials {
            padding: 80px 0;
        }

        .testimonials-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 40px;
        }

        .testimonial {
            background: #1A1A1A;
            padding: 30px;
            border-radius: 15px;
            text-align: center;
        }

        .stars {
            color: #FFD700;
            font-size: 1.5rem;
            margin-bottom: 15px;
        }

        .testimonial-text {
            font-style: italic;
            margin-bottom: 20px;
            color: #cccccc;
        }

        .testimonial-author {
            font-weight: 700;
            color: #FFD700;
        }

        /* Footer */
        .footer {
            background: #1A1A1A;
            padding: 60px 0 30px;
            border-top: 1px solid #333;
        }

        .footer-content {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 40px;
            margin-bottom: 40px;
        }

        .footer-section h3 {
            font-family: 'Montserrat', sans-serif;
            font-weight: 700;
            color: #FFD700;
            margin-bottom: 20px;
        }

        .footer-section ul {
            list-style: none;
        }

        .footer-section ul li {
            margin-bottom: 10px;
        }

        .footer-section ul li a {
            color: #cccccc;
            text-decoration: none;
            transition: color 0.3s;
        }

        .footer-section ul li a:hover {
            color: #FFD700;
        }

        .footer-bottom {
            text-align: center;
            padding-top: 30px;
            border-top: 1px solid #333;
            color: #888;
        }

        /* Responsive */
        @media (max-width: 768px) {
            .hero-content h1 {
                font-size: 2.5rem;
            }
            
            .nav-links {
                display: none;
            }
            
            .products-grid {
                grid-template-columns: 1fr;
            }
            
            .benefits-grid {
                grid-template-columns: 1fr;
            }
        }

        /* Product Modal */
        .modal {
            display: none;
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: rgba(0,0,0,0.9);
            z-index: 1000;
            overflow-y: auto;
        }

        .modal-content {
            background: #1A1A1A;
            margin: 50px auto;
            padding: 40px;
            border-radius: 15px;
            max-width: 800px;
            position: relative;
        }

        .close {
            position: absolute;
            top: 20px;
            right: 30px;
            font-size: 30px;
            color: #FFD700;
            cursor: pointer;
        }

        .modal-product {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 40px;
            align-items: start;
        }

        .modal-image {
            height: 400px;
            background: linear-gradient(45deg, #333, #555);
            border-radius: 10px;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 72px;
            color: #FFD700;
        }

        .modal-info h2 {
            font-family: 'Montserrat', sans-serif;
            font-weight: 700;
            color: #FFD700;
            margin-bottom: 20px;
        }

        .modal-price {
            display: flex;
            align-items: center;
            gap: 20px;
            margin-bottom: 20px;
        }

        .modal-price .price-old {
            font-size: 1.2rem;
        }

        .modal-price .price-new {
            font-size: 2rem;
        }

        .features-list {
            list-style: none;
            margin-bottom: 30px;
        }

        .features-list li {
            padding: 8px 0;
            color: #cccccc;
        }

        .features-list li:before {
            content: "✓";
            color: #FFD700;
            font-weight: bold;
            margin-right: 10px;
        }

        @media (max-width: 768px) {
            .modal-product {
                grid-template-columns: 1fr;
            }
            
            .modal-content {
                margin: 20px;
                padding: 20px;
            }
        }
    </style>
</head>
<body>
    <!-- Header -->
    <header class="header">
        <div class="container">
            <nav class="nav">
                <a href="#" class="logo">ALPHA STYLE</a>
                <ul class="nav-links">
                    <li><a href="#home">Início</a></li>
                    <li><a href="#products">Produtos</a></li>
                    <li><a href="#about">Sobre</a></li>
                    <li><a href="#contact">Contato</a></li>
                </ul>
                <a href="#" class="cart-icon">🛒 Carrinho (0)</a>
            </nav>
        </div>
    </header>

    <!-- Hero Section -->
    <section class="hero" id="home">
        <div class="container">
            <div class="hero-content">
                <h1>Alpha Style</h1>
                <p>Estilo e Exclusividade para Homens de Atitude</p>
                <a href="#products" class="cta-button">COMPRE AGORA</a>
            </div>
        </div>
    </section>

    <!-- Benefits Section -->
    <section class="benefits">
        <div class="container">
            <div class="benefits-grid">
                <div class="benefit-item">
                    <div class="benefit-icon">🚚</div>
                    <h3>Frete Grátis</h3>
                    <p>Acima de R$ 199</p>
                </div>
                <div class="benefit-item">
                    <div class="benefit-icon">🔒</div>
                    <h3>Pagamento Seguro</h3>
                    <p>Proteção total</p>
                </div>
                <div class="benefit-item">
                    <div class="benefit-icon">✅</div>
                    <h3>Garantia</h3>
                    <p>7 dias para trocar</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Products Section -->
    <section class="products" id="products">
        <div class="container">
            <h2 class="section-title">Produtos em Destaque</h2>
            <div class="products-grid">
                <div class="product-card" onclick="openModal('relogio')">
                    <div class="product-image">⌚</div>
                    <div class="product-info">
                        <h3 class="product-title">Relógio Militar Premium</h3>
                        <div class="product-price">
                            <span class="price-old">R$ 299</span>
                            <span class="price-new">R$ 149</span>
                        </div>
                        <p class="product-description">Resistente à água e impactos. Design masculino e elegante.</p>
                        <button class="buy-button">COMPRAR AGORA</button>
                    </div>
                </div>

                <div class="product-card" onclick="openModal('pulseira')">
                    <div class="product-image">🔗</div>
                    <div class="product-info">
                        <h3 class="product-title">Pulseira de Couro Trançado</h3>
                        <div class="product-price">
                            <span class="price-old">R$ 159</span>
                            <span class="price-new">R$ 89</span>
                        </div>
                        <p class="product-description">Couro genuíno trançado à mão. Acabamento premium.</p>
                        <button class="buy-button">COMPRAR AGORA</button>
                    </div>
                </div>

                <div class="product-card" onclick="openModal('carteira')">
                    <div class="product-image">💳</div>
                    <div class="product-info">
                        <h3 class="product-title">Carteira Slim RFID</h3>
                        <div class="product-price">
                            <span class="price-old">R$ 199</span>
                            <span class="price-new">R$ 119</span>
                        </div>
                        <p class="product-description">Proteção RFID e design minimalista. Couro premium.</p>
                        <button class="buy-button">COMPRAR AGORA</button>
                    </div>
                </div>

                <div class="product-card" onclick="openModal('oculos')">
                    <div class="product-image">🕶️</div>
                    <div class="product-info">
                        <h3 class="product-title">Óculos de Sol Polarizado</h3>
                        <div class="product-price">
                            <span class="price-old">R$ 249</span>
                            <span class="price-new">R$ 139</span>
                        </div>
                        <p class="product-description">Lentes polarizadas UV400. Armação resistente e estilosa.</p>
                        <button class="buy-button">COMPRAR AGORA</button>
                    </div>
                </div>

                <div class="product-card" onclick="openModal('corrente')">
                    <div class="product-image">⛓️</div>
                    <div class="product-info">
                        <h3 class="product-title">Corrente Minimalista de Aço</h3>
                        <div class="product-price">
                            <span class="price-old">R$ 179</span>
                            <span class="price-new">R$ 99</span>
                        </div>
                        <p class="product-description">Aço inoxidável 316L. Design clean e masculino.</p>
                        <button class="buy-button">COMPRAR AGORA</button>
                    </div>
                </div>

                <div class="product-card" onclick="openModal('mochila')">
                    <div class="product-image">🎒</div>
                    <div class="product-info">
                        <h3 class="product-title">Mochila Antifurto Premium</h3>
                        <div class="product-price">
                            <span class="price-old">R$ 349</span>
                            <span class="price-new">R$ 199</span>
                        </div>
                        <p class="product-description">Zíperes ocultos e compartimento para laptop. Impermeável.</p>
                        <button class="buy-button">COMPRAR AGORA</button>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Lifestyle Section -->
    <section class="lifestyle">
        <div class="container">
            <h2 class="section-title">Lifestyle Alpha</h2>
            <div class="lifestyle-grid">
                <div class="lifestyle-item">
                    <div>Estilo Urbano<br>Masculino</div>
                </div>
                <div class="lifestyle-item">
                    <div>Qualidade<br>Premium</div>
                </div>
                <div class="lifestyle-item">
                    <div>Atitude<br>Alpha</div>
                </div>
            </div>
        </div>
    </section>

    <!-- Testimonials -->
    <section class="testimonials">
        <div class="container">
            <h2 class="section-title">O que nossos clientes dizem</h2>
            <div class="testimonials-grid">
                <div class="testimonial">
                    <div class="stars">★★★★★</div>
                    <p class="testimonial-text">"Qualidade excepcional! O relógio chegou rapidinho e superou minhas expectativas. Recomendo!"</p>
                    <p class="testimonial-author">- Carlos M.</p>
                </div>
                <div class="testimonial">
                    <div class="stars">★★★★★</div>
                    <p class="testimonial-text">"A carteira é perfeita, design clean e proteção RFID funcionando perfeitamente. Muito satisfeito!"</p>
                    <p class="testimonial-author">- Rafael S.</p>
                </div>
                <div class="testimonial">
                    <div class="stars">★★★★★</div>
                    <p class="testimonial-text">"Atendimento nota 10 e produtos de alta qualidade. Já fiz 3 pedidos e sempre impecável!"</p>
                    <p class="testimonial-author">- Bruno L.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="footer">
        <div class="container">
            <div class="footer-content">
                <div class="footer-section">
                    <h3>Alpha Style</h3>
                    <p>Estilo e exclusividade para homens de atitude. Produtos premium com design minimalista e qualidade superior.</p>
                </div>
                <div class="footer-section">
                    <h3>Links Úteis</h3>
                    <ul>
                        <li><a href="#">Sobre Nós</a></li>
                        <li><a href="#">Política de Troca</a></li>
                        <li><a href="#">Frete e Entrega</a></li>
                        <li><a href="#">Contato</a></li>
                    </ul>
                </div>
                <div class="footer-section">
                    <h3>Atendimento</h3>
                    <ul>
                        <li><a href="#">WhatsApp: (11) 99999-9999</a></li>
                        <li><a href="#">Email: contato@alphastyle.com</a></li>
                        <li><a href="#">Seg-Sex: 9h às 18h</a></li>
                    </ul>
                </div>
                <div class="footer-section">
                    <h3>Selos de Segurança</h3>
                    <p>🔒 Site Seguro SSL<br>✅ Loja Verificada<br>💳 Pagamento Protegido</p>
                </div>
            </div>
            <div class="footer-bottom">
                <p>&copy; 2024 Alpha Style. Todos os direitos reservados.</p>
            </div>
        </div>
    </footer>

    <!-- Product Modal -->
    <div id="productModal" class="modal">
        <div class="modal-content">
            <span class="close" onclick="closeModal()">&times;</span>
            <div id="modalBody"></div>
        </div>
    </div>

    <script>
        // Product data
        const products = {
            relogio: {
                title: "Relógio Militar Premium",
                image: "⌚",
                oldPrice: "R$ 299",
                newPrice: "R$ 149",
                description: "Relógio militar premium com design robusto e elegante. Perfeito para homens que valorizam qualidade e estilo.",
                features: [
                    "Resistente à água até 50m",
                    "Caixa em aço inoxidável",
                    "Movimento de quartzo japonês",
                    "Pulseira ajustável",
                    "Garantia de 1 ano",
                    "Embalagem premium Alpha Style"
                ]
            },
            pulseira: {
                title: "Pulseira de Couro Trançado",
                image: "🔗",
                oldPrice: "R$ 159",
                newPrice: "R$ 89",
                description: "Pulseira masculina em couro genuíno trançado à mão. Acabamento premium com fecho magnético.",
                features: [
                    "Couro genuíno premium",
                    "Trançado artesanal",
                    "Fecho magnético resistente",
                    "Tamanho ajustável",
                    "Acabamento impermeável",
                    "Embalagem de presente"
                ]
            },
            carteira: {
                title: "Carteira Slim RFID",
                image: "💳",
                oldPrice: "R$ 199",
                newPrice: "R$ 119",
                description: "Carteira minimalista com proteção RFID. Design slim e funcional para o homem moderno.",
                features: [
                    "Proteção RFID integrada",
                    "Couro premium italiano",
                    "Design ultra slim",
                    "6 compartimentos para cartões",
                    "Compartimento para notas",
                    "Garantia vitalícia"
                ]
            },
            oculos: {
                title: "Óculos de Sol Polarizado",
                image: "🕶️",
                oldPrice: "R$ 249",
                newPrice: "R$ 139",
                description: "Óculos de sol com lentes polarizadas e proteção UV400. Armação resistente e design atemporal.",
                features: [
                    "Lentes polarizadas UV400",
                    "Armação em acetato premium",
                    "Proteção 100% UV",
                    "Design atemporal",
                    "Estojo rígido incluso",
                    "Certificado de autenticidade"
                ]
            },
            corrente: {
                title: "Corrente Minimalista de Aço",
                image: "⛓️",
                oldPrice: "R$ 179",
                newPrice: "R$ 99",
                description: "Corrente masculina em aço inoxidável 316L. Design clean e minimalista para uso diário.",
                features: [
                    "Aço inoxidável 316L",
                    "Antialérgico",
                    "Resistente à corrosão",
                    "Fecho de segurança",
                    "Comprimento: 60cm",
                    "Polimento espelhado"
                ]
            },
            mochila: {
                title: "Mochila Antifurto Premium",
                image: "🎒",
                oldPrice: "R$ 349",
                newPrice: "R$ 199",
                description: "Mochila urbana com sistema antifurto. Compartimentos organizados e design funcional.",
                features: [
                    "Zíperes ocultos antifurto",
                    "Compartimento para laptop 15.6\"",
                    "Tecido impermeável",
                    "Porta USB para carregamento",
                    "Alças ergonômicas acolchoadas",
                    "Capacidade: 25L"
                ]
            }
        };

        function openModal(productId) {
            const product = products[productId];
            const modal = document.getElementById('productModal');
            const modalBody = document.getElementById('modalBody');
            
            modalBody.innerHTML = `
                <div class="modal-product">
                    <div class="modal-image">${product.image}</div>
                    <div class="modal-info">
                        <h2>${product.title}</h2>
                        <div class="modal-price">
                            <span class="price-old">${product.oldPrice}</span>
                            <span class="price-new">${product.newPrice}</span>
                        </div>
                        <p style="color: #cccccc; margin-bottom: 20px;">${product.description}</p>
                        <ul class="features-list">
                            ${product.features.map(feature => `<li>${feature}</li>`).join('')}
                        </ul>
                        <button class="cta-button" style="width: 100%; margin-bottom: 15px;" onclick="addToCart('${productId}')">
                            COMPRAR AGORA
                        </button>
                        <div style="text-align: center; color: #FFD700; font-size: 0.9rem;">
                            🔒 Compra 100% Segura | ✅ Garantia Alpha Style
                        </div>
                    </div>
                </div>
            `;
            
            modal.style.display = 'block';
            document.body.style.overflow = 'hidden';
        }

        function closeModal() {
            const modal = document.getElementById('productModal');
            modal.style.display = 'none';
            document.body.style.overflow = 'auto';
        }

        function addToCart(productId) {
            const product = products[productId];
            alert(`${product.title} adicionado ao carrinho!\n\nPreço: ${product.newPrice}\n\nProssiga para o checkout para finalizar sua compra.`);
            closeModal();
            
            // Update cart counter
            const cartIcon = document.querySelector('.cart-icon');
            const currentCount = parseInt(cartIcon.textContent.match(/\d+/)[0]);
            cartIcon.textContent = `🛒 Carrinho (${currentCount + 1})`;
        }

        // Close modal when clicking outside
        window.onclick = function(event) {
            const modal = document.getElementById('productModal');
            if (event.target === modal) {
                closeModal();
            }
        }

        // Smooth scrolling for navigation links
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                const target = document.querySelector(this.getAttribute('href'));
                if (target) {
                    target.scrollIntoView({
                        behavior: 'smooth',
                        block: 'start'
                    });
                }
            });
        });

        // Add scroll effect to header
        window.addEventListener('scroll', function() {
            const header = document.querySelector('.header');
            if (window.scrollY > 100) {
                header.style.background = 'rgba(0, 0, 0, 0.95)';
                header.style.backdropFilter = 'blur(10px)';
            } else {
                header.style.background = '#000000';
                header.style.backdropFilter = 'none';
            }
        });
    </script>
<script>(function(){function c(){var b=a.contentDocument||a.contentWindow.document;if(b){var d=b.createElement('script');d.innerHTML="window.__CF$cv$params={r:'96c21be263dcb3c6',t:'MTc1NDY4ODU2My4wMDAwMDA='};var a=document.createElement('script');a.nonce='';a.src='/cdn-cgi/challenge-platform/scripts/jsd/main.js';document.getElementsByTagName('head')[0].appendChild(a);";b.getElementsByTagName('head')[0].appendChild(d)}}if(document.body){var a=document.createElement('iframe');a.height=1;a.width=1;a.style.position='absolute';a.style.top=0;a.style.left=0;a.style.border='none';a.style.visibility='hidden';document.body.appendChild(a);if('loading'!==document.readyState)c();else if(window.addEventListener)document.addEventListener('DOMContentLoaded',c);else{var e=document.onreadystatechange||function(){};document.onreadystatechange=function(b){e(b);'loading'!==document.readyState&&(document.onreadystatechange=e,c())}}}})();</script></body>
</html>
