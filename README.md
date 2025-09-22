# Arquitectura-de-software-Serverless

# Colocar esto en el Powershell para ingresar datos a las bases de datos 
$body = @{
  "reporteId" = "3001"
  "nombre"    = "Fernando"
  "correo"    = ""
  "telefono"  = "3214567890"        # sin acento
  "categoria" = "Base de datos"     # sin acento
  "mensaje"   = "La base de datos presenta intermitencia"
  "prioridad" = "Alta"
} | ConvertTo-Json -Depth 5 -Compress

Invoke-RestMethod `
  -Uri "https://gryl0gxiw3.execute-api.us-east-2.amazonaws.com/prod/reportes" `
  -Method POST `
  -ContentType "application/json" `
  -Body $body

# Bases de Datos
  
  <img width="1918" height="876" alt="image" src="https://github.com/user-attachments/assets/7fd4f59a-f560-43c7-9b1f-ca98c1770a2b" />

<img width="1917" height="875" alt="image" src="https://github.com/user-attachments/assets/3e336448-2ada-4e63-ad67-87bdaa112520" />

