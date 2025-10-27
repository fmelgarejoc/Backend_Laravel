# Lab Laravel - Backend Application

## **Información del Proyecto**
- **Desarrollado por:** Fabio Melgarejo Cardozo
- **Tecnologías:** Laravel (Backend)

## **Descripción del Proyecto**
Esta aplicación demuestra la integración entre un frontend desarrollado en Angular y un backend construido con Laravel. 

## **Backend - Laravel**
### **Configuración realizada:**
- **Archivo de rutas:** `api.php`
- **Controlador:** `ProductoController`
- **Métodos implementados:**

### **Rutas configuradas en `routes/api.php`:**
```php
<?php

use App\Http\Controllers\ProductoController;
use Illuminate\Http\Request;
use Illuminate\Support\Facades\Route;

Route::get('/productos', [ProductoController::class, 'index']);      // GET - Obtener todos los productos
Route::post('/productos', [ProductoController::class, 'store']);     // POST - Crear nuevo producto