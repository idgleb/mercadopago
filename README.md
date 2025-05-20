# Mercado Pago QR 💳

**🌐 Integración con la API de Mercado Pago para pagos QR en puntos de venta.**

## ✨ Descripción

**Mercado Pago QR** es un proyecto Java que permite crear órdenes de pago mediante códigos QR usando la API de Mercado Pago. Ideal para comercios que buscan implementar pagos digitales rápidos y seguros.

---

## 🚀 Características

- 🧾 Genera órdenes QR con detalles de ítems y montos.
- 🔗 Notificaciones webhook para actualizaciones de pago.
- 🔒 Autenticación segura con token Bearer.

---

## 🛠️ Requisitos

- ☕ Java 8+
- 🔑 Token de Mercado Pago
- 🧰 IDE (IntelliJ IDEA, Android Studio, etc.)

---

## ⚙️ Instalación

1. **Clona el repositorio** 📥:
   ```bash
   git clone https://github.com/idgleb/mercadopago.git
   ```

2. **Configura credenciales** 🔑:
   - Añade tu token en un archivo `.env`:
     ```properties
     MERCADO_PAGO_TOKEN=APP_USR-7885482239406684-083115-...
     ```

3. **Ejecuta** 🚀:
   - Abre en tu IDE y compila.
   - Usa un servidor local o emulador Android.

---

## 📖 Uso

1. Configura una orden POST:
   ```json
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
   ```

2. Envía a:
   ```
   POST https://api.mercadopago.com/instore/orders/qr/seller/collectors/{SELLER_ID}/pos/{POS_ID}/qrs
   ```

3. Muestra el código QR 🖼️.

---

## 🧑‍💻 Tecnologías

- ☕ Java
- 🌐 API Mercado Pago
- 📡 OkHttp (recomendado)

---

## 🤝 Contribuir

1. Fork 🍴.
2. Crea una rama (`git checkout -b feature/nueva-funcionalidad`) 🌿.
3. Commitea (`git commit -m "Añadir funcionalidad"`) ✅.
4. Push (`git push origin feature/nueva-funcionalidad`) 🚀.
5. Abre un Pull Request 📬.

---

## 📜 Licencia

Licencia **[MIT](LICENSE)** 📝.

---

## 📬 Contacto

- 🐞 Issues: [GitHub](https://github.com/idgleb/mercadopago/issues)
- ✉️ Email: idgleb@example.com

---

🌟 **¡Simplifica pagos con Mercado Pago QR!** 🌟
