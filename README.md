<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Seu Nome | Profissão/Área</title>
    <style>
        /* Estilos modernos e clean */
        :root {
            --primary: #2c3e50;
            --secondary: #3498db;
            --light: #ecf0f1;
            --dark: #1a252f;
        }
        
        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            line-height: 1.6;
            margin: 0;
            padding: 0;
            color: var(--dark);
            background-color: var(--light);
        }
        
        header {
            background: linear-gradient(135deg, var(--primary), var(--secondary));
            color: white;
            text-align: center;
            padding: 4rem 1rem;
            clip-path: polygon(0 0, 100% 0, 100% 90%, 0 100%);
        }
        
        .profile-img {
            width: 150px;
            height: 150px;
            border-radius: 50%;
            object-fit: cover;
            border: 5px solid white;
            box-shadow: 0 5px 15px rgba(0,0,0,0.2);
        }
        
        h1 {
            margin: 1rem 0;
            font-size: 2.5rem;
        }
        
        .tagline {
            font-size: 1.2rem;
            opacity: 0.9;
            max-width: 600px;
            margin: 0 auto;
        }
        
        .container {
            max-width: 1100px;
            margin: 2rem auto;
            padding: 0 2rem;
        }
        
        section {
            background: white;
            border-radius: 8px;
            box-shadow: 0 3px 10px rgba(0,0,0,0.1);
            padding: 2rem;
            margin-bottom: 2rem;
        }
        
        h2 {
            color: var(--secondary);
            border-bottom: 2px solid var(--light);
            padding-bottom: 0.5rem;
        }
        
        .skills {
            display: flex;
            flex-wrap: wrap;
            gap: 1rem;
        }
        
        .skill-tag {
            background: var(--light);
            padding: 0.5rem 1rem;
            border-radius: 20px;
            font-size: 0.9rem;
        }
        
        footer {
            text-align: center;
            padding: 2rem;
            background: var(--dark);
            color: white;
        }
        
        .social-links a {
            color: white;
            margin: 0 10px;
            font-size: 1.5rem;
            text-decoration: none;
        }
        
        @media (max-width: 768px) {
            h1 {
                font-size: 2rem;
            }
            .container {
                padding: 0 1rem;
            }
        }
    </style>
</head>
<body>
    <header>
        <img src="https://via.placeholder.com/150" alt="Sua Foto" class="profile-img">
        <h1>Seu Nome Completo</h1>
        <p class="tagline">Desenvolvedor Web | Analista de Dados | [Sua Especialidade]</p>
    </header>
    
    <div class="container">
        <section id="sobre">
            <h2>Sobre Mim</h2>
            <p>Olá! Sou um profissional apaixonado por [sua área] com [X] anos de experiência. Minha jornada começou quando [breve história pessoal relevante]. Acredito que [sua filosofia profissional].</p>
        </section>
        
        <section id="habilidades">
            <h2>Habilidades Técnicas</h2>
            <div class="skills">
                <span class="skill-tag">HTML5/CSS3</span>
                <span class="skill-tag">JavaScript</span>
                <span class="skill-tag">Python</span>
                <span class="skill-tag">Git</span>
                <span class="skill-tag">SQL</span>
                <span class="skill-tag">React</span>
                <!-- Adicione mais habilidades -->
            </div>
        </section>
        
        <section id="experiencia">
            <h2>Experiência Profissional</h2>
            <h3>Cargo Principal</h3>
            <p><strong>Empresa</strong> | 2020 - Presente</p>
            <ul>
                <li>Responsável por [principais atividades]</li>
                <li>Desenvolvi [projeto importante] que resultou em [benefício mensurável]</li>
                <li>Liderança de equipe de [X] pessoas</li>
            </ul>
            
            <h3>Cargo Anterior</h3>
            <p><strong>Outra Empresa</strong> | 2018 - 2020</p>
            <ul>
                <li>[Realização importante]</li>
                <li>[Outro ponto relevante]</li>
            </ul>
        </section>
        
        <section id="contato">
            <h2>Contato</h2>
            <p>Email: <a href="mailto:seu@email.com">seu@email.com</a></p>
            <p>Telefone: (XX) XXXX-XXXX</p>
            <p>Disponível para freelances e oportunidades de colaboração.</p>
        </section>
    </div>
    
    <footer>
        <div class="social-links">
            <a href="#"><i class="fab fa-linkedin"></i></a>
            <a href="#"><i class="fab fa-github"></i></a>
            <a href="#"><i class="fab fa-twitter"></i></a>
            <!-- Ícones do Font Awesome -->
        </div>
        <p>&copy; <span id="year"></span> Seu Nome. Todos os direitos reservados.</p>
    </footer>

    <script>
        // Atualiza o ano automaticamente
        document.getElementById('year').textContent = new Date().getFullYear();
        
        // Efeito simples de scroll suave
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                document.querySelector(this.getAttribute('href')).scrollIntoView({
                    behavior: 'smooth'
                });
            });
        });
    </script>
    
    <!-- Adicione isso no <head> para ícones -->
    <!-- <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.4/css/all.min.css"> -->
</body>
</html>
