# 🧪 ASP.NET Core Empty Setup Guide

This guide will walk you through setting up a minimal **ASP.NET Core Empty** project using Visual Studio 2022 and .NET 8/9.

---

## ✅ Prerequisites

- ✅ Visual Studio 2022 installed
- ✅ .NET 8.0 or .NET 9.0 SDK installed

---

## 🛠️ Setup Instructions

### 1. Open Visual Studio 2022  
📷 ![Step 1](images/step1.png)

---

### 2. Create a new project  
📷 ![Step 2](images/step2.png)

- Click on **"Create a new project"**

---

### 3. Select "ASP.NET Core Empty"  
📷 ![Step 3](images/step3.png)

- Search for **"ASP.NET Core Empty"**
- Select it and click **Next**

---

### 4. Select .NET 8.0 or 9.0  
📷 ![Step 4](images/step4.png)

- Choose either **.NET 8.0** or **.NET 9.0** as the framework
- Click **Create**

---

### 5. Go to `Program.cs`  
📷 ![Step 5](images/step5.png)

- Open the `Program.cs` file from the **Solution Explorer**

---

### 6. Replace with this code  
📷 ![Step 6](images/step6.png)

```csharp
var builder = WebApplication.CreateBuilder(args);
var app = builder.Build();

app.MapGet("/", () => "Hello, World!");

app.Run();
