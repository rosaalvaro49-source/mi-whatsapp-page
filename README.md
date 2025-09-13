<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Contacto por WhatsApp</title>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/qrious/4.0.2/qrious.min.js"></script>
    <style>
        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            background: linear-gradient(135deg, #25D366, #128C7E, #075E54);
            min-height: 100vh;
            display: flex;
            align-items: center;
            justify-content: center;
            padding: 20px;
        }
        .container {
            background: rgba(255,255,255,0.95);
            border-radius: 20px;
            padding: 40px;
            text-align: center;
            box-shadow: 0 20px 40px rgba(0,0,0,0.1);
            max-width: 500px;
            width: 100%;
            animation: slideUp 0.8s ease-out;
        }
        @keyframes slideUp {
            from {opacity: 0;transform: translateY(30px);}
            to {opacity: 1;transform: translateY(0);}
        }
        .whatsapp-icon {
            width: 80px; height: 80px; margin: 0 auto 20px;
            background: #25D366; border-radius: 50%;
            display: flex; align-items: center; justify-content: center;
            animation: bounce 2s infinite;
        }
        @keyframes bounce {
            0%,20%,50%,80%,100% {transform: translateY(0);}
            40% {transform: translateY(-10px);}
            60% {transform: translateY(-5px);}
        }
        .whatsapp-icon svg {width: 50px; height: 50px; fill: white;}
        h1 {color: #075E54; margin-bottom: 10px; font-size: 28px; font-weight: 700;}
        .subtitle {color: #666; margin-bottom: 30px; font-size: 16px;}
        .whatsapp-btn {
            background: linear-gradient(135deg, #25D366, #128C7E);
            color: white; border: none; padding: 15px 30px; border-radius: 50px;
            font-size: 18px; font-weight: 600; cursor: pointer; text-decoration: none;
            display: inline-flex; align-items: center; gap: 10px; transition: all 0.3s ease;
            margin-bottom: 30px; box-shadow: 0 5px 15px rgba(37,211,102,0.3);
        }
        .whatsapp-btn:hover {
            transform: translateY(-2px);
            box-shadow: 0 10px 25px rgba(37,211,102,0.4);
            background: linear-gradient(135deg, #128C7E, #25D366);
        }
        .qr-section {
            border-top: 2px solid #eee; padding-top: 30px; margin-top: 30px;
        }
        .qr-title {
            color: #075E54; margin-bottom: 15px; font-size: 20px; font-weight: 600;
        }
        #qr-code {
            margin: 20px auto; padding: 20px; background: white; border-radius: 15px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.1); display: inline-block;
        }
        .phone-number {
            background: #f0f0f0; padding: 10px 20px; border-radius: 25px;
            margin: 20px 0; font-family: monospace; font-size: 18px; color: #075E54; font-weight: bold;
        }
        .instructions {
            color: #666; font-size: 14px; line-height: 1.6; margin-top: 20px;
        }
        @media (max-width:480px) {
            .container {padding: 30px 20px;}
            h1 {font-size: 24px;}
            .whatsapp-btn {padding: 12px 25px; font-size: 16px;}
        }
    </style>
</head>
<body>
    <div class="container">
        <div class="whatsapp-icon">
            <svg viewBox="0 0 24 24"><path d="M17.472 14.382c-.297-.149-1.758-.867-2.03-.967-.273-.099-.471-.148-.67.15-.197.297-.767.966-.94 1.164-.173.199-.347.223-.644.075-.297-.15-1.255-.463-2.39-1.475-.883-.788-1.48-1.761-1.653-2.059-.173-.297-.018-.458.13-.606.134-.133.298-.347.446-.52.149-.174.198-.298.298-.497.099-.198.05-.371-.025-.52-.075-.149-.669-1.612-.916-2.207-.242-.579-.487-.5-.669-.51-.173-.008-.371-.01-.57-.01-.198 0-.52.074-.792.372-.272.297-1.04 1.016-1.04 2.479 0 1.462 1.065 2.875 1.213 3.074.149.198 2.096 3.2 5.077 4.487.709.306 1.262.489 1.694.625.712.227 1.36.195 1.871.118.571-.085 1.758-.719 2.006-1.413.248-.694.248-1.289.173-1.413-.074-.124-.272-.198-.57-.347m-5.421 7.403h-.004a9.87 9.87 0 01-5.031-1.378l-.361-.214-3.741.982.998-3.648-.235-.374a9.86 9.86 0 01-1.51-5.26c.001-5.45 4.436-9.884 9.888-9.884 2.64 0 5.122 1.03 6.988 2.898a9.825 9.825 0 012.893 6.994c-.003 5.45-4.437 9.884-9.885 9.884m8.413-18.297A11.815 11.815 0 0012.05 0C5.495 0 .16 5.335.157 11.892c0 2.096.547 4.142 1.588 5.945L.057 24l6.305-1.654a11.882 11.882 0 005.683 1.448h.005c6.554 0 11.890-5.335 11.893-11.893A11.821 11.821 0 0020.893 3.506"/></svg>
        </div>
        <h1>¡Contáctame por WhatsApp!</h1>
        <p class="subtitle">Haz clic en el botón o escanea el código QR</p>
        <a href="https://wa.me/525610094722" class="whatsapp-btn" target="_blank" rel="noopener">
            <svg width="24" height="24" viewBox="0 0 24 24" fill="currentColor"><path d="M17.472 14.382c-.297-.149-1.758-.867-2.03-.967-.273-.099-.471-.148-.67.15-.197.297-.767.966-.94 1.164-.173.199-.347.223-.644.075-.297-.15-1.255-.463-2.39-1.475-.883-.788-1.48-1.761-1.653-2.059-.173-.297-.018-.458.13-.606.134-.133.298-.347.446-.52.149-.174.198-.298.298-.497.099-.198.05-.371-.025-.52-.075-.149-.669-1.612-.916-2.207-.242-.579-.487-.5-.669-.51-.173-.008-.371-.01-.57-.01-.198 0-.52.074-.792.372-.272.297-1.04 1.016-1.04 2.479 0 1.462 1.065 2.875 1.213 3.074.149.198 2.096 3.2 5.077 4.487.709.306 1.262.489 1.694.625.712.227 1.36.195 1.871.118.571-.085 1.758-.719 2.006-1.413.248-.694.248-1.289.173-1.413-.074-.124-.272-.198-.57-.347m-5.421 7.403h-.004a9.87 9.87 0 01-5.031-1.378l-.361-.214-3.741.982.998-3.648-.235-.374a9.86 9.86 0 01-1.51-5.26c.001-5.45 4.436-9.884 9.888-9.884 2.64 0 5.122 1.03 6.988 2.898a9.825 9.825 0 012.893 6.994c-.003 5.45-4.437 9.884-9.885 9.884m8.413-18.297A11.815 11.815 0 0012.05 0C5.495 0 .16 5.335.157 11.892c0 2.096.547 4.142 1.588 5.945L.057 24l6.305-1.654a11.882 11.882 0 005.683 1.448h.005c6.554 0 11.890-5.335 11.893-11.893A11.821 11.821 0 0020.893 3.506"/></svg>
            Abrir WhatsApp
        </a>
        <div class="phone-number">📱 +52 56 1009 4722</div>
        <div class="qr-section">
            <h3 class="qr-title">O escanea este código QR</h3>
            <canvas id="qr-code"></canvas>
            <div class="instructions">
                <strong>Instrucciones:</strong><br>
                1. Abre la cámara de tu celular<br>
                2. Apunta al código QR<br>
                3. Toca el enlace que aparece<br>
                4. ¡Listo para chatear!
            </div>
        </div>
    </div>
    <script>
        window.addEventListener('load', function() {
            const qr = new QRious({
                element: document.getElementById('qr-code'),
                value: 'https://wa.me/525610094722',
                size: 200,
                foreground: '#075E54',
                background: '#ffffff',
                level: 'M'
            });
        });
    </script>
</body>
</html>
