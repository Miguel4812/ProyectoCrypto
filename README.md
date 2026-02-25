# CryptoPro ??

**CryptoPro** es una aplicación web moderna desarrollada con **Angular** que permite a los usuarios consultar el estado del mercado de criptomonedas en tiempo real. Utiliza la API pública de **CoinGecko** para obtener precios, gráficos históricos y detalles financieros, todo presentado con una interfaz limpia y responsiva diseñada con **Bootstrap 5**.

---

## ?? Características Principales

*   **?? Dashboard Principal**: Visualización destacada de las criptomonedas más importantes mediante un carrusel interactivo.
*   **?? Listado Completo**: Tabla dinámica con las 100 principales criptomonedas, mostrando precio actual, capitalización de mercado y variación en 24h (con indicadores visuales de colores).
*   **?? Búsqueda en Tiempo Real**: Funcionalidad de búsqueda integrada en la barra de navegación para filtrar criptomonedas instantáneamente.
*   **?? Detalles y Gráficos**: Página de detalle para cada moneda con:
    *   Información financiera profunda (Volumen, Ranking, Oferta).
    *   Gráficos interactivos de historial de precios (últimos 30 días) usando **Chart.js**.
*   **?? Diseño Responsivo**: Adaptado perfectamente a móviles, tablets y escritorio gracias al sistema de grid de Bootstrap.
*   **?? Formulario de Contacto**: Sección funcional para consultas.

---

## ??? Tecnologías Utilizadas

Este proyecto demuestra el uso de tecnologías punteras en el ecosistema Frontend:

*   **Framework**: [Angular](https://angular.io/) (v21)
    *   Uso de **Signals** para la gestión reactiva del estado.
    *   **Componentes Standalone**.
    *   **Servicios** con inyección de dependencias (`HttpClient`).
    *   **Routing** para la navegación SPA (Single Page Application).
*   **Lenguaje**: [TypeScript](https://www.typescriptlang.org/)
*   **Estilos**: [Bootstrap 5](https://getbootstrap.com/)
*   **Gráficos**: [Chart.js](https://www.chartjs.org/) y [ng2-charts](https://valor-software.com/ng2-charts/)
*   **API Externa**: [CoinGecko API](https://www.coingecko.com/en/api)

---

## ?? Estructura del Proyecto

El código está organizado siguiendo las mejores prácticas de arquitectura en Angular:

```text
src/app/
+-- components/
¦   +-- home/           # Página de aterrizaje con carrusel destacado
¦   +-- crypto-list/    # Tabla principal de criptomonedas
¦   +-- crypto-detail/  # Vista detallada con gráficos
¦   +-- contact/        # Formulario de contacto
¦   +-- navbar/         # Barra de navegación con buscador global
¦   +-- footer/         # Pie de página
+-- services/
¦   +-- crypto.ts       # Lógica de comunicación con la API y gestión de estado
+-- app.routes.ts       # Configuración de rutas
```

### Puntos Destacados del Código

*   **Servicios y Signals**: El servicio `CryptoService` maneja la comunicación HTTP y utiliza Signals para compartir el estado de búsqueda entre el Navbar y la Lista de Criptos.
*   **Manejo de Errores**: Implementación de `catchError` en las peticiones HTTP para gestionar fallos de red o de la API elegantemente.
*   **Optimización**: Uso de `HttpParams` para consultas seguras y eficientes.

---

## ?? Instalación y Ejecución

Si deseas correr este proyecto en tu entorno local, sigue estos pasos:

1.  **Clonar el repositorio**:
    ```bash
    git clone https://github.com/Miguel4812/ProyectoCrypto.git
    cd ProyectoCrypto/crypto-pro
    ```

2.  **Instalar dependencias**:
    Asegúrate de tener Node.js instalado.
    ```bash
    npm install
    ```

3.  **Ejecutar el servidor de desarrollo**:
    ```bash
    ng serve
    ```

4.  **Abrir en el navegador**:
    Navega a `http://localhost:4200/`. La aplicación se recargará automáticamente si cambias algún archivo fuente.

---

## ?? Licencia

Este proyecto es para fines educativos y demostrativos.

---

<p align="center">
  <sub>Desarrollado con ?? por Miguel</sub>
</p>
