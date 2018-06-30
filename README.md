# 04.SQL-VBA
Aplicación de un ETL desarrollado con SQL y VBA en Excel

## INDICACIONES

### 1. Descargar la macro Aplicación_V1.xlsm y el archivo TXT input BALANCE_LIMA_MN_20180101.txt.

### 2. Editar la ruta donde se encuentre el archivo TXT input.
En la macro, la ruta se encuentra en el módulo Extraccion.

![img](https://github.com/JesusAVV/04.SQL-VBA/blob/master/ETL%20Application%20SQL-VBA.jpg)

### 3. En la base de datos, crear las tablas dbo.BALANCE_VBA y dbo.INDICADORES_VBA

```
CREATE TABLE dbo.BALANCE_VBA
([FECHA PROCESO] varchar(8) NULL,
CUENTA varchar(20) NULL,
DESCRIPCION varchar(30) NULL,
[SALDO INICIAL] decimal(28,2) NULL,
CARGO decimal(28,2) NULL,
ABONO decimal(28,2) NULL,
[SALDO FINAL] decimal(28,2) NULL
)

CREATE TABLE dbo.INDICADORES_VBA
([FECHA PROCESO] varchar(8) NULL,
INDICADOR varchar(100) NULL,
RESULTADO decimal(28,2) NULL
)
```

### 4. Ejecutar la macro según el orden de los botones.
