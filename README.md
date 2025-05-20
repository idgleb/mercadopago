Mercado Pago QR 💳


🌐 Integración con la API de Mercado Pago para pagos QR en puntos de venta.

✨ Descripción

Mercado Pago QR es un proyecto Java que permite crear órdenes de pago mediante códigos QR usando la API de Mercado Pago. Ideal para comercios que buscan implementar pagos digitales rápidos y seguros.



🚀 Características





🧾 Genera órdenes QR con detalles de ítems y montos.



🔗 Notificaciones webhook para actualizaciones de pago.



🔒 Autenticación segura con token Bearer.



🛠️ Requisitos





☕ Java 8+



🔑 Token de Mercado Pago



🧰 IDE (IntelliJ IDEA, Android Studio, etc.)



⚙️ Instalación





Clona el repositorio 📥:

git clone https://github.com/idgleb/mercadopago.git



Configura credenciales 🔑:





Añade tu token en un archivo .env:

MERCADO_PAGO_TOKEN=APP_USR-7885482239406684-083115-...



Ejecuta 🚀:





Abre en tu IDE y compila.



Usa un servidor local o emulador Android.



📖 Uso





Configura una orden POST:

{
  "items": [
    {
      "sku_number": "A123K9191938",
      "title": "Point Mini",
      "unit_price": 15,
      "quantity": 1,
      "total_amount": 15
    }
  ],
  "total_amount": 15,
  "notification_url": "https://www.cualquersitio.com/",
  "external_reference": "random123"
}



Envía a:

POST https://api.mercadopago.com/instore/orders/qr/seller/collectors/{SELLER_ID}/pos/{POS_ID}/qrs



Muestra el código QR 🖼️.



🧑‍💻 Tecnologías





☕ Java



🌐 API Mercado Pago



📡 OkHttp (recomendado)



🤝 Contribuir





Fork 🍴.



Crea una rama (git checkout -b feature/nueva-funcionalidad) 🌿.



Commitea (git commit -m "Añadir funcionalidad") ✅.



Push (git push origin feature/nueva-funcionalidad) 🚀.



Abre un Pull Request 📬.



📜 Licencia

Licencia MIT 📝.



📬 Contacto





🐞 Issues: GitHub



✉️ Email: idgleb@example.com



🌟 ¡Simplifica pagos con Mercado Pago QR! 🌟
