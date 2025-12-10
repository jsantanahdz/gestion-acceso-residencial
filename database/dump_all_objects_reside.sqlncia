-- MySQL dump 10.13  Distrib 8.0.44, for Win64 (x86_64)
--
-- Host: localhost    Database: residencia
-- ------------------------------------------------------
-- Server version	8.0.44

/*!40101 SET @OLD_CHARACTER_SET_CLIENT=@@CHARACTER_SET_CLIENT */;
/*!40101 SET @OLD_CHARACTER_SET_RESULTS=@@CHARACTER_SET_RESULTS */;
/*!40101 SET @OLD_COLLATION_CONNECTION=@@COLLATION_CONNECTION */;
/*!50503 SET NAMES utf8 */;
/*!40103 SET @OLD_TIME_ZONE=@@TIME_ZONE */;
/*!40103 SET TIME_ZONE='+00:00' */;
/*!40014 SET @OLD_UNIQUE_CHECKS=@@UNIQUE_CHECKS, UNIQUE_CHECKS=0 */;
/*!40014 SET @OLD_FOREIGN_KEY_CHECKS=@@FOREIGN_KEY_CHECKS, FOREIGN_KEY_CHECKS=0 */;
/*!40101 SET @OLD_SQL_MODE=@@SQL_MODE, SQL_MODE='NO_AUTO_VALUE_ON_ZERO' */;
/*!40111 SET @OLD_SQL_NOTES=@@SQL_NOTES, SQL_NOTES=0 */;

--
-- Table structure for table `comunicado`
--

DROP TABLE IF EXISTS `comunicado`;
/*!40101 SET @saved_cs_client     = @@character_set_client */;
/*!50503 SET character_set_client = utf8mb4 */;
CREATE TABLE `comunicado` (
  `id_comunicado` int NOT NULL AUTO_INCREMENT,
  `id_fraccionamiento` int DEFAULT NULL,
  `titulo` varchar(150) DEFAULT NULL,
  `comentarios` varchar(500) DEFAULT NULL,
  `fecha_registro` datetime DEFAULT NULL,
  PRIMARY KEY (`id_comunicado`),
  KEY `fk_comunicado_residencia_idx` (`id_fraccionamiento`),
  CONSTRAINT `fk_comunicado_fraccionamiento` FOREIGN KEY (`id_fraccionamiento`) REFERENCES `fraccionamiento` (`id_fraccionamiento`) ON DELETE CASCADE ON UPDATE CASCADE
) ENGINE=InnoDB AUTO_INCREMENT=26 DEFAULT CHARSET=utf8mb4 COLLATE=utf8mb4_0900_ai_ci;
/*!40101 SET character_set_client = @saved_cs_client */;

--
-- Dumping data for table `comunicado`
--

LOCK TABLES `comunicado` WRITE;
/*!40000 ALTER TABLE `comunicado` DISABLE KEYS */;
INSERT INTO `comunicado` VALUES (1,1,'Horario Festivo: Día de Reyes','La administración operará con horario reducido de 10:00 a 14:00 el día 6 de enero. Favor de tomar precauciones.','2025-01-02 10:30:00'),(2,1,'Aviso de Mantenimiento Preventivo','Se realizará mantenimiento a la bomba de agua el día 15 de enero. Podría haber baja presión entre 9:00 y 11:00 hrs.','2025-01-10 14:00:00'),(3,1,'Cambio de Ruta de Recolección de Basura','Por obras en la calle principal, la recolección de residuos se adelantará 1 hora a partir de mañana. Esté atento.','2025-02-05 08:45:00'),(4,1,'Ingreso de Proveedor - Bonafont','El servicio de reparto de agua Bonafont ingresará el jueves 20 de febrero. Se le pide facilitar el acceso a la unidad.','2025-02-18 17:00:00'),(5,1,'Perro Perdido: \"Max\"','Se busca perro raza Beagle, llamado \"Max\", visto por última vez cerca del área de juegos. Si lo ve, comuníquese con caseta. ¡Gracias!','2025-03-01 11:20:00'),(6,1,'Reunión Vecinal Extraordinaria','Convocatoria a reunión el sábado 22 de marzo a las 18:00 hrs para discutir el tema de seguridad perimetral.','2025-03-15 09:10:00'),(7,1,'Día de Asueto Administrativo','La oficina de administración permanecerá cerrada el lunes 7 de abril por día de asueto del personal.','2025-04-03 15:30:00'),(8,1,'Fumigación de Áreas Comunes','El día 18 de abril se realizará la fumigación contra mosquitos en jardines y parque. Mantener mascotas alejadas.','2025-04-14 12:00:00'),(9,1,'Servicio de Gas LP - Acceso','El camión de Gas LP entrará al fraccionamiento el martes 6 de mayo en el horario habitual.','2025-05-02 07:50:00'),(10,1,'Entrega de Paquetería Especial (COCA-COLA)','Se espera el ingreso de unidades de reparto de Coca-Cola el 15 de mayo para abastecer eventos. Favor de no obstruir vías.','2025-05-13 16:30:00'),(11,1,'Restricción de Horario de Construcción','Debido a quejas vecinales, se recuerda que los trabajos de construcción solo están permitidos de 8:00 a 18:00 hrs.','2025-05-28 13:15:00'),(12,1,'Actualización de Código de Acceso','Se ha actualizado el código de acceso peatonal temporal. El nuevo código será enviado por correo a los residentes.','2025-06-05 10:00:00'),(13,1,'Aviso de Corte de Luz Programado','CFE notificó un corte programado para el día 25 de junio de 13:00 a 16:00. Tome medidas con equipos electrónicos.','2025-06-20 17:45:00'),(14,1,'Prohibición de Fuegos Pirotécnicos','Se recuerda la prohibición estricta de usar pirotecnia dentro de las instalaciones del fraccionamiento por seguridad.','2025-07-01 11:00:00'),(15,1,'Ingreso de Proveedores de Internet (TotalPlay)','Personal técnico de TotalPlay ingresará el día 10 de julio para atender solicitudes pendientes.','2025-07-07 08:30:00'),(16,1,'Gato Extraviado: \"Pecas\"','Se perdió gato siamés con collar azul, llamado \"Pecas\", en la sección 3. Recompensa ofrecida por su localización.','2025-07-25 14:00:00'),(17,1,'Mantenimiento a la Alberca','La alberca estará fuera de servicio del 5 al 7 de agosto por limpieza profunda y cambio de químicos.','2025-08-01 16:00:00'),(18,1,'Cierre Temporal de Gimnasio','El gimnasio estará cerrado el viernes 15 de agosto para instalación de nuevo equipo de cardio.','2025-08-12 09:30:00'),(19,1,'Servicio de Recolección de Basura: Regularizado','Se informa a los vecinos que el servicio de recolección regresa a su horario y ruta normal a partir de mañana.','2025-09-02 12:45:00'),(20,1,'Falla en el Sistema de Acceso','Por una falla eléctrica, el acceso vehicular con TAG podría no funcionar temporalmente. El guardia realizará el acceso manual.','2025-09-20 18:00:00'),(21,1,'Preparación para Lluvias: Limpieza de Drenaje','Pedimos a los residentes no tirar basura en las coladeras, se está realizando la limpieza de drenajes para prevenir inundaciones.','2025-10-05 10:40:00'),(22,1,'Restricciones por Halloween / Día de Muertos','El día 31 de octubre y 2 de noviembre, la caseta estará más atenta al acceso de grupos grandes. Favor de avisar sus visitas.','2025-10-28 15:00:00'),(23,1,'Aviso de Cobro de Cuotas Pendientes','Se recuerda a los residentes con cuotas pendientes que tienen hasta el 15 de noviembre para regularizarse y evitar recargos.','2025-11-01 07:00:00'),(24,1,'Vacante en el Comité de Vigilancia','Se abre la convocatoria para ocupar un puesto en el Comité de Vigilancia. Interesados enviar correo a la administración.','2025-11-20 14:20:00'),(25,1,'Instalación de Decoraciones Navideñas','El personal de mantenimiento comenzará la instalación de luces y adornos navideños en las áreas comunes el día 1 de diciembre.','2025-12-01 11:30:00');
/*!40000 ALTER TABLE `comunicado` ENABLE KEYS */;
UNLOCK TABLES;

--
-- Table structure for table `estatus_pago`
--

DROP TABLE IF EXISTS `estatus_pago`;
/*!40101 SET @saved_cs_client     = @@character_set_client */;
/*!50503 SET character_set_client = utf8mb4 */;
CREATE TABLE `estatus_pago` (
  `id_estatus_pago` int NOT NULL AUTO_INCREMENT,
  `nombre` varchar(50) NOT NULL,
  PRIMARY KEY (`id_estatus_pago`)
) ENGINE=InnoDB AUTO_INCREMENT=4 DEFAULT CHARSET=utf8mb4 COLLATE=utf8mb4_0900_ai_ci;
/*!40101 SET character_set_client = @saved_cs_client */;

--
-- Dumping data for table `estatus_pago`
--

LOCK TABLES `estatus_pago` WRITE;
/*!40000 ALTER TABLE `estatus_pago` DISABLE KEYS */;
INSERT INTO `estatus_pago` VALUES (1,'Pendiente'),(2,'Por Aprobar'),(3,'Aporbado');
/*!40000 ALTER TABLE `estatus_pago` ENABLE KEYS */;
UNLOCK TABLES;

--
-- Table structure for table `fraccionamiento`
--

DROP TABLE IF EXISTS `fraccionamiento`;
/*!40101 SET @saved_cs_client     = @@character_set_client */;
/*!50503 SET character_set_client = utf8mb4 */;
CREATE TABLE `fraccionamiento` (
  `id_fraccionamiento` int NOT NULL AUTO_INCREMENT,
  `nombre` varchar(50) NOT NULL,
  `fecha_creacion` datetime DEFAULT NULL,
  PRIMARY KEY (`id_fraccionamiento`)
) ENGINE=InnoDB AUTO_INCREMENT=2 DEFAULT CHARSET=utf8mb4 COLLATE=utf8mb4_0900_ai_ci;
/*!40101 SET character_set_client = @saved_cs_client */;

--
-- Dumping data for table `fraccionamiento`
--

LOCK TABLES `fraccionamiento` WRITE;
/*!40000 ALTER TABLE `fraccionamiento` DISABLE KEYS */;
INSERT INTO `fraccionamiento` VALUES (1,'BARCELONA','2025-01-01 00:00:00');
/*!40000 ALTER TABLE `fraccionamiento` ENABLE KEYS */;
UNLOCK TABLES;

--
-- Table structure for table `guardia`
--

DROP TABLE IF EXISTS `guardia`;
/*!40101 SET @saved_cs_client     = @@character_set_client */;
/*!50503 SET character_set_client = utf8mb4 */;
CREATE TABLE `guardia` (
  `id_guardia` int NOT NULL AUTO_INCREMENT,
  `id_persona` int DEFAULT NULL,
  `id_fraccionamiento` int DEFAULT NULL,
  `numero_gafete` varchar(50) DEFAULT NULL,
  `turno` varchar(50) DEFAULT NULL,
  PRIMARY KEY (`id_guardia`),
  KEY `fk_guardia_persona_idx` (`id_persona`),
  KEY `fk_guardia_residencia_idx` (`id_fraccionamiento`),
  CONSTRAINT `fk_guardia_fraccionamiento` FOREIGN KEY (`id_fraccionamiento`) REFERENCES `fraccionamiento` (`id_fraccionamiento`) ON DELETE CASCADE ON UPDATE CASCADE,
  CONSTRAINT `fk_guardia_persona` FOREIGN KEY (`id_persona`) REFERENCES `persona` (`id_persona`) ON DELETE CASCADE ON UPDATE CASCADE
) ENGINE=InnoDB AUTO_INCREMENT=10 DEFAULT CHARSET=utf8mb4 COLLATE=utf8mb4_0900_ai_ci;
/*!40101 SET character_set_client = @saved_cs_client */;

--
-- Dumping data for table `guardia`
--

LOCK TABLES `guardia` WRITE;
/*!40000 ALTER TABLE `guardia` DISABLE KEYS */;
INSERT INTO `guardia` VALUES (1,11,1,'ABC123','Matutino'),(2,12,1,'DFG123','Matutino'),(3,13,1,'GLJ212','Matutino'),(4,14,1,'KHY365','Vespertino'),(5,15,1,'KIE987','Vespertino'),(6,16,1,'UEW983','Vespertino'),(7,17,1,'PQS932','Nocturno'),(8,18,1,'PQM773','Nocturno'),(9,19,1,'OQS831','Nocturno');
/*!40000 ALTER TABLE `guardia` ENABLE KEYS */;
UNLOCK TABLES;

--
-- Temporary view structure for view `historial_visitas`
--

DROP TABLE IF EXISTS `historial_visitas`;
/*!50001 DROP VIEW IF EXISTS `historial_visitas`*/;
SET @saved_cs_client     = @@character_set_client;
/*!50503 SET character_set_client = utf8mb4 */;
/*!50001 CREATE VIEW `historial_visitas` AS SELECT 
 1 AS `nombre_fraccionamiento`,
 1 AS `nombre_residencia`,
 1 AS `motivo_visita`,
 1 AS `nombre`,
 1 AS `placa_vehiculo`,
 1 AS `fecha_hora_entrada`,
 1 AS `fecha_hora_salida`,
 1 AS `codigo_qr`*/;
SET character_set_client = @saved_cs_client;

--
-- Temporary view structure for view `listado_residentes`
--

DROP TABLE IF EXISTS `listado_residentes`;
/*!50001 DROP VIEW IF EXISTS `listado_residentes`*/;
SET @saved_cs_client     = @@character_set_client;
/*!50503 SET character_set_client = utf8mb4 */;
/*!50001 CREATE VIEW `listado_residentes` AS SELECT 
 1 AS `nombre_usuario`,
 1 AS `nombre`,
 1 AS `apellido_paterno`,
 1 AS `apellido_materno`,
 1 AS `calle`,
 1 AS `numero`,
 1 AS `colonia`,
 1 AS `fecha_registro`,
 1 AS `activo`*/;
SET character_set_client = @saved_cs_client;

--
-- Table structure for table `motivo_visita`
--

DROP TABLE IF EXISTS `motivo_visita`;
/*!40101 SET @saved_cs_client     = @@character_set_client */;
/*!50503 SET character_set_client = utf8mb4 */;
CREATE TABLE `motivo_visita` (
  `id_motivo_visita` int NOT NULL AUTO_INCREMENT,
  `nombre` varchar(100) NOT NULL,
  PRIMARY KEY (`id_motivo_visita`)
) ENGINE=InnoDB AUTO_INCREMENT=6 DEFAULT CHARSET=utf8mb4 COLLATE=utf8mb4_0900_ai_ci;
/*!40101 SET character_set_client = @saved_cs_client */;

--
-- Dumping data for table `motivo_visita`
--

LOCK TABLES `motivo_visita` WRITE;
/*!40000 ALTER TABLE `motivo_visita` DISABLE KEYS */;
INSERT INTO `motivo_visita` VALUES (1,'Proveedor'),(2,'Paquetería'),(3,'Servicio domicilio'),(4,'Invitado'),(5,'Familiar');
/*!40000 ALTER TABLE `motivo_visita` ENABLE KEYS */;
UNLOCK TABLES;

--
-- Table structure for table `pago`
--

DROP TABLE IF EXISTS `pago`;
/*!40101 SET @saved_cs_client     = @@character_set_client */;
/*!50503 SET character_set_client = utf8mb4 */;
CREATE TABLE `pago` (
  `id_pago` int NOT NULL AUTO_INCREMENT,
  `id_usuario` int DEFAULT NULL,
  `id_fraccionamiento` int DEFAULT NULL,
  `id_residencia` int DEFAULT NULL,
  `id_estatus_pago` int DEFAULT NULL,
  `referencia` varchar(50) DEFAULT NULL,
  `fecha_pago` datetime DEFAULT NULL,
  `monto` decimal(10,2) DEFAULT NULL,
  `comprobante` varchar(250) DEFAULT NULL,
  PRIMARY KEY (`id_pago`),
  KEY `fk_pago_id_usuario_idx` (`id_usuario`),
  KEY `fk_pago_id_residencia_idx` (`id_fraccionamiento`),
  KEY `fk_pago_estatus_pago_idx` (`id_estatus_pago`),
  KEY `fk_pago_residencia_idx` (`id_residencia`),
  CONSTRAINT `fk_pago_estatus_pago` FOREIGN KEY (`id_estatus_pago`) REFERENCES `estatus_pago` (`id_estatus_pago`) ON DELETE CASCADE ON UPDATE CASCADE,
  CONSTRAINT `fk_pago_id_fraccionamiento` FOREIGN KEY (`id_fraccionamiento`) REFERENCES `fraccionamiento` (`id_fraccionamiento`) ON DELETE CASCADE ON UPDATE CASCADE,
  CONSTRAINT `fk_pago_id_usuario` FOREIGN KEY (`id_usuario`) REFERENCES `usuario` (`id_usuario`) ON DELETE CASCADE ON UPDATE CASCADE,
  CONSTRAINT `fk_pago_residencia` FOREIGN KEY (`id_residencia`) REFERENCES `residencia` (`id_residencia`)
) ENGINE=InnoDB AUTO_INCREMENT=51 DEFAULT CHARSET=utf8mb4 COLLATE=utf8mb4_0900_ai_ci;
/*!40101 SET character_set_client = @saved_cs_client */;

--
-- Dumping data for table `pago`
--

LOCK TABLES `pago` WRITE;
/*!40000 ALTER TABLE `pago` DISABLE KEYS */;
INSERT INTO `pago` VALUES (1,2,1,1,3,'102345','2025-01-05 00:00:00',500.00,'d:comprobanteIMG_012345.jpg'),(2,3,1,2,3,'203456','2025-01-05 00:00:00',500.00,'d:comprobanteIMG_023456.jpg'),(3,4,1,3,3,'304567','2025-01-05 00:00:00',500.00,'d:comprobanteIMG_034567.jpg'),(4,5,1,4,3,'405678','2025-01-05 00:00:00',500.00,'d:comprobanteIMG_045678.jpg'),(5,6,1,5,3,'506789','2025-01-05 00:00:00',500.00,'d:comprobanteIMG_056789.jpg'),(6,7,1,6,3,'607890','2025-01-05 00:00:00',500.00,'d:comprobanteIMG_067890.jpg'),(7,2,1,1,1,NULL,NULL,NULL,NULL),(8,3,1,2,3,'809012','2025-02-05 00:00:00',500.00,'d:comprobanteIMG_089012.jpg'),(9,4,1,3,3,'901234','2025-02-05 00:00:00',500.00,'d:comprobanteIMG_090123.jpg'),(10,5,1,4,2,'112345','2025-02-05 00:00:00',500.00,'d:comprobanteIMG_101234.jpg'),(11,6,1,5,3,'223456','2025-02-05 00:00:00',500.00,'d:comprobanteIMG_112345.jpg'),(12,7,1,6,3,'334567','2025-02-05 00:00:00',500.00,'d:comprobanteIMG_123456.jpg'),(13,2,1,1,3,'445678','2025-03-05 00:00:00',500.00,'d:comprobanteIMG_134567.jpg'),(14,3,1,2,3,'556789','2025-03-05 00:00:00',500.00,'d:comprobanteIMG_145678.jpg'),(15,4,1,3,1,NULL,NULL,NULL,NULL),(16,5,1,4,3,'778901','2025-03-05 00:00:00',500.00,'d:comprobanteIMG_167890.jpg'),(17,6,1,5,3,'889012','2025-03-05 00:00:00',500.00,'d:comprobanteIMG_178901.jpg'),(18,7,1,6,3,'990123','2025-03-05 00:00:00',500.00,'d:comprobanteIMG_189012.jpg'),(19,2,1,1,3,'121234','2025-04-05 00:00:00',500.00,'d:comprobanteIMG_190123.jpg'),(20,3,1,2,3,'232345','2025-04-05 00:00:00',500.00,'d:comprobanteIMG_201234.jpg'),(21,4,1,3,3,'343456','2025-04-05 00:00:00',500.00,'d:comprobanteIMG_212345.jpg'),(22,5,1,4,3,'454567','2025-04-05 00:00:00',500.00,'d:comprobanteIMG_223456.jpg'),(23,6,1,5,3,'565678','2025-04-05 00:00:00',500.00,'d:comprobanteIMG_234567.jpg'),(24,7,1,6,3,'676789','2025-04-05 00:00:00',500.00,'d:comprobanteIMG_245678.jpg'),(25,2,1,1,3,'787890','2025-05-05 00:00:00',500.00,'d:comprobanteIMG_256789.jpg'),(26,3,1,2,2,'898901','2025-05-05 00:00:00',500.00,'d:comprobanteIMG_267890.jpg'),(27,4,1,3,3,'909012','2025-05-05 00:00:00',500.00,'d:comprobanteIMG_278901.jpg'),(28,5,1,4,3,'131345','2025-05-05 00:00:00',500.00,'d:comprobanteIMG_289012.jpg'),(29,6,1,5,3,'242456','2025-05-05 00:00:00',500.00,'d:comprobanteIMG_290123.jpg'),(30,7,1,6,3,'353567','2025-05-05 00:00:00',500.00,'d:comprobanteIMG_301234.jpg'),(31,2,1,1,3,'464678','2025-06-05 00:00:00',500.00,'d:comprobanteIMG_312345.jpg'),(32,3,1,2,3,'575789','2025-06-05 00:00:00',500.00,'d:comprobanteIMG_323456.jpg'),(33,4,1,3,2,'686890','2025-06-05 00:00:00',500.00,'d:comprobanteIMG_334567.jpg'),(34,5,1,4,3,'797901','2025-06-05 00:00:00',500.00,'d:comprobanteIMG_345678.jpg'),(35,6,1,5,3,'808012','2025-06-05 00:00:00',500.00,'d:comprobanteIMG_356789.jpg'),(36,7,1,6,3,'919123','2025-06-05 00:00:00',500.00,'d:comprobanteIMG_367890.jpg'),(37,2,1,1,3,'141456','2025-07-05 00:00:00',500.00,'d:comprobanteIMG_378901.jpg'),(38,3,1,2,3,'252567','2025-07-05 00:00:00',500.00,'d:comprobanteIMG_389012.jpg'),(39,4,1,3,3,'363678','2025-07-05 00:00:00',500.00,'d:comprobanteIMG_390123.jpg'),(40,5,1,4,3,'474789','2025-07-05 00:00:00',500.00,'d:comprobanteIMG_401234.jpg'),(41,6,1,5,2,'585890','2025-07-05 00:00:00',500.00,'d:comprobanteIMG_412345.jpg'),(42,7,1,6,3,'696901','2025-07-05 00:00:00',500.00,'d:comprobanteIMG_423456.jpg'),(43,2,1,1,1,NULL,NULL,NULL,NULL),(44,3,1,2,1,NULL,NULL,NULL,NULL),(45,4,1,3,3,'929234','2025-08-05 00:00:00',500.00,'d:comprobanteIMG_456789.jpg'),(46,5,1,4,3,'151567','2025-08-05 00:00:00',500.00,'d:comprobanteIMG_467890.jpg'),(47,6,1,5,2,'262678','2025-08-05 00:00:00',500.00,'d:comprobanteIMG_478901.jpg'),(48,7,1,6,3,'373789','2025-08-05 00:00:00',500.00,'d:comprobanteIMG_489012.jpg'),(49,2,1,1,2,'484890','2025-09-05 00:00:00',500.00,'d:comprobanteIMG_490123.jpg'),(50,3,1,2,3,'595901','2025-09-05 00:00:00',500.00,'d:comprobanteIMG_501234.jpg');
/*!40000 ALTER TABLE `pago` ENABLE KEYS */;
UNLOCK TABLES;

--
-- Table structure for table `persona`
--

DROP TABLE IF EXISTS `persona`;
/*!40101 SET @saved_cs_client     = @@character_set_client */;
/*!50503 SET character_set_client = utf8mb4 */;
CREATE TABLE `persona` (
  `id_persona` int NOT NULL AUTO_INCREMENT,
  `nombre` varchar(100) NOT NULL,
  `apellido_paterno` varchar(100) DEFAULT NULL,
  `apellido_materno` varchar(100) DEFAULT NULL,
  `calle` varchar(100) DEFAULT NULL,
  `numero` int DEFAULT NULL,
  `colonia` varchar(100) DEFAULT NULL,
  `telefono` varchar(20) DEFAULT NULL,
  `celular` varchar(20) DEFAULT NULL,
  `email` varchar(150) DEFAULT NULL,
  `activo` tinyint DEFAULT NULL,
  `fecha_registro` datetime DEFAULT NULL,
  PRIMARY KEY (`id_persona`)
) ENGINE=InnoDB AUTO_INCREMENT=51 DEFAULT CHARSET=utf8mb4 COLLATE=utf8mb4_0900_ai_ci;
/*!40101 SET character_set_client = @saved_cs_client */;

--
-- Dumping data for table `persona`
--

LOCK TABLES `persona` WRITE;
/*!40000 ALTER TABLE `persona` DISABLE KEYS */;
INSERT INTO `persona` VALUES (1,'Alejandro','García','López','Avenida Principal',105,'Privada Barcelona','8112345678','8180000001','alejandro.g@mail.com',1,'2025-09-26 00:00:00'),(2,'Sofía','Martínez','Ramírez','Avenida Principal',21,'Privada Barcelona','5512345678','5580000002','sofia.m@mail.com',1,'2025-09-23 00:00:00'),(3,'Roberto','Hernández','Díaz','Avenida Principal',45,'Privada Barcelona','3312345678','3380000003','roberto.h@mail.com',1,'2025-07-07 00:00:00'),(4,'Mariana','Pérez','Sánchez','Avenida Principal',300,'Privada Barcelona','9912345678','9980000004','mariana.p@mail.com',1,'2025-05-19 00:00:00'),(5,'Carlos','González','Flores','Avenida Principal',12,'Privada Barcelona','2212345678','2280000005','carlos.g@mail.com',1,'2025-05-11 00:00:00'),(6,'Laura','Rodríguez','Torres','Avenida Principal',88,'Privada Barcelona','4412345678','4480000006','laura.r@mail.com',1,'2025-08-24 00:00:00'),(7,'Fernando','Vázquez','Ruiz','Avenida Principal',7,'Privada Barcelona','8112345679','8180000007','fernando.v@mail.com',1,'2025-04-22 00:00:00'),(8,'Andrea','Cruz','Mendoza','Avenida Principal',1500,'Privada Barcelona','5512345679','5580000008','andrea.c@mail.com',1,'2025-07-07 00:00:00'),(9,'Daniel','Morales','Castro','Avenida Principal',90,'Privada Barcelona','3312345679','3380000009','daniel.m@mail.com',1,'2025-09-26 00:00:00'),(10,'Gabriela','Jiménez','Ortega','Avenida Principal',33,'Privada Barcelona','9912345679','9980000010','gabriela.j@mail.com',1,'2025-04-17 00:00:00'),(11,'Javier','Reyes','Guerrero','Avenida Principal',101,'Privada Barcelona','2212345679','2280000011','javier.r@mail.com',1,'2025-03-03 00:00:00'),(12,'Valeria','Silva','Méndez','Avenida Principal',200,'Privada Barcelona','4412345679','4480000012','valeria.s@mail.com',1,'2025-11-22 00:00:00'),(13,'Héctor','Vega','Lozano','Avenida Principal',60,'Privada Barcelona','8112345680','8180000013','hector.v@mail.com',1,'2025-04-08 00:00:00'),(14,'Natalia','Paredes','Herrera','Avenida Principal',55,'Privada Barcelona','5512345680','5580000014','natalia.p@mail.com',1,'2025-07-01 00:00:00'),(15,'Emilio','Soto','Ibarra','Avenida Principal',120,'Privada Barcelona','3312345680','3380000015','emilio.s@mail.com',1,'2025-10-09 00:00:00'),(16,'Regina','Cano','Montes','Calle Cedro',14,'Privada Barcelona','9912345680','9980000016','regina.c@mail.com',1,'2025-07-05 00:00:00'),(17,'Ricardo','Blanco','Salas','Calle Cedro',25,'Privada Barcelona','2212345680','2280000017','ricardo.b@mail.com',1,'2025-03-27 00:00:00'),(18,'Samantha','Ferrer','Vidal','Calle Cedro',707,'Privada Barcelona','4412345680','4480000018','samantha.f@mail.com',1,'2025-07-27 00:00:00'),(19,'Guillermo','Luna','Peña','Calle Cedro',99,'Privada Barcelona','8112345681','8180000019','guillermo.l@mail.com',1,'2025-04-16 00:00:00'),(20,'Paulina','Rivas','Galván','Calle Cedro',1,'Privada Barcelona','5512345681','5580000020','paulina.r@mail.com',1,'2025-08-31 00:00:00'),(21,'Manuel','Acosta','Vargas','Calle Cedro',350,'Privada Barcelona','3312345681','3380000021','manuel.a@mail.com',1,'2025-08-09 00:00:00'),(22,'Elisa','Ochoa','Navarro','Calle Cedro',2,'Privada Barcelona','9912345681','9980000022','elisa.o@mail.com',1,'2025-02-09 00:00:00'),(23,'Jorge','Salazar','Chávez','Calle Cedro',10,'Privada Barcelona','2212345681','2280000023','jorge.s@mail.com',1,'2025-07-28 00:00:00'),(24,'Diana','Ibarra','Lara','Calle Cedro',500,'Privada Barcelona','4412345681','4480000024','diana.i@mail.com',1,'2025-09-08 00:00:00'),(25,'Miguel','Zamora','Sosa','Calle Cedro',1,'Privada Barcelona','8112345682','8180000025','miguel.z@mail.com',1,'2025-10-18 00:00:00'),(26,'Rosa','Téllez','Pardo','Calle Cedro',110,'Privada Barcelona','5512345682','5580000026','rosa.t@mail.com',1,'2025-01-27 00:00:00'),(27,'Alfredo','Cisneros','Zúñiga','Calle Cedro',55,'Privada Barcelona','3312345682','3380000027','alfredo.c@mail.com',1,'2025-09-30 00:00:00'),(28,'Luisa','Molina','Brito','Calle Cedro',30,'Privada Barcelona','9912345682','9980000028','luisa.m@mail.com',1,'2025-09-30 00:00:00'),(29,'Felipe','Duarte','Herrera','Calle Cedro',222,'Privada Barcelona','2212345682','2280000029','felipe.d@mail.com',1,'2025-07-25 00:00:00'),(30,'Silvia','Núñez','Vera','Calle Olivo',1,'Privada Barcelona','4412345682','4480000030','silvia.n@mail.com',1,'2025-07-31 00:00:00'),(31,'Roberto','Méndez','Castillo','Calle Olivo',45,'Privada Barcelona','8112345690','8180000031','roberto.m@mail.com',1,'2025-04-14 00:00:00'),(32,'Lucía','Fernández','Romero','Calle Olivo',102,'Privada Barcelona','8112345691','8180000032','lucia.f@mail.com',1,'2025-08-07 00:00:00'),(33,'Fernando','Torres','Gil','Calle Olivo',88,'Privada Barcelona','8112345692','8180000033','fernando.t@mail.com',1,'2025-04-19 00:00:00'),(34,'Gabriela','Vargas','Ortiz','Calle Olivo',230,'Privada Barcelona','8112345693','8180000034','gabriela.v@mail.com',1,'2025-08-15 00:00:00'),(35,'Hugo','Reyes','Navarro','Calle Olivo',12,'Privada Barcelona','8112345694','8180000035','hugo.r@mail.com',1,'2025-05-11 00:00:00'),(36,'Mariana','Cruz','Mendoza','Calle Olivo',56,'Privada Barcelona','8112345695','8180000036','mariana.c@mail.com',1,'2025-11-08 00:00:00'),(37,'Alejandro','Silva','Ramos','Calle Olivo',404,'Privada Barcelona','8112345696','8180000037','alejandro.s@mail.com',1,'2025-06-05 00:00:00'),(38,'Verónica','Guzmán','Flores','Calle Olivo',77,'Privada Barcelona','8112345697','8180000038','veronica.g@mail.com',1,'2025-06-30 00:00:00'),(39,'Daniel','Ortega','Delgado','Calle Olivo',19,'Privada Barcelona','8112345698','8180000039','daniel.o@mail.com',1,'2025-04-09 00:00:00'),(40,'Patricia','Rios','Sandoval','Calle Alamo',300,'Privada Barcelona','8112345699','8180000040','patricia.r@mail.com',1,'2025-10-14 00:00:00'),(41,'Eduardo','Morales','Guerrero','Calle Alamo',5,'Privada Barcelona','8112345700','8180000041','eduardo.m@mail.com',1,'2025-05-06 00:00:00'),(42,'Isabel','Herrera','Cano','Calle Alamo',63,'Privada Barcelona','8112345701','8180000042','isabel.h@mail.com',1,'2025-04-16 00:00:00'),(43,'Sergio','Aguilar','Pacheco','Calle Alamo',150,'Privada Barcelona','8112345702','8180000043','sergio.a@mail.com',1,'2025-05-31 00:00:00'),(44,'Lorena','Medina','Vega','Calle Alamo',28,'Privada Barcelona','8112345703','8180000044','lorena.m@mail.com',1,'2025-04-12 00:00:00'),(45,'Francisco','León','Serrano','Calle Alamo',91,'Privada Barcelona','8112345704','8180000045','francisco.l@mail.com',1,'2025-02-25 00:00:00'),(46,'Claudia','Cervantes','Solares','Calle Alamo',210,'Privada Barcelona','8112345705','8180000046','claudia.c@mail.com',1,'2025-11-06 00:00:00'),(47,'Arturo','Salinas','Fuentes','Calle Alamo',500,'Privada Barcelona','8112345706','8180000047','arturo.s@mail.com',1,'2025-02-04 00:00:00'),(48,'Mónica','Pena','Rosales','Calle Alamo',33,'Privada Barcelona','8112345707','8180000048','monica.p@mail.com',1,'2025-09-11 00:00:00'),(49,'Javier','Duran','Esquivel','Calle Alamo',115,'Privada Barcelona','8112345708','8180000049','javier.d@mail.com',1,'2025-06-01 00:00:00'),(50,'Beatriz','Carrillo','Montoya','Calle Alamo',8,'Privada Barcelona','8112345709','8180000050','beatriz.c@mail.com',1,'2025-01-01 00:00:00');
/*!40000 ALTER TABLE `persona` ENABLE KEYS */;
UNLOCK TABLES;

--
-- Table structure for table `reservacion`
--

DROP TABLE IF EXISTS `reservacion`;
/*!40101 SET @saved_cs_client     = @@character_set_client */;
/*!50503 SET character_set_client = utf8mb4 */;
CREATE TABLE `reservacion` (
  `id_reservacion` int NOT NULL AUTO_INCREMENT,
  `id_usuario` int DEFAULT NULL,
  `id_fraccionamiento` int DEFAULT NULL,
  `fecha_inicio` datetime DEFAULT NULL,
  `fecha_final` datetime DEFAULT NULL,
  `nota` varchar(250) DEFAULT NULL,
  `numero_invitados` int DEFAULT NULL,
  PRIMARY KEY (`id_reservacion`),
  KEY `fk_reservacion_usuario_idx` (`id_usuario`),
  KEY `fk_reservacion_residencia_idx` (`id_fraccionamiento`),
  CONSTRAINT `fk_reservacion_fraccionamiento` FOREIGN KEY (`id_fraccionamiento`) REFERENCES `fraccionamiento` (`id_fraccionamiento`) ON DELETE CASCADE ON UPDATE CASCADE,
  CONSTRAINT `fk_reservacion_usuario` FOREIGN KEY (`id_usuario`) REFERENCES `usuario` (`id_usuario`) ON DELETE CASCADE ON UPDATE CASCADE
) ENGINE=InnoDB AUTO_INCREMENT=31 DEFAULT CHARSET=utf8mb4 COLLATE=utf8mb4_0900_ai_ci;
/*!40101 SET character_set_client = @saved_cs_client */;

--
-- Dumping data for table `reservacion`
--

LOCK TABLES `reservacion` WRITE;
/*!40000 ALTER TABLE `reservacion` DISABLE KEYS */;
INSERT INTO `reservacion` VALUES (1,2,1,'2025-01-01 10:00:00','2025-01-01 13:00:00','Reserva para área común de piscina.',5),(2,3,1,'2025-01-02 15:00:00','2025-01-02 18:00:00','Cumpleaños de niño en salón principal.',15),(3,4,1,'2025-01-03 08:00:00','2025-01-03 11:00:00','Reunión de trabajo en sala de juntas.',3),(4,5,1,'2025-01-04 19:00:00','2025-01-04 22:00:00','Cena familiar privada.',8),(5,6,1,'2025-01-05 11:00:00','2025-01-05 14:00:00','Clase de yoga en el gimnasio.',10),(6,7,1,'2025-01-06 16:00:00','2025-01-06 19:00:00','Uso de asadores para parrillada.',6),(7,2,1,'2025-01-07 13:00:00','2025-01-07 16:00:00','Reserva de cancha de tenis.',4),(8,3,1,'2025-01-08 09:00:00','2025-01-08 12:00:00','Mantenimiento preventivo en sala.',2),(9,4,1,'2025-01-09 17:00:00','2025-01-09 20:00:00','Reunión de vecinos.',20),(10,5,1,'2025-01-10 14:00:00','2025-01-10 17:00:00','Fiesta infantil.',18),(11,6,1,'2025-01-11 10:00:00','2025-01-11 13:00:00','Reserva de salón pequeño.',7),(12,7,1,'2025-01-12 15:00:00','2025-01-12 18:00:00','Torneo de videojuegos.',12),(13,2,1,'2025-01-13 12:00:00','2025-01-13 15:00:00','Reserva de área de juegos.',9),(14,3,1,'2025-01-14 18:00:00','2025-01-14 21:00:00','Pool party con amigos.',15),(15,4,1,'2025-01-15 09:00:00','2025-01-15 12:00:00','Clase de natación.',5),(16,5,1,'2025-01-16 16:00:00','2025-01-16 19:00:00','Asamblea de condominio.',30),(17,6,1,'2025-01-17 11:00:00','2025-01-17 14:00:00','Evento deportivo.',10),(18,7,1,'2025-01-18 14:00:00','2025-01-18 17:00:00','Reunión informal.',4),(19,2,1,'2025-01-19 10:00:00','2025-01-19 13:00:00','Reserva de sala de cine.',6),(20,3,1,'2025-01-20 19:00:00','2025-01-20 22:00:00','Noche de juegos de mesa.',8),(21,4,1,'2025-01-21 08:00:00','2025-01-21 11:00:00','Taller de manualidades.',5),(22,5,1,'2025-01-22 15:00:00','2025-01-22 18:00:00','Sesión de fotos.',3),(23,6,1,'2025-01-23 12:00:00','2025-01-23 15:00:00','Clase de cocina.',10),(24,7,1,'2025-01-24 17:00:00','2025-01-24 20:00:00','Evento de networking.',25),(25,2,1,'2025-01-25 11:00:00','2025-01-25 14:00:00','Reserva de sauna.',2),(26,3,1,'2025-01-26 16:00:00','2025-01-26 19:00:00','Despedida de soltera.',12),(27,4,1,'2025-01-27 13:00:00','2025-01-27 16:00:00','Reunión de padres.',15),(28,5,1,'2025-01-28 10:00:00','2025-01-28 13:00:00','Brunch corporativo.',20),(29,6,1,'2025-01-29 18:00:00','2025-01-29 21:00:00','Cata de vinos.',7),(30,7,1,'2025-01-30 14:00:00','2025-01-30 17:00:00','Reserva para lectura en terraza.',3);
/*!40000 ALTER TABLE `reservacion` ENABLE KEYS */;
UNLOCK TABLES;

--
-- Table structure for table `residencia`
--

DROP TABLE IF EXISTS `residencia`;
/*!40101 SET @saved_cs_client     = @@character_set_client */;
/*!50503 SET character_set_client = utf8mb4 */;
CREATE TABLE `residencia` (
  `id_residencia` int NOT NULL AUTO_INCREMENT,
  `id_fraccionamiento` int DEFAULT NULL,
  `nombre` varchar(200) DEFAULT NULL,
  `fecha_registro` datetime DEFAULT NULL,
  PRIMARY KEY (`id_residencia`),
  KEY `fk_residencia_fraccionamiento_idx` (`id_fraccionamiento`),
  CONSTRAINT `fk_residencia_fraccionamiento` FOREIGN KEY (`id_fraccionamiento`) REFERENCES `fraccionamiento` (`id_fraccionamiento`) ON DELETE CASCADE ON UPDATE CASCADE
) ENGINE=InnoDB AUTO_INCREMENT=32 DEFAULT CHARSET=utf8mb4 COLLATE=utf8mb4_0900_ai_ci;
/*!40101 SET character_set_client = @saved_cs_client */;

--
-- Dumping data for table `residencia`
--

LOCK TABLES `residencia` WRITE;
/*!40000 ALTER TABLE `residencia` DISABLE KEYS */;
INSERT INTO `residencia` VALUES (1,1,'Avenida Principal 21','2025-09-23 00:00:00'),(2,1,'Avenida Principal 12','2025-05-11 00:00:00'),(3,1,'Avenida Principal 45','2025-07-07 00:00:00'),(4,1,'Avenida Principal 300','2025-05-19 00:00:00'),(5,1,'Avenida Principal 88','2025-08-24 00:00:00'),(6,1,'Avenida Principal 7','2025-04-22 00:00:00'),(7,1,'Avenida Principal 1500','2025-07-07 00:00:00'),(8,1,'Avenida Principal 90','2025-09-26 00:00:00'),(9,1,'Avenida Principal 33','2025-04-17 00:00:00'),(10,1,'Calle Cedro 1','2025-08-31 00:00:00'),(11,1,'Calle Cedro 350','2025-08-09 00:00:00'),(12,1,'Calle Cedro 2','2025-02-09 00:00:00'),(13,1,'Calle Cedro 10','2025-07-28 00:00:00'),(14,1,'Calle Cedro 500','2025-09-08 00:00:00'),(15,1,'Calle Cedro 1','2025-10-18 00:00:00'),(16,1,'Calle Cedro 110','2025-01-27 00:00:00'),(17,1,'Calle Cedro 55','2025-09-30 00:00:00'),(18,1,'Calle Cedro 30','2025-09-30 00:00:00'),(19,1,'Calle Cedro 222','2025-07-25 00:00:00'),(20,1,'Calle Olivo 1','2025-07-31 00:00:00');
/*!40000 ALTER TABLE `residencia` ENABLE KEYS */;
UNLOCK TABLES;

--
-- Table structure for table `rol_usuario`
--

DROP TABLE IF EXISTS `rol_usuario`;
/*!40101 SET @saved_cs_client     = @@character_set_client */;
/*!50503 SET character_set_client = utf8mb4 */;
CREATE TABLE `rol_usuario` (
  `id_rol_usuario` int NOT NULL AUTO_INCREMENT,
  `nombre` varchar(50) NOT NULL,
  PRIMARY KEY (`id_rol_usuario`)
) ENGINE=InnoDB AUTO_INCREMENT=3 DEFAULT CHARSET=utf8mb4 COLLATE=utf8mb4_0900_ai_ci;
/*!40101 SET character_set_client = @saved_cs_client */;

--
-- Dumping data for table `rol_usuario`
--

LOCK TABLES `rol_usuario` WRITE;
/*!40000 ALTER TABLE `rol_usuario` DISABLE KEYS */;
INSERT INTO `rol_usuario` VALUES (1,'Administrador'),(2,'Residente');
/*!40000 ALTER TABLE `rol_usuario` ENABLE KEYS */;
UNLOCK TABLES;

--
-- Table structure for table `usuario`
--

DROP TABLE IF EXISTS `usuario`;
/*!40101 SET @saved_cs_client     = @@character_set_client */;
/*!50503 SET character_set_client = utf8mb4 */;
CREATE TABLE `usuario` (
  `id_usuario` int NOT NULL AUTO_INCREMENT,
  `id_persona` int NOT NULL,
  `id_fraccionamiento` int NOT NULL,
  `id_residencia` int DEFAULT NULL,
  `id_rol_usuario` int NOT NULL,
  `nombre_usuario` varchar(100) NOT NULL,
  `contraseña` varchar(100) NOT NULL,
  PRIMARY KEY (`id_usuario`),
  KEY `fk_usuario_persona_idx` (`id_persona`),
  KEY `fk_usuario_residencia_idx` (`id_fraccionamiento`),
  KEY `fk_usuario_rol_usuario_idx` (`id_rol_usuario`),
  KEY `fk_usuario_residencia_idx1` (`id_residencia`),
  CONSTRAINT `fk_usuario_fraccionamiento` FOREIGN KEY (`id_fraccionamiento`) REFERENCES `fraccionamiento` (`id_fraccionamiento`) ON DELETE CASCADE ON UPDATE CASCADE,
  CONSTRAINT `fk_usuario_persona` FOREIGN KEY (`id_persona`) REFERENCES `persona` (`id_persona`) ON DELETE CASCADE ON UPDATE CASCADE,
  CONSTRAINT `fk_usuario_residencia` FOREIGN KEY (`id_residencia`) REFERENCES `residencia` (`id_residencia`) ON DELETE CASCADE ON UPDATE CASCADE,
  CONSTRAINT `fk_usuario_rol_usuario` FOREIGN KEY (`id_rol_usuario`) REFERENCES `rol_usuario` (`id_rol_usuario`) ON DELETE CASCADE ON UPDATE CASCADE
) ENGINE=InnoDB AUTO_INCREMENT=22 DEFAULT CHARSET=utf8mb4 COLLATE=utf8mb4_0900_ai_ci;
/*!40101 SET character_set_client = @saved_cs_client */;

--
-- Dumping data for table `usuario`
--

LOCK TABLES `usuario` WRITE;
/*!40000 ALTER TABLE `usuario` DISABLE KEYS */;
INSERT INTO `usuario` VALUES (1,1,1,NULL,1,'ADMON1','12345678'),(2,2,1,1,2,'USR001','12345678'),(3,5,1,2,2,'USR002','12345678'),(4,3,1,3,2,'USR003','12345678'),(5,4,1,4,2,'USR004','12345678'),(6,6,1,5,2,'USR005','12345678'),(7,7,1,6,2,'USR006','12345678'),(8,8,1,7,2,'USR007','12345678'),(9,9,1,8,2,'USR008','12345678'),(10,10,1,9,2,'USR009','12345678'),(11,20,1,10,2,'USR010','12345678'),(12,21,1,11,2,'USR011','12345678'),(13,22,1,12,2,'USR012','12345678'),(14,23,1,13,2,'USR013','12345678'),(15,24,1,14,2,'USR014','12345678'),(16,25,1,15,2,'USR015','12345678'),(17,26,1,16,2,'USR016','12345678'),(18,27,1,17,2,'USR017','12345678'),(19,28,1,18,2,'USR018','12345678'),(20,29,1,19,2,'USR019','12345678'),(21,30,1,20,2,'USR020','12345678');
/*!40000 ALTER TABLE `usuario` ENABLE KEYS */;
UNLOCK TABLES;

--
-- Table structure for table `visita`
--

DROP TABLE IF EXISTS `visita`;
/*!40101 SET @saved_cs_client     = @@character_set_client */;
/*!50503 SET character_set_client = utf8mb4 */;
CREATE TABLE `visita` (
  `id_visita` int NOT NULL AUTO_INCREMENT,
  `id_fraccionamiento` int DEFAULT NULL,
  `id_residencia` int DEFAULT NULL,
  `id_motivo_visita` int DEFAULT NULL,
  `nombre` varchar(250) DEFAULT NULL,
  `identificacion` varchar(50) DEFAULT NULL,
  `placa_vehiculo` varchar(10) DEFAULT NULL,
  `codigo_qr` varchar(255) DEFAULT NULL,
  `fecha_hora_entrada` datetime DEFAULT NULL,
  `fecha_hora_salida` datetime DEFAULT NULL,
  `fecha_registro` datetime DEFAULT NULL,
  PRIMARY KEY (`id_visita`),
  KEY `fk_visita_residencia_idx` (`id_fraccionamiento`),
  KEY `fk_visita_motivo_visita_idx` (`id_motivo_visita`),
  KEY `fk_visita_residencia_idx1` (`id_residencia`),
  CONSTRAINT `fk_visita_fraccionamiento` FOREIGN KEY (`id_fraccionamiento`) REFERENCES `fraccionamiento` (`id_fraccionamiento`) ON DELETE CASCADE ON UPDATE CASCADE,
  CONSTRAINT `fk_visita_motivo_visita` FOREIGN KEY (`id_motivo_visita`) REFERENCES `motivo_visita` (`id_motivo_visita`) ON DELETE CASCADE ON UPDATE CASCADE,
  CONSTRAINT `fk_visita_residencia` FOREIGN KEY (`id_residencia`) REFERENCES `residencia` (`id_residencia`) ON DELETE CASCADE ON UPDATE CASCADE
) ENGINE=InnoDB AUTO_INCREMENT=239 DEFAULT CHARSET=utf8mb4 COLLATE=utf8mb4_0900_ai_ci;
/*!40101 SET character_set_client = @saved_cs_client */;

--
-- Dumping data for table `visita`
--

LOCK TABLES `visita` WRITE;
/*!40000 ALTER TABLE `visita` DISABLE KEYS */;
INSERT INTO `visita` VALUES (1,1,1,1,'Alejandra Ramírez',NULL,'ABC-587','0c0c2d5a00a7d7f861a4a1488fefb0de5ed234fd54d52ee19249835c7eb2e7b7','2025-09-06 09:05:27','2025-09-06 11:58:41','2025-09-06 09:05:20'),(2,1,1,1,'Roberto Gómez',NULL,'ABC-831','dfa4be762567a6bda0756e1be1605a7cd6a163ae0e65d8592c7db608af28b1f6','2025-07-19 20:56:05','2025-07-20 01:42:46','2025-07-19 20:53:14'),(3,1,2,2,'Sofía Vargas',NULL,'ABC-041','1f143692422338970ef35198ffd5c4a786a984b42f19d8087b1847cd015da41b','2025-03-12 12:15:46','2025-03-12 13:23:49','2025-03-12 12:12:47'),(4,1,3,2,'Carlos Mendoza',NULL,'ABC-966','c86ac035695e7d10efa3b2ee8eb28702578958af0856df33b29275f70f7ffe9f','2025-07-13 08:27:07','2025-07-13 12:41:14','2025-07-13 08:24:33'),(5,1,3,5,'Laura Fuentes',NULL,'ABC-833','33e5863f12e15b8d13768b0ecc6c952135878cc3398cd49712cd3feda39fe004','2025-03-30 18:46:36','2025-03-30 19:57:48','2025-03-30 18:44:50'),(6,1,4,3,'Javier Ponce',NULL,'ABC-723','0104fae7105a97d25956eec50ea33cf3e20101011630f80afdb7f4ba581abb8f','2025-04-11 13:49:08','2025-04-11 16:11:57','2025-04-11 13:46:22'),(7,1,4,4,'Elena Ortega',NULL,'ABC-508','6ab031ab0203362efcd0f83db6b50bb82710c3c8b987fbb6862803387c97bd34','2025-07-20 11:58:57','2025-07-20 16:46:48','2025-07-20 11:57:02'),(8,1,5,4,'Miguel Soto',NULL,'ABC-427','dd45af5b38a7f53f5e27038d4721875cd001992c9878a4bd2dcade26b0123876','2025-03-25 08:42:58','2025-03-25 13:17:56','2025-03-25 08:38:55'),(9,1,5,3,'Andrea Díaz',NULL,'ABC-824','45249a832ca2ecc14de28018cdbda999f17c92441e9dcf0df71f79cebdc8bcc6','2025-07-06 12:03:17','2025-07-06 12:41:14','2025-07-06 12:02:36'),(10,1,5,1,'Ricardo Castro',NULL,'ABC-771','ddc5370cc16248153e316b7436b75b0fc1f3af3aff546da93eb78c9b482034d0','2025-07-01 11:50:42','2025-07-01 17:15:07','2025-07-01 11:50:31'),(11,1,6,5,'Valeria Hernández',NULL,'ABC-565','782c5634ad3e1ce48a7d9629ee3b6e58f24ba50b79784322ecb9afec3013ab9f','2025-02-07 14:27:51','2025-02-07 15:42:27','2025-02-07 14:26:29'),(12,1,6,1,'Jorge Lozano',NULL,'ABC-231','da5b1fe2c5032335f10a034bb4df050c5d83c43a333f0a993afc480190798731','2025-10-18 14:49:12','2025-10-18 15:25:09','2025-10-18 14:46:29'),(13,1,7,4,'Mónica Pérez',NULL,'ABC-465','8b6a1109ce5140b0c328c44b53ad342a7885d61a9f64cf3bcce098d7b065e4cd','2025-07-30 14:40:37','2025-07-30 18:32:45','2025-07-30 14:36:10'),(14,1,8,4,'Gabriel Torres',NULL,'ABC-611','fffaab3d3f0cf38c573efe0571d78c446863ffe70b459ff8d5f837fbec082bad','2025-05-15 11:46:10','2025-05-15 14:12:54','2025-05-15 11:45:58'),(15,1,9,3,'Isabel Flores',NULL,'ABC-724','f844140cc3920fe166af9b744ae34deea212443af307fbfd9bf9e3c173b996fa','2025-11-12 16:07:53','2025-11-12 17:46:55','2025-11-12 16:06:07'),(16,1,9,2,'Daniel Ruiz',NULL,'ABC-135','62b36de8e7c235d3857bdaae3eeffbdbbf3658f940222851e503de9464a32ba8','2025-01-06 07:48:59','2025-01-06 09:24:03','2025-01-06 07:44:17'),(17,1,9,3,'Verónica Salazar',NULL,'ABC-331','3a9c360b7f3572f47864dde153eda09ffe7840bd3d9c0119139aedf56db8ac5c','2025-01-13 12:25:04','2025-01-13 16:21:00','2025-01-13 12:22:59'),(18,1,9,4,'Fernando Herrera',NULL,'ABC-730','dd9709c32ea5113996f5090dc931ec4b5a0be1b253413e797d8c043cdc63b112','2025-11-13 14:12:29','2025-11-13 17:34:10','2025-11-13 14:10:06'),(19,1,10,3,'Patricia Morales',NULL,'ABC-686','5243bdf8efe5c39a313de10c58d252d320835cd4ff2405898197e1b76e11b548','2025-07-20 15:36:07','2025-07-20 16:29:47','2025-07-20 15:32:42'),(20,1,10,2,'Luis Silva',NULL,'ABC-649','89559eab3f140bebb7e20be2092feaa425e2e0d1018993db33193cf5dea4a2ec','2025-02-25 18:36:41','2025-02-25 20:58:57','2025-02-25 18:33:45'),(21,1,10,1,'Marcela Quintero',NULL,'ABC-065','b8dfbcea76632093ea7d5152f586058c34d22739eabbeef467263560a183aa8b','2025-09-14 07:57:38','2025-09-14 08:38:29','2025-09-14 07:52:41'),(22,1,11,2,'Esteban Vidal',NULL,'ABC-266','a68180b36cadb8d6ac65b3d114b776738bba73ee88dc7d2ceb1285846e26224c','2025-10-13 11:00:48','2025-10-13 15:24:26','2025-10-13 10:59:57'),(23,1,1,5,'Adriana Guerrero',NULL,'ABC-009','5daa127ba52f2ed5a42e70a579bf804c60d2610a45e3bbb65b8479947edd44ff','2025-05-19 15:45:32','2025-05-19 19:37:51','2025-05-19 15:42:08'),(24,1,1,4,'Cristian Peña',NULL,'ABC-208','6cf1bf676f186a94de6f9709f1802baadf89867814bf2dc1830b335d8aa0d454','2025-04-22 16:14:23','2025-04-22 17:11:13','2025-04-22 16:11:19'),(25,1,1,3,'Jimena Rojas',NULL,'ABC-373','fbf403590954d079f45674de82bd50c284a82251a743a8193265c6df5d233e9a','2025-09-14 21:49:56','2025-09-15 01:34:07','2025-09-14 21:48:16'),(26,1,11,2,'Héctor Bravo',NULL,'ABC-628','a20d6162f02298dbeb4318a90b6329faee72a53e4cd47e7dbda437777f1fa93a','2025-08-07 11:04:54','2025-08-07 13:36:38','2025-08-07 11:03:37'),(27,1,11,1,'Diana Núñez',NULL,'ABC-090','ffb29dfd19064e5b08a6e009a68d389e3f8d43324da07011573118eb22673354','2025-12-03 10:39:56','2025-12-03 12:17:57','2025-12-03 10:37:48'),(28,1,12,1,'Oscar León',NULL,'ABC-536','58e4d7f5f14d472a7c7bba88d8626098b671fa21f26dc5bd515966e5fe42f1f2','2025-05-18 18:40:49','2025-05-18 22:28:35','2025-05-18 18:40:40'),(29,1,12,4,'Karla Rivas',NULL,'ABC-419','770c39d9075c45d971102b315193e9849069651a49196a9ce89f799fe4d3b623','2025-01-24 11:25:23','2025-01-24 13:14:40','2025-01-24 11:23:03'),(30,1,12,1,'Mario Sánchez',NULL,'ABC-674','fe9d4d8371b1c1cdf205ae9b91b28a2338bdc23b52c628a239aa48b58e44a143','2025-06-15 08:04:51','2025-06-15 12:57:31','2025-06-15 08:03:37'),(31,1,12,3,'Silvia Gil',NULL,'ABC-527','5e97227268a8f30c7246d4ac2495d86d189b4695d74c79cb4c90fdd33315f4b2','2025-06-21 19:28:22','2025-06-21 23:05:28','2025-06-21 19:24:58'),(32,1,12,2,'Andrés Osorio',NULL,'ABC-796','d181b703ea0d00400296db9018896cd2526436df29a3aeefacb3f9b2f1376163','2025-06-12 12:38:01','2025-06-12 15:16:09','2025-06-12 12:37:43'),(33,1,13,1,'Paula Durán',NULL,'ABC-476','7d3cd4f955c9d9c14dccf3055f51292272b1c880f91d727b6bb5bf7208524c41','2025-11-07 14:07:16','2025-11-07 17:36:35','2025-11-07 14:04:10'),(34,1,13,2,'Felipe Nieto',NULL,'ABC-848','b6b6a6b598229c932a80f7c70a8304d73a27f4768e169cc269f749d824cddbd6','2025-03-26 13:12:33','2025-03-26 15:15:15','2025-03-26 13:10:51'),(35,1,13,4,'Giselle Moya',NULL,'ABC-297','b90fab4795891868ed3ddd9846fb3cabc275e492b3890695b2d111c1e73197ad','2025-08-26 15:00:37','2025-08-26 18:14:50','2025-08-26 14:59:39'),(36,1,13,2,'Diego Pardo',NULL,'ABC-433','e673f66727748bb68dc3afbd85ef81ffc682d6086014414cab0a354b62e85c58','2025-03-21 16:38:01','2025-03-21 19:35:17','2025-03-21 16:35:09'),(37,1,13,4,'Sara Cárdenas',NULL,'ABC-697','422128b78f36005f73c211f44612634ab93278f6cc835a0614d04b4258da768d','2025-04-28 07:33:13','2025-04-28 08:43:49','2025-04-28 07:30:18'),(38,1,13,3,'Enrique Barrios',NULL,'ABC-106','000982b1c665d2ddd525ee80a374992f41039eb131cd35f2847974d89d3bfe02','2025-06-10 16:38:05','2025-06-10 21:00:06','2025-06-10 16:37:59'),(39,1,13,3,'Natalia Uribe',NULL,'ABC-899','c5e0d0132775dee7e711efeb6b665d17c6b56afa0b15ca3ff54586271de10b1c','2025-08-14 11:55:42','2025-08-14 15:33:07','2025-08-14 11:54:41'),(40,1,15,1,'Renato Guzmán',NULL,'ABC-039','d5782991db6c94c4cd67467e5e8b11bf37478fccc22aafae1ee7239f47a42912','2025-01-17 17:02:38','2025-01-17 18:32:25','2025-01-17 17:02:32'),(41,1,15,2,'Lina Acuña',NULL,'ABC-886','d6b28a83168c1f09ff53ab66c9edcc4d5f9f4bd0c2f4d41590cb791ca545cdc3','2025-05-20 07:55:05','2025-05-20 08:43:05','2025-05-20 07:54:25'),(42,1,14,2,'Sebastián Blanco',NULL,'ABC-687','f4cf4ed3a33691978fb72435803d8177687603931bbc9c4d9d0a0c1a54f6e213','2025-05-24 18:22:56','2025-05-24 21:26:20','2025-05-24 18:21:16'),(43,1,14,1,'Vanessa Cortés',NULL,'ABC-425','8d4cd2d4e90cb9753ae5e18bc3c50122d4cc499c3e8083fded416901ac5d4edb','2025-01-20 11:48:17','2025-01-20 14:24:11','2025-01-20 11:47:21'),(44,1,14,4,'Iván Morales',NULL,'ABC-642','50a7c994d832b545306e2052a04245598d9369a4c5347880d34f72e4b75e8976','2025-07-17 13:05:54','2025-07-17 14:57:41','2025-07-17 13:05:00'),(45,1,15,5,'Claudia Navarro',NULL,'ABC-895','a510e0cfed5079be3ad9eebdc46cf37d99c26c6af3ce7af59103953aabaee16f','2025-01-01 14:37:38','2025-01-01 17:46:07','2025-01-01 14:36:46'),(46,1,16,2,'Mauro Quiroga',NULL,'ABC-424','478c72f3577b57a535ae68aca1092f0b392e39e777913c23154315021109ad60','2025-03-06 14:10:37','2025-03-06 18:41:18','2025-03-06 14:07:23'),(47,1,16,4,'Belén Ríos',NULL,'ABC-273','8328123a2105c4bb9a95137e92a66197183656120a7671ee80e80d370ef25e87','2025-09-18 20:57:32','2025-09-18 23:06:27','2025-09-18 20:53:06'),(48,1,16,2,'Fabián Torres',NULL,'ABC-269','bca48a24b0b4a320dba98dd07284b5fa6c36f0f488dafd38979e9ca8779319eb','2025-05-22 13:35:29','2025-05-22 18:42:56','2025-05-22 13:33:31'),(49,1,1,1,'Daniela Vega',NULL,'ABC-884','6c18c6a2e83b9394f63cb85d997035aa7d4600c79090467e27006cc23fe0ba70','2025-02-03 12:12:18','2025-02-03 14:50:39','2025-02-03 12:11:34'),(50,1,1,1,'Benjamín Zuluaga',NULL,'ABC-809','b8300556b8cbcc7e48ac0d1fbb3dd96bcc93ac2b5594f81c9624af30abf9c19f','2025-05-04 13:27:29','2025-05-04 14:12:57','2025-05-04 13:22:38'),(51,1,15,3,'Viviana Peña',NULL,'ABC-045','2d59bc69fef2fdc3d01df8f8c8230037080be605256679f8b260233ee84e4faf','2025-08-23 15:30:00','2025-08-23 19:40:09','2025-08-23 15:29:46'),(52,1,15,1,'Camilo Marín',NULL,'ABC-473','b13c7e84902b92c2b4def405cc6e491ef7edd272d3e2e285876a463bb28c8d79','2025-11-06 14:26:11','2025-11-06 18:30:01','2025-11-06 14:25:26'),(53,1,15,1,'Jessica Rojas',NULL,'ABC-450','0abed813c431df94deb7fd187e31b206404befbd4973da11dff6e9ee467c2398','2025-06-22 09:11:34','2025-06-22 10:39:26','2025-06-22 09:08:50'),(54,1,15,2,'Arturo Pinto',NULL,'ABC-073','9acdd7ba10fdc7e860f6772a0c3e78c43f0a863b7fdcff81147deab6c1f5815d','2025-02-11 21:49:43','2025-02-12 01:08:54','2025-02-11 21:45:12'),(55,1,15,5,'Ximena Salas',NULL,'ABC-478','849f0307839d9467cb7f9bb2b696a2b9282a47cc34b455aa57e065ecefcef838','2025-09-24 10:37:12','2025-09-24 15:14:29','2025-09-24 10:34:50'),(56,1,15,1,'Eugenio Solano',NULL,'ABC-885','b0217ed23c471d014b9602df7f6d2e76912be3b31479dc930d688b4585ff58e8','2025-10-04 17:36:54','2025-10-04 18:28:18','2025-10-04 17:35:39'),(57,1,3,1,'Gabriela Landa',NULL,'ABC-682','0188958b170a6fc4406a0cf95cad591994d225728e1951fd3efe7fdbeebd83f2','2025-11-27 09:47:38','2025-11-27 15:09:06','2025-11-27 09:45:41'),(58,1,3,1,'Nicolás Bravo',NULL,'ABC-314','98e209594bcba5fc62f42b6f67ee5f08077865cfd055c3e8e943ef9611f9180e','2025-11-14 15:33:09','2025-11-14 16:09:42','2025-11-14 15:31:06'),(59,1,3,1,'Sandra Melo',NULL,'ABC-101','5b34f7f862b38ed930a788f0150069629c96da96a835748caa2474d700a12e96','2025-11-12 14:12:17','2025-11-12 17:37:01','2025-11-12 14:09:39'),(60,1,5,1,'Raúl Rueda',NULL,'ABC-532','3a42ba42f7aaa323d9783c7fca5f29155b2b18899185dfda20f22dc38cec2c22','2025-10-06 15:32:05','2025-10-06 17:50:10','2025-10-06 15:31:24'),(61,1,5,2,'Angélica Paz',NULL,'ABC-563','18731b92d0c0161e479d6f31b6b6776db676b0fbf5c816904374a399908fcf42','2025-06-27 10:50:18','2025-06-27 14:47:02','2025-06-27 10:46:36'),(62,1,5,4,'Juan Valencia',NULL,'ABC-818','cf9111923e92cbff21724bfa4c34618af8037a694cdf517a1df922f1a5bd7010','2025-07-15 17:18:49','2025-07-15 21:15:18','2025-07-15 17:16:36'),(63,1,18,5,'Teresa Ochoa',NULL,'ABC-494','2cfb396ac5d880869e11e43d711f1c8dbea14346b1bc096a31050fa541e1cfde','2025-01-29 08:42:46','2025-01-29 10:45:57','2025-01-29 08:41:32'),(64,1,18,1,'Manuel Londoño',NULL,'ABC-189','d0a375c9cfaaea331055f9d0baac371b807b1b8a8efebc9d529b32b5c6edd90e','2025-03-21 14:05:35','2025-03-21 17:48:35','2025-03-21 14:01:19'),(65,1,18,3,'Rosa Herrera',NULL,'ABC-367','d720aaddf208d8189e9da7a84c9ca556b63d7e028109d646a5f48c4a6489c51f','2025-04-12 21:10:58','2025-04-13 01:44:27','2025-04-12 21:09:28'),(66,1,19,2,'Pablo Vélez',NULL,'ABC-113','b5c97ce249c849133181882a24d131335b30288d1eacc6cfbe0fe5b83ce5dfbe','2025-11-26 07:09:35','2025-11-26 08:16:07','2025-11-26 07:06:37'),(67,1,19,1,'Catalina Cruz',NULL,'ABC-076','9f3f1e52313577bfe5cd594bbc28eb780732bf7ed94505e7b355239d5c33ad03','2025-07-10 07:59:24','2025-07-10 11:36:08','2025-07-10 07:54:34'),(68,1,19,2,'Humberto Díaz',NULL,'ABC-887','43677aa141831884915399fe34c08a4e5e4d11a9f38f6c490e451ca1f8d5e9d5','2025-11-12 18:41:33','2025-11-12 19:37:50','2025-11-12 18:40:57'),(69,1,19,4,'Gloria Sierra',NULL,'ABC-544','e7b918bb4cc0883b27217798dd958160146db1a9bff1688838911a9124743ed6','2025-04-01 07:19:27','2025-04-01 09:18:35','2025-04-01 07:17:11'),(70,1,19,1,'Alfredo Vélez',NULL,'ABC-134','590df2785edb880d6a00c0f8be1813ac811d4f2518db440d9f15c25208bdaf32','2025-04-19 11:09:25','2025-04-19 13:42:22','2025-04-19 11:08:06'),(71,1,19,3,'Luisa Rincón',NULL,'ABC-239','df0310909f674bc49e07aec5847ac5a4a0e907ac90d9e196990009768e53b8e2','2025-01-05 11:34:46','2025-01-05 14:28:54','2025-01-05 11:32:06'),(72,1,19,4,'Adrián Lleras',NULL,'ABC-748','7739bdde83d5924f61abe9a9d01ace821bf00ef951ba8730b9a9f08bf3fe9978','2025-02-27 11:02:01','2025-02-27 15:38:07','2025-02-27 11:00:09'),(73,1,1,2,'Marisol Vega',NULL,'ABC-382','ec90499b0258eba8b40904071c087d2a31203c1cff56c1172eccd66f9e4ce95a','2025-04-18 14:36:14','2025-04-18 17:55:38','2025-04-18 14:34:26'),(74,1,2,3,'Julio Acosta',NULL,'ABC-101','0fcf59cfe5be7471ea2f4e62304d870fdf59cc3a155ece81a7b5ad55838f52d2','2025-01-10 08:26:52','2025-01-10 10:53:04','2025-01-10 08:23:27'),(75,1,3,4,'Violeta Peña',NULL,'ABC-022','c3d4d4aacdaad3adc08253df449a9a4e143c6afba2cf7f09f174384ee37aac61','2025-03-15 07:44:27','2025-03-15 11:09:31','2025-03-15 07:40:21'),(76,1,4,5,'Gustavo Luna',NULL,'ABC-569','e67069bd4b711944a1183d16bde91982b7e184bb7a11ad180a1e07850cc2ff14','2025-04-17 08:49:57','2025-04-17 12:35:28','2025-04-17 08:45:13'),(77,1,7,3,'Lucía Sáenz',NULL,'ABC-012','9f42a7b419be42325aebad70afaecc0124680b841be2d030a29b1cbe19ec4a78','2025-09-10 20:33:06','2025-09-10 22:22:38','2025-09-10 20:29:53'),(78,1,5,2,'Mauricio Reyes',NULL,'ABC-128','3133d751ca52bdf380a442c5efc80b8411bb67440744773400d8bc732ed6bab7','2025-05-09 21:50:21','2025-05-10 02:17:43','2025-05-09 21:50:00'),(79,1,6,3,'Erika Zapata',NULL,'ABC-388','67537a1d34a090b661bd0496b76f5efd4dfe04232263ffb76066d84f26cc1475','2025-10-18 09:12:45','2025-10-18 10:26:50','2025-10-18 09:11:11'),(80,1,6,3,'David Quintero',NULL,'ABC-930','482bf3b6d85d4bc31d8fd977ffaed4eebfdc056d1a65dc9cb2446ab98841fb76','2025-01-26 13:58:51','2025-01-26 14:58:02','2025-01-26 13:58:17'),(81,1,8,1,'Susana Muñoz',NULL,'ABC-981','76064755aea2bee768135fce955dac5dec4039a1729936ea0e8e88339fdc778d','2025-03-07 17:13:45','2025-03-07 21:46:39','2025-03-07 17:13:19'),(82,1,8,2,'Alan Guerrero',NULL,'ABC-483','7bc639475ed664bd142c36b1fae5513585d5c60224d92c4b39ded6bf2bd46d6e','2025-10-26 10:13:31','2025-10-26 12:46:49','2025-10-26 10:11:15'),(83,1,8,5,'Cecilia Torres',NULL,'ABC-290','1692f63cc2a71db1cf80e84e071e8272c36b3a7428a4e754ce9484c34224aa82','2025-11-24 14:46:15','2025-11-24 18:36:27','2025-11-24 14:42:03'),(84,1,8,3,'Fidel Barrios',NULL,'ABC-013','aded67aaccf4b5a565dba2b48efcd9d619a5753d854e20037b9bd690aa54712b','2025-02-23 11:12:21','2025-02-23 16:14:43','2025-02-23 11:08:28'),(85,1,8,3,'Yessica Ruiz',NULL,'ABC-166','a686e25a8c8a495e54327c0bfdc1835f68dece69c457c8c2ce763f96f8356e6d','2025-02-06 10:08:53','2025-02-06 14:13:32','2025-02-06 10:08:46'),(86,1,8,1,'Orlando Osorio',NULL,'ABC-043','87d9feb279cc714dd79220216720867ff9a7215de26c64ec606d5a51c29a9325','2025-10-17 11:07:13','2025-10-17 15:31:12','2025-10-17 11:06:27'),(87,1,10,2,'Nora Salgado',NULL,'ABC-361','703a1ad9b6249e3a55d1d2121f3b05de2ad205cc942e4dc0250e6822026c1f2f','2025-04-22 10:20:32','2025-04-22 11:27:26','2025-04-22 10:15:45'),(88,1,10,2,'Víctor Parra',NULL,'ABC-415','473c5330bee8780e4012690cb3ca053062650ba0f87803bb50b28d7e9f1e3f1c','2025-05-19 09:39:36','2025-05-19 13:23:38','2025-05-19 09:35:48'),(89,1,10,2,'Alba Soto',NULL,'ABC-931','905485224ff106396455275d735566738e5a9ababe03d5b612ea2df3dadc6697','2025-10-01 18:44:08','2025-10-01 21:35:48','2025-10-01 18:43:48'),(90,1,10,1,'Jaime Castro',NULL,'ABC-471','cf4ae9329d56e7ffee222b66ebd98d76e8498d3e33bf75993a30c786a6b2337f','2025-10-07 21:49:45','2025-10-08 00:33:11','2025-10-07 21:48:13'),(91,1,10,1,'Penélope Díaz',NULL,'ABC-792','29865a2e9cbe3b869ca343f222ddeb063c94c99fe40b571c1c747602fe234bb6','2025-02-11 17:52:45','2025-02-11 19:39:01','2025-02-11 17:52:06'),(92,1,10,3,'Ramón Vargas',NULL,'ABC-023','8abc2a28658381f17d7143aab2b6533ffef53105800e7b11779f3124bd27539f','2025-09-30 17:22:58','2025-09-30 18:03:23','2025-09-30 17:22:24'),(93,1,10,1,'Blanca Nieto',NULL,'ABC-694','cd77f9687d6457fa3deda386371f9d162e9c1c0b057f94ab566c59b78321b2d8','2025-05-14 17:06:26','2025-05-14 18:30:51','2025-05-14 17:01:56'),(94,1,11,2,'Héctor Mejía',NULL,'ABC-905','73b193eae7554199274fee364a336bc055ea54ee1fc1cbf4ef3ec079cf92cee7','2025-11-17 07:47:47','2025-11-17 10:19:19','2025-11-17 07:43:17'),(95,1,11,1,'Marina López',NULL,'ABC-189','7e5926561c9f630e781bb008c68b11861c1f8fd9e748e1512ab5c5815b7ccb63','2025-04-01 16:31:28','2025-04-01 18:51:24','2025-04-01 16:26:41'),(96,1,11,4,'Elías Ríos',NULL,'ABC-058','92e672c16dafe546eff58fa5e6da43333bb59222687528041d67f9713c82c535','2025-08-16 14:25:31','2025-08-16 17:09:09','2025-08-16 14:21:36'),(97,1,12,4,'Clara Pérez',NULL,'ABC-112','efff0c1057da225f6701cff7ac9f006ba44315cb0d201df2f96628464da98d4f','2025-07-02 12:27:56','2025-07-02 13:56:43','2025-07-02 12:23:25'),(98,1,12,4,'Guillermo Mora',NULL,'ABC-707','8df4fbad7e1a66e7841e623b68e06406c58745c68f31c82fc05783102f5a15ec','2025-11-06 20:14:51','2025-11-06 23:59:34','2025-11-06 20:11:35'),(99,1,12,1,'Eva Cifuentes',NULL,'ABC-154','d657011e8c2d4730cd331b689b18600fe711e252136f04cdfe4e40ea73928b61','2025-04-03 13:14:18','2025-04-03 15:00:35','2025-04-03 13:14:00'),(100,1,12,2,'Alfonso Solano',NULL,'ABC-308','a1fa89d098eb6458f3f08e41cd6a00318d9840364d0b1c3f426deb1c784a8926','2025-06-01 08:46:33','2025-06-01 10:27:08','2025-06-01 08:42:20'),(101,1,12,3,'Inés Vivas',NULL,'ABC-245','d63756a657f452a927ad433d09b418d868c2e8732d23f9e2179a904dc906e185','2025-06-14 20:47:52','2025-06-14 21:57:06','2025-06-14 20:43:20'),(102,1,1,4,'José Martínez',NULL,'ABC-834','dfb8ce893951ce263727a59bcb940889bd67373ffee0ca5108265a4dc8350c5d','2025-02-13 20:52:26','2025-02-13 22:33:12','2025-02-13 20:50:16'),(103,1,11,1,'Leticia Prada',NULL,'ABC-058','0c5c9e427f289339b2211da984b7586c7dba3d0a87758345e4f7461990fc3cd8','2025-05-16 18:09:11','2025-05-16 21:08:49','2025-05-16 18:07:36'),(104,1,1,4,'Omar Rico',NULL,'ABC-873','f696952361d5454656d386067b546d68048bd2b285f7b6737f8b43a432ad07ab','2025-01-03 08:43:08','2025-01-03 11:56:36','2025-01-03 08:40:58'),(105,1,1,4,'Zaida Bernal',NULL,'ABC-514','c054d67e8e53e528e7a7368d5890ede83efe23a7feac3e1806fd7c55961e315e','2025-06-09 08:10:53','2025-06-09 13:29:27','2025-06-09 08:07:35'),(106,1,15,3,'Pedro Olarte',NULL,'ABC-853','678c64954402bb75250db721ce3ece6cc038b60fb05ebd98ccbb4cb3178b91ef','2025-04-25 18:01:26','2025-04-25 21:44:35','2025-04-25 18:01:01'),(107,1,15,4,'Tatiana Giraldo',NULL,'ABC-283','f6ff61639d58d716eaf122806fb432f7bf4fc96fae823c7d6f611e0975ce4c02','2025-05-09 17:29:33','2025-05-09 19:43:47','2025-05-09 17:26:11'),(108,1,15,4,'Andrés Uribe',NULL,'ABC-233','cea32ab5c5a8310208c87bdfbe919b1d51012add654326280f182f47aaea1465','2025-04-05 13:03:26','2025-04-05 14:24:40','2025-04-05 13:00:08'),(109,1,15,2,'Yolanda Téllez',NULL,'ABC-695','c51464464aa8f30a065ddada7641fd6c3a5fa2327d1448a7b7c47a644445993d','2025-09-15 19:45:33','2025-09-16 00:58:43','2025-09-15 19:44:15'),(110,1,16,4,'Ricardo Ledesma',NULL,'ABC-812','831fc8be3d839f777b1b36c6e70cbe1891c73e6538c0cf7a85cfce8a9d9aefe1','2025-05-02 07:47:33','2025-05-02 09:12:32','2025-05-02 07:43:40'),(111,1,17,3,'Luciana Caro',NULL,'ABC-786','5444872184bcaef414b56bc0879f846155178c8f140c6c25b6117f4985adce80','2025-04-15 10:21:38','2025-04-15 11:48:37','2025-04-15 10:20:07'),(112,1,18,2,'Saúl Montero',NULL,'ABC-836','9d329c7d7475bdc5b56ec53e25d448426a373b0c24ad7135624de35aaf62cf8e','2025-10-27 15:30:36','2025-10-27 16:49:57','2025-10-27 15:29:52'),(113,1,19,4,'Nadia Sierra',NULL,'ABC-885','48bd5c87cf3bc0010fd8ba1d9893038a9a8fd80ea6c8a21758f237d1814b2fc7','2025-02-27 13:45:27','2025-02-27 17:53:45','2025-02-27 13:43:40'),(114,1,20,2,'Marco Tulio Gil',NULL,'ABC-335','250185d57243d8bdad394cbc8fcb257510ac5a6223201d55d74c310ff7cb8d7a','2025-06-26 15:30:43','2025-06-26 17:20:13','2025-06-26 15:27:28'),(115,1,20,4,'Kelly Ospina',NULL,'ABC-356','d594d1d3518ca8d09924fd1bfd2b696a01beb294b2333a8b82a92eb8e57f196b','2025-05-21 09:16:59','2025-05-21 12:16:56','2025-05-21 09:16:29'),(116,1,20,1,'Antonio Rincón',NULL,'ABC-907','896d2bac2dd17b92afaba980b4f259c58824fc2830cfb052a2b95c44b53d9e7f','2025-10-31 10:39:32','2025-10-31 13:43:03','2025-10-31 10:35:11'),(117,1,20,4,'Valeria Parra',NULL,'ABC-824','8f6e9d88752d7093934999529d3c7455f34b2fc2aba9068fa66ec4356e2485c9','2025-09-24 12:06:29','2025-09-24 14:14:22','2025-09-24 12:03:16'),(118,1,6,4,'Iván Camargo',NULL,'ABC-013','a2934d04dbd2be99d24f1e623221a0107448b14e5f42cd7faac68a3b47e970cb','2025-03-06 07:43:50','2025-03-06 11:30:30','2025-03-06 07:42:50'),(119,1,7,3,'Rocío Morales',NULL,'ABC-788','fe2c0a249a8e8c236513e441c0fe37e236e2d3be6a997435cb488e9acb95c674','2025-11-12 08:51:01','2025-11-12 13:18:35','2025-11-12 08:47:43'),(120,1,8,3,'Esteban López',NULL,'ABC-679','6dfd0410c3d50415894d364f02ea9f12e9cdb7418d13ec993072530cd5f50776','2025-10-20 12:28:47','2025-10-20 14:05:18','2025-10-20 12:28:33'),(121,1,8,4,'Luz Marina Díaz',NULL,'ABC-283','3cb46ffcb938999994681e48833e1c35cbf8905cce5da6c577455579a48c091f','2025-06-12 11:42:28','2025-06-12 12:49:02','2025-06-12 11:39:03'),(122,1,8,1,'Fabián Cruz',NULL,'ABC-874','bb15497b147be8995707d011dbfab13804f7332fa07b7fe963a2a1749cd7a2ac','2025-01-07 07:55:27','2025-01-07 09:39:17','2025-01-07 07:55:03'),(123,1,9,3,'Sofía Vargas',NULL,'ABC-854','5b598350d1e79d562d86ea11698ec45d64a497eda2d5d0d14cb8b5a1ec4a528a','2025-07-16 17:42:45','2025-07-16 22:15:17','2025-07-16 17:37:55'),(124,1,10,2,'Jesús Aguirre',NULL,'ABC-550','e18ecd52cb4727388c294301aa7c5c3373fb4012d700d3762784ae1759de41b5','2025-05-07 21:32:55','2025-05-08 01:36:42','2025-05-07 21:29:20'),(125,1,12,3,'Viviana Rojas',NULL,'ABC-403','e7c213c7f9074319a4cdf4835d10f347b78e9b9a3f9f335f6b4c00368a2c6781','2025-05-14 19:32:15','2025-05-15 00:55:03','2025-05-14 19:29:56'),(126,1,1,1,'Hugo Torres',NULL,'ABC-548','de7f6e93b1219ba46ea186090fc0173b26319765d1d73a11fa8e38377724b4ba','2025-04-11 08:54:45','2025-04-11 13:03:30','2025-04-11 08:53:05'),(127,1,12,2,'Daniela Pardo',NULL,'ABC-298','d26c0b28e6b8f71a88a9c562ba6ed504bc072c07669f4a57bd1d1f1409e0a05f','2025-05-16 07:29:05','2025-05-16 12:41:19','2025-05-16 07:25:38'),(128,1,12,1,'Boris Gómez',NULL,'ABC-160','4a86e3326d7e956eafac92025167636a70d87bff7c4f85aca2291a69f1296397','2025-07-10 18:23:31','2025-07-10 19:24:35','2025-07-10 18:22:13'),(129,1,12,1,'Andrea Soler',NULL,'ABC-302','fe408da273b9eb52ce81dadec0f70b1831906328bb1c30262ac9ab331a6e597a','2025-11-08 20:12:19','2025-11-08 23:47:13','2025-11-08 20:09:49'),(130,1,12,3,'Camilo Blanco',NULL,'ABC-970','2290ca9e65c94dab699df25e2cf4e2e9be6dde6a5d295c19da632d443e3c9d1d','2025-07-17 13:40:31','2025-07-17 16:29:21','2025-07-17 13:40:21'),(131,1,13,1,'Ximena Varela',NULL,'ABC-678','e24aeb04010403459d3873f8432ce6ea23d9692d8dedcda0f74d233ec6c62d24','2025-08-17 12:04:36','2025-08-17 15:48:18','2025-08-17 12:03:13'),(132,1,14,1,'Eugenio Soto',NULL,'ABC-863','6959c636c748180cba610b5f5b720aa257dadb20947a25218ee160473d764795','2025-05-05 07:36:55','2025-05-05 08:36:00','2025-05-05 07:35:01'),(133,1,15,4,'Gina Acosta',NULL,'ABC-228','12a58bba12f78859f88b0d76fc10a9396d5c7d91eade0ff785f1a7bdb8574e9f','2025-07-06 16:53:37','2025-07-06 20:31:18','2025-07-06 16:52:33'),(134,1,15,3,'Nelson Marín',NULL,'ABC-059','31d5acd9339be5c235b735c01cbe08948afec8cc46599b7f4f12402f2939f721','2025-02-05 20:41:38','2025-02-05 22:26:03','2025-02-05 20:38:59'),(135,1,3,1,'Elsa Quintero',NULL,'ABC-378','143cada74c0247831558bbadcc7e2e832d6dc3a7651eec1485adabb373e89b91','2025-10-16 17:41:13','2025-10-16 23:04:31','2025-10-16 17:37:02'),(136,1,17,3,'Óscar Reyes',NULL,'ABC-481','47bc2f153462c34a463d39a6121c611140332256bbb947d29efa5aff775b6fd6','2025-03-05 13:29:34','2025-03-05 16:57:35','2025-03-05 13:25:57'),(137,1,17,4,'Paola Navarro',NULL,'ABC-819','482c4d1d01df84f2130e8244c671c4d8aa61d9173b41b3c15d9d552f5cbb6bb8','2025-09-22 18:25:11','2025-09-22 21:09:41','2025-09-22 18:20:13'),(138,1,17,4,'Raúl Cárdenas',NULL,'ABC-206','005daa145d17eeaac8d15645c322ddaa026d8d4cac09872858aae8b09f940f89','2025-07-26 08:04:23','2025-07-26 11:08:22','2025-07-26 08:02:22'),(139,1,8,2,'Silvana Mora',NULL,'ABC-029','032dcdc4f27ca82452fe5d4b1029e8ee23a92682f9d06da44ee97b0a374fe4d7','2025-05-19 20:04:00','2025-05-19 21:09:41','2025-05-19 19:59:03'),(140,1,7,2,'Tomás Gil',NULL,'ABC-576','2d98e5d0e447274f70a99319c39f0a375504d8c8099c9c7d7f371973da814f9e','2025-07-20 21:59:10','2025-07-20 23:31:28','2025-07-20 21:58:48'),(141,1,7,3,'Úrsula Valencia',NULL,'ABC-762','8fa7804685f1090fee6782e81b06a82be670b772bbf78ee6b00e563c30b3c9aa','2025-08-11 08:53:47','2025-08-11 12:35:39','2025-08-11 08:49:25'),(142,1,7,2,'Vicente Saavedra',NULL,'ABC-035','ef79c0d231ae7f6d292faf25b933f6773f500f4d8125e3e4e97a603315693018','2025-05-19 13:38:19','2025-05-19 18:56:25','2025-05-19 13:35:31'),(143,1,7,4,'Wendy López',NULL,'ABC-344','ea9002378a1ea72a9f82355152e8404a2c974e6f9afa84c6b8f9396119810965','2025-10-13 15:30:27','2025-10-13 17:27:47','2025-10-13 15:26:33'),(144,1,9,4,'Xavier Peña',NULL,'ABC-852','37847e1b3e26a0ddb9908b039ab21c4ec8f5665436bd00f5ab33ac472f041dbb','2025-01-03 17:24:00','2025-01-03 20:06:23','2025-01-03 17:23:07'),(145,1,9,1,'Yuliana Salas',NULL,'ABC-446','ba6d60223a71c89fa9033be0dd19ab1f54dfa10c2290362430e811536863ad9e','2025-06-09 20:04:54','2025-06-10 01:12:56','2025-06-09 20:04:21'),(146,1,9,3,'Zacarías Arias',NULL,'ABC-310','632ac90b5ab78c133d8aa89aa5e8b8089ba3a462145cd387240e7dfd1c1f296e','2025-08-09 21:41:47','2025-08-10 02:48:25','2025-08-09 21:38:01'),(147,1,10,2,'Amalia Castro',NULL,'ABC-981','622218fad8bce468eba512e221aec3198bb34ba13b2089e5b0196ca794022ca2','2025-11-11 13:19:10','2025-11-11 15:19:03','2025-11-11 13:17:49'),(148,1,10,2,'Bernardo Díaz',NULL,'ABC-878','6a0239e1be9560e838ebd6f51348d19aa7b28327806bad6daa28b3e2a685c320','2025-05-10 09:09:54','2025-05-10 12:27:18','2025-05-10 09:07:50'),(149,1,16,1,'Carla Fuentes',NULL,'ABC-522','a8eeba449a35af3bd927a531bf96fa0a668c881522cf350cc712a79eac1db178','2025-04-18 12:46:15','2025-04-18 18:00:53','2025-04-18 12:42:53'),(150,1,14,3,'Darío Herrera',NULL,'ABC-403','ddf665873dcc8a765a2049628cd8ff96c3f3e56c90e16e66beaa8379682b9ca4','2025-06-03 11:04:56','2025-06-03 16:27:17','2025-06-03 11:04:11'),(151,1,14,2,'Emilia Jiménez',NULL,'ABC-121','6b8ec3844c80150351b874eab091cef5e85136f973e15465a08e9ce5921648d8','2025-08-31 09:48:58','2025-08-31 14:07:57','2025-08-31 09:47:20'),(152,1,14,1,'Franco Múnera',NULL,'ABC-698','cdc2fc9d8ba3fcb5540db2cee651fab72019cd85e3782acdb0237b1429cd3f26','2025-03-30 12:18:15','2025-03-30 17:38:21','2025-03-30 12:13:58'),(153,1,16,1,'Gladys Orozco',NULL,'ABC-010','882a5e6593d5affef969a364b67de58fc7336b36013926ce6cba4857793d08bf','2025-04-22 08:17:38','2025-04-22 10:56:56','2025-04-22 08:12:58'),(154,1,15,1,'Iván Pinzón',NULL,'ABC-391','49394aa89fb5dba48ed5707a2a914fb82688a05f958c7f24f03f5cd5df4dd78e','2025-04-28 21:11:52','2025-04-29 01:04:09','2025-04-28 21:08:54'),(155,1,2,4,'Jessica Quintero',NULL,'ABC-125','dd159cdfd99242cf7c367026ccfa96cda523e5fe558741c8615d1fffa115c26e','2025-10-27 17:04:11','2025-10-27 20:58:49','2025-10-27 17:01:52'),(156,1,8,3,'Kevin Ramírez',NULL,'ABC-929','03bf8667464f71e0b1e69c9ed2fbc877409cc6453dfcb74b624b05f89e7df342','2025-03-06 15:54:06','2025-03-06 18:20:04','2025-03-06 15:53:07'),(157,1,8,3,'Lorena Soto',NULL,'ABC-104','3af44313a735ec22cd51d3dcda920a6ab159f6417949588be3d200175642bb4f','2025-09-09 09:40:20','2025-09-09 13:22:14','2025-09-09 09:36:44'),(158,1,8,4,'Manuel Tobón',NULL,'ABC-297','31bae43260e5da362da95ef7249251c106e842432741944828b34d85f334871b','2025-08-04 07:36:28','2025-08-04 09:30:45','2025-08-04 07:34:53'),(159,1,8,1,'Noelia Uribe',NULL,'ABC-498','08c74908171757a80fd824dff18b6c6c65a4d587e342ae45facd027f066773ea','2025-08-17 14:03:57','2025-08-17 16:08:17','2025-08-17 14:02:58'),(160,1,9,1,'Pablo Vélez',NULL,'ABC-073','d0dcb8d69819c16fc007eb56c0e4b5e216ca70da3490b0969b070f9e8a44443d','2025-11-23 11:20:44','2025-11-23 14:30:08','2025-11-23 11:16:34'),(161,1,9,5,'Quiteria Zárate',NULL,'ABC-351','40e36de55d899fe440695ada5d7ee8484f17c364775206744ed3b8b1b57dd333','2025-07-02 10:14:01','2025-07-02 12:56:37','2025-07-02 10:10:59'),(162,1,1,2,'Rodrigo Acuña',NULL,'ABC-423','c884740befe3d989c0c3a4ed1d81241266129db5f4f5a6b32006f504d6bf9d53','2025-08-09 14:07:59','2025-08-09 16:39:11','2025-08-09 14:04:49'),(163,1,15,2,'Sara Bernal',NULL,'ABC-643','26c559ec455dc07fdcbd2d5165793cdb71a12d9c126483b481e37eae56a5aae5','2025-11-02 16:43:48','2025-11-02 19:48:24','2025-11-02 16:40:25'),(164,1,15,4,'Tadeo Corredor',NULL,'ABC-832','52e5809c9a54f2ceb1198b30afa2dcaf59693428fa68d026e7b74022971290ee','2025-09-27 21:38:36','2025-09-28 00:30:36','2025-09-27 21:36:10'),(165,1,15,4,'Úrsula Durán',NULL,'ABC-418','95867ae02f2e1a223d142409d009e17ce03171d6fad6cf2775700936a1d5aac7','2025-11-16 11:32:16','2025-11-16 15:19:56','2025-11-16 11:30:01'),(166,1,15,2,'Valentina Escobar',NULL,'ABC-723','07c063931add574884104cc79d44ab80309cced60eafb2dd2f4c19fcd92d81fa','2025-03-10 17:23:34','2025-03-10 22:04:42','2025-03-10 17:22:37'),(167,1,15,5,'Wilson Flórez',NULL,'ABC-205','07167914c7d4dafb4c7daa20618ab17cda2ab36ae29d7392979faebc5a71d583','2025-04-24 09:14:17','2025-04-24 13:21:21','2025-04-24 09:13:04'),(168,1,18,2,'Yenny Gaviria',NULL,'ABC-159','4a062a08defbd9b415b65c98c8c55548833402cb39f891dfaa8086e222343ddc','2025-11-17 07:52:22','2025-11-17 10:31:54','2025-11-17 07:52:11'),(169,1,18,1,'Zoe Hernández',NULL,'ABC-050','ca1d74eb38f78c32e2c6d3c628819bff7e0a6fbc6a1d7c5fda9bb0107f889522','2025-09-23 20:07:53','2025-09-23 20:42:02','2025-09-23 20:05:37'),(170,1,18,1,'Ángel Ibarra',NULL,'ABC-372','6ee17aa7882398d0ef10598c1be2af21cb302234092c700461d9cf5558d2c3cc','2025-03-02 15:23:40','2025-03-02 17:11:14','2025-03-02 15:20:28'),(171,1,18,1,'Blanca Jaramillo',NULL,'ABC-418','8b678cb34bbb0bcdf35d74af5d7650a006f4aa27fd57087adf18f7acff22820b','2025-05-12 07:41:33','2025-05-12 08:28:48','2025-05-12 07:40:43'),(172,1,18,3,'César Londoño',NULL,'ABC-223','59db062686deb5dbfd4c8890da6755979147722cfd2573aa70af40fa1ea7b5df','2025-07-20 14:39:25','2025-07-20 18:56:13','2025-07-20 14:37:48'),(173,1,19,1,'Dalia Mesa',NULL,'ABC-805','1b92b9c01e674efb53c1166e4098b2f9e05624f51335f1a7e6726ec7ee69ecb3','2025-03-28 12:15:42','2025-03-28 17:34:52','2025-03-28 12:11:27'),(174,1,19,3,'Efrén Naranjo',NULL,'ABC-183','8cd33a9fe31a5042dd818cfa38b2ed0e1392444b9a7be5e8a2dc55b52b955dfe','2025-04-13 21:36:13','2025-04-14 02:48:06','2025-04-13 21:31:56'),(175,1,4,1,'Fabiola Orjuela',NULL,'ABC-614','43609e080110a219cd60a27e2b6167647c692467b8dbdb429d8eb918679f1b4e','2025-05-22 14:52:06','2025-05-22 17:09:48','2025-05-22 14:50:47'),(176,1,5,2,'Germán Pardo',NULL,'ABC-544','fb851d50e9e908c6fa16e99482d832054f0838faafa637abf34e6b66950bc0bf','2025-02-25 07:59:53','2025-02-25 12:37:27','2025-02-25 07:54:55'),(177,1,6,5,'Helena Quijano',NULL,'ABC-516','132250256d2b7f2c1d3de23f38e7fbc9986f70dd274d8c5474c8b9f8380228a4','2025-06-06 12:02:09','2025-06-06 13:55:45','2025-06-06 12:00:04'),(178,1,7,1,'Ignacio Restrepo',NULL,'ABC-278','edca1de3bd4abd4e6d27688b9258a5dc016d33dc9e62a9bc7b7c23dbd33448cd','2025-03-09 18:31:06','2025-03-09 20:12:08','2025-03-09 18:26:36'),(179,1,8,3,'Juana Salamanca',NULL,'ABC-485','d9ff3746a82d57e9eea39d4e2577136adc2e7b966e1d3bd150308251eaf0a6ac','2025-09-20 09:56:18','2025-09-20 13:35:29','2025-09-20 09:53:11'),(180,1,8,2,'Klaus Tamayo',NULL,'ABC-798','3caa64ad0e4fee4adf558abf9168c36024eef365ea3ab1165d039c3ec84343a1','2025-02-27 21:55:28','2025-02-28 00:42:20','2025-02-27 21:53:45'),(181,1,8,1,'Luisa Velásquez',NULL,'ABC-867','aed09e2f0faad21ae8b4fd10765d3878f13de1db54abeea004f90c5e502c357e','2025-04-06 13:07:52','2025-04-06 14:35:35','2025-04-06 13:04:06'),(182,1,8,5,'Mateo Yepes',NULL,'ABC-122','58b6dea14884ece812fe2e59c923945d51182c51df32d29c5eac9d31e5f10686','2025-02-28 16:09:41','2025-02-28 19:17:05','2025-02-28 16:05:30'),(183,1,8,1,'Nelly Zambrano',NULL,'ABC-898','f063acdeea405cae9477e73f6bdda492b69d4bfeac3f603dab740c5ed7a74a91','2025-07-14 12:43:03','2025-07-14 14:04:04','2025-07-14 12:39:26'),(184,1,8,4,'Óliver Álvarez',NULL,'ABC-071','07b8a463230f106167cff3c187b610ec0d27f98caf5e5a5c712b9f7ee0a3ee7a','2025-01-30 11:07:29','2025-01-30 12:10:23','2025-01-30 11:03:48'),(185,1,8,4,'Pilar Borja',NULL,'ABC-803','9fcf46a2e9a64808e322c790c31b40a18c00057a8a188aa8a208e536f6160df9','2025-04-21 13:43:24','2025-04-21 15:28:04','2025-04-21 13:38:48'),(186,1,8,3,'Quique Casas',NULL,'ABC-714','16ad53a8e287ed9b6945c6f23511c2215989e926260a8689d7f30e5f9710b43e','2025-10-13 14:00:41','2025-10-13 18:26:17','2025-10-13 13:57:42'),(187,1,8,1,'Raquel Delgado',NULL,'ABC-187','54f6bee637ad132061fae02fb2745e480b9a6c78dc1253b141dde96e3eb16bf8','2025-07-08 07:21:09','2025-07-08 10:00:47','2025-07-08 07:20:27'),(188,1,7,4,'Saúl Echeverri',NULL,'ABC-860','58af3188cff53d8bf2cc85b274f5299fa4756134f2db1d3cc25b75f91ab24a70','2025-04-17 10:00:15','2025-04-17 10:45:48','2025-04-17 09:56:55'),(189,1,20,4,'Tania Franco',NULL,'ABC-720','3d3b9ecf31f23dd765c20b75077cda90c4ecbc6975484b44463bcafe63aa4166','2025-02-22 18:53:55','2025-02-22 21:50:32','2025-02-22 18:53:19'),(190,1,20,1,'Ulises González',NULL,'ABC-483','c3f5c00e3c9ffbf670d3560b350f0cad0c13bc0cfbe0def1cbeb7712a1c169ea','2025-01-13 19:58:18','2025-01-13 21:31:46','2025-01-13 19:55:51'),(191,1,2,2,'Vivian Henao',NULL,'ABC-054','39562f0fe1d3616fc0fd96ee11c9b73f140f361758e69c1aac18baeee07121d9','2025-09-14 12:29:12','2025-09-14 15:39:17','2025-09-14 12:26:06'),(192,1,2,1,'Walter Isaza',NULL,'ABC-193','7af8bde3453c11e66ac274c2088bf64662390ea833167ba7e61965efc0646526','2025-06-02 13:13:14','2025-06-02 17:14:21','2025-06-02 13:11:31'),(193,1,2,2,'Yadira Jaimes',NULL,'ABC-247','cd312d284c014c7065a4196672c988c48de1fc213204d3ec49f2cb9920843875','2025-06-26 16:15:21','2025-06-26 19:16:51','2025-06-26 16:11:45'),(194,1,2,4,'Zelanda Klinger',NULL,'ABC-165','8ce8c279f615e319ac2944ac3e1908fae4e29c2b94aa8b8518e8e9250cc772f6','2025-01-15 07:56:30','2025-01-15 09:21:27','2025-01-15 07:52:46'),(195,1,2,2,'Adriana Latorre',NULL,'ABC-747','f2a245a8f5ad2b521ff8dd0180d7103dcd8cd1202e12373655134f6aa5ed5f5b','2025-02-22 15:19:33','2025-02-22 17:19:24','2025-02-22 15:15:15'),(196,1,3,4,'Benito Marroquín',NULL,'ABC-267','7b0dc002d2e7d5b9d980c20033d4fd1f8d90ecbbb54f5b30752ee5afda260712','2025-05-07 11:33:31','2025-05-07 13:59:27','2025-05-07 11:33:11'),(197,1,4,4,'Carolina Noguera',NULL,'ABC-629','0c64eba2f22ad3c644c5b835ff68c0fe0cc87d7948ce682f49830b0209037031','2025-01-30 11:11:41','2025-01-30 12:21:19','2025-01-30 11:07:31'),(198,1,3,2,'Diego Oviedo',NULL,'ABC-638','faec8e593b2d180f8a421cab3835019e6f344bce8cb5a2759690f06b627aa225','2025-09-14 11:37:51','2025-09-14 13:24:17','2025-09-14 11:35:58'),(199,1,3,1,'Estefanía Palacio',NULL,'ABC-550','f8e146813b148baddcfff9318dc89b56d9a6c7c2ed6307a2334ed108602a210d','2025-01-24 10:35:58','2025-01-24 15:58:17','2025-01-24 10:34:44'),(200,1,3,4,'Federico Quintero',NULL,'ABC-348','bdeb46b0d25c068b8b706bcc9db6cf470801a8caf766604a253b1b6d8e928fdc','2025-03-09 11:31:53','2025-03-09 16:29:19','2025-03-09 11:28:44'),(201,1,3,3,'Gloria Restrepo',NULL,'ABC-148',NULL,'2025-05-20 09:46:18','2025-05-20 13:38:28','2025-05-20 09:41:56'),(202,1,3,4,'Héctor Saldarriaga',NULL,'ABC-070',NULL,'2025-04-14 20:40:21','2025-04-15 00:19:16','2025-04-14 20:37:59'),(203,1,9,3,'Irene Torres',NULL,'ABC-111',NULL,'2025-05-21 17:12:44','2025-05-21 18:28:08','2025-05-21 17:09:05'),(204,1,9,1,'Jairo Urdaneta',NULL,'ABC-448',NULL,'2025-02-28 17:19:44','2025-02-28 22:21:24','2025-02-28 17:17:01'),(205,1,9,2,'Katia Valencia',NULL,'ABC-023',NULL,'2025-11-10 07:37:06','2025-11-10 10:08:28','2025-11-10 07:32:26'),(206,1,9,3,'Leopoldo Vásquez',NULL,'ABC-884',NULL,'2025-05-27 12:29:42','2025-05-27 15:36:30','2025-05-27 12:26:53'),(207,1,9,2,'Milena Wilches',NULL,'ABC-352',NULL,'2025-03-09 11:46:42','2025-03-09 17:10:31','2025-03-09 11:46:30'),(208,1,9,4,'Néstor Yepes',NULL,'ABC-585',NULL,'2025-02-14 15:54:45','2025-02-14 19:13:06','2025-02-14 15:54:20'),(209,1,9,4,'Olga Zambrano',NULL,'ABC-727',NULL,'2025-08-05 07:00:45','2025-08-05 07:53:09','2025-08-05 06:58:49'),(210,1,9,4,'Pedro Ávila',NULL,'ABC-218',NULL,'2025-08-10 09:25:20','2025-08-10 14:00:35','2025-08-10 09:21:57'),(211,1,9,3,'Quiteria Betancur',NULL,'ABC-893',NULL,'2025-10-20 11:49:17','2025-10-20 12:20:28','2025-10-20 11:48:56'),(212,1,9,4,'Rubén Caicedo',NULL,'ABC-628',NULL,'2025-04-01 09:31:59','2025-04-01 10:14:30','2025-04-01 09:28:26'),(213,1,9,2,'Silvia Dueñas',NULL,'ABC-944',NULL,'2025-05-16 20:20:55','2025-05-16 22:03:15','2025-05-16 20:18:06'),(214,1,9,2,'Tiberio Echeverri',NULL,'ABC-762',NULL,'2025-01-16 15:24:45','2025-01-16 19:11:18','2025-01-16 15:21:29'),(215,1,9,3,'Úrsula Flórez',NULL,'ABC-433',NULL,'2025-03-25 11:16:56','2025-03-25 15:09:49','2025-03-25 11:14:00'),(216,1,10,3,'Víctor Galindo',NULL,'ABC-297',NULL,'2025-10-13 14:24:38','2025-10-13 19:27:42','2025-10-13 14:23:50'),(217,1,10,2,'Wanda Henao',NULL,'ABC-594',NULL,'2025-11-18 11:58:09','2025-11-18 16:22:32','2025-11-18 11:53:16'),(218,1,19,3,'Xavier Ibarra',NULL,'ABC-879',NULL,'2025-06-22 16:15:10','2025-06-22 19:28:03','2025-06-22 16:10:37'),(219,1,19,2,'Yuliana Jiménez',NULL,'ABC-210',NULL,'2025-10-29 18:11:24','2025-10-29 18:54:18','2025-10-29 18:06:30'),(220,1,10,1,'Zaira Lara',NULL,'ABC-806',NULL,'2025-09-18 20:46:23','2025-09-18 22:37:30','2025-09-18 20:43:16'),(221,1,3,1,'Ángela Moncada',NULL,'ABC-476',NULL,'2025-04-04 14:48:57','2025-04-04 19:07:55','2025-04-04 14:47:19'),(222,1,19,4,'Bruno Noguera',NULL,'ABC-688',NULL,'2025-03-29 12:14:50','2025-03-29 17:30:07','2025-03-29 12:10:54'),(223,1,4,1,'Celia Osorio',NULL,'ABC-923',NULL,'2025-01-10 18:46:58','2025-01-10 23:25:13','2025-01-10 18:42:42'),(224,1,4,1,'Demetrio Paz',NULL,'ABC-556',NULL,'2025-09-04 08:31:02','2025-09-04 10:33:24','2025-09-04 08:29:40'),(225,1,4,2,'Eugenia Quiroga',NULL,'ABC-000',NULL,'2025-05-06 08:03:23','2025-05-06 09:43:36','2025-05-06 07:58:30'),(226,1,4,2,'Félix Rivera',NULL,'ABC-075',NULL,'2025-03-02 21:29:02','2025-03-02 23:23:34','2025-03-02 21:26:19'),(227,1,7,2,'Graciela Soto',NULL,'ABC-196',NULL,'2025-10-04 14:26:31','2025-10-04 15:01:49','2025-10-04 14:23:29'),(228,1,6,3,'Hernán Tamayo',NULL,'ABC-005',NULL,'2025-11-18 21:28:10','2025-11-19 02:41:49','2025-11-18 21:23:36'),(229,1,6,2,'Inés Uribe',NULL,'ABC-738',NULL,'2025-08-19 17:15:07','2025-08-19 19:31:56','2025-08-19 17:11:18'),(230,1,5,3,'Juan Vélez',NULL,'ABC-341',NULL,'2025-08-29 11:22:48','2025-08-29 13:26:10','2025-08-29 11:19:15'),(231,1,15,1,'Karen Wilches',NULL,'ABC-758',NULL,'2025-07-16 18:59:35','2025-07-16 20:42:07','2025-07-16 18:55:25'),(232,1,15,2,'Leonardo Yépez',NULL,'ABC-128',NULL,'2025-05-21 15:53:26','2025-05-21 19:53:31','2025-05-21 15:49:31'),(233,1,15,3,'Marcela Zambrano',NULL,'ABC-990',NULL,'2025-09-19 15:02:56','2025-09-19 17:16:49','2025-09-19 15:02:07'),(234,1,15,2,'Néstor Arango',NULL,'ABC-347',NULL,'2025-08-24 07:37:39','2025-08-24 08:40:42','2025-08-24 07:35:26'),(235,1,3,4,'Ofelia Botero',NULL,'ABC-565',NULL,'2025-10-10 20:17:31','2025-10-11 01:17:48','2025-10-10 20:12:54'),(236,1,18,3,'Pascual Cifuentes',NULL,'ABC-064',NULL,'2025-10-19 15:23:38','2025-10-19 16:52:56','2025-10-19 15:21:57'),(237,1,9,3,'Quintina Díaz',NULL,'ABC-561',NULL,'2025-01-10 09:30:32','2025-01-10 13:41:15','2025-01-10 09:29:17'),(238,1,9,2,'Mariano Montes',NULL,'ABC-278',NULL,'2025-11-17 07:38:26','2025-11-17 09:53:45','2025-11-17 07:35:08');
/*!40000 ALTER TABLE `visita` ENABLE KEYS */;
UNLOCK TABLES;

--
-- Final view structure for view `historial_visitas`
--

/*!50001 DROP VIEW IF EXISTS `historial_visitas`*/;
/*!50001 SET @saved_cs_client          = @@character_set_client */;
/*!50001 SET @saved_cs_results         = @@character_set_results */;
/*!50001 SET @saved_col_connection     = @@collation_connection */;
/*!50001 SET character_set_client      = utf8mb4 */;
/*!50001 SET character_set_results     = utf8mb4 */;
/*!50001 SET collation_connection      = utf8mb4_0900_ai_ci */;
/*!50001 CREATE ALGORITHM=UNDEFINED */
/*!50013 DEFINER=`root`@`localhost` SQL SECURITY DEFINER */
/*!50001 VIEW `historial_visitas` AS select `f`.`nombre` AS `nombre_fraccionamiento`,`r`.`nombre` AS `nombre_residencia`,`mv`.`nombre` AS `motivo_visita`,`v`.`nombre` AS `nombre`,`v`.`placa_vehiculo` AS `placa_vehiculo`,`v`.`fecha_hora_entrada` AS `fecha_hora_entrada`,`v`.`fecha_hora_salida` AS `fecha_hora_salida`,`v`.`codigo_qr` AS `codigo_qr` from (((`visita` `v` join `fraccionamiento` `f` on((`v`.`id_fraccionamiento` = `f`.`id_fraccionamiento`))) join `residencia` `r` on((`r`.`id_residencia` = `v`.`id_residencia`))) join `motivo_visita` `mv` on((`mv`.`id_motivo_visita` = `v`.`id_motivo_visita`))) order by `v`.`fecha_hora_entrada` */;
/*!50001 SET character_set_client      = @saved_cs_client */;
/*!50001 SET character_set_results     = @saved_cs_results */;
/*!50001 SET collation_connection      = @saved_col_connection */;

--
-- Final view structure for view `listado_residentes`
--

/*!50001 DROP VIEW IF EXISTS `listado_residentes`*/;
/*!50001 SET @saved_cs_client          = @@character_set_client */;
/*!50001 SET @saved_cs_results         = @@character_set_results */;
/*!50001 SET @saved_col_connection     = @@collation_connection */;
/*!50001 SET character_set_client      = utf8mb4 */;
/*!50001 SET character_set_results     = utf8mb4 */;
/*!50001 SET collation_connection      = utf8mb4_0900_ai_ci */;
/*!50001 CREATE ALGORITHM=UNDEFINED */
/*!50013 DEFINER=`root`@`localhost` SQL SECURITY DEFINER */
/*!50001 VIEW `listado_residentes` AS select `u`.`nombre_usuario` AS `nombre_usuario`,`p`.`nombre` AS `nombre`,`p`.`apellido_paterno` AS `apellido_paterno`,`p`.`apellido_materno` AS `apellido_materno`,`p`.`calle` AS `calle`,`p`.`numero` AS `numero`,`p`.`colonia` AS `colonia`,`p`.`fecha_registro` AS `fecha_registro`,`p`.`activo` AS `activo` from (((`usuario` `u` join `persona` `p` on((`u`.`id_persona` = `p`.`id_persona`))) join `fraccionamiento` `f` on((`f`.`id_fraccionamiento` = `u`.`id_fraccionamiento`))) join `rol_usuario` `r` on((`u`.`id_rol_usuario` = `r`.`id_rol_usuario`))) where ((`r`.`nombre` = 'Residente') and (`p`.`activo` = true)) */;
/*!50001 SET character_set_client      = @saved_cs_client */;
/*!50001 SET character_set_results     = @saved_cs_results */;
/*!50001 SET collation_connection      = @saved_col_connection */;
/*!40103 SET TIME_ZONE=@OLD_TIME_ZONE */;

/*!40101 SET SQL_MODE=@OLD_SQL_MODE */;
/*!40014 SET FOREIGN_KEY_CHECKS=@OLD_FOREIGN_KEY_CHECKS */;
/*!40014 SET UNIQUE_CHECKS=@OLD_UNIQUE_CHECKS */;
/*!40101 SET CHARACTER_SET_CLIENT=@OLD_CHARACTER_SET_CLIENT */;
/*!40101 SET CHARACTER_SET_RESULTS=@OLD_CHARACTER_SET_RESULTS */;
/*!40101 SET COLLATION_CONNECTION=@OLD_COLLATION_CONNECTION */;
/*!40111 SET SQL_NOTES=@OLD_SQL_NOTES */;

-- Dump completed on 2025-12-09 17:18:27
