# CIIU4_EAM
Gráficos CIIU4 EAM
########CIIU
library(dplyr)
library(ggplot2)
library(scales)

CIIU <- read_excel("IICA/Banco Mundial/CIIU.xlsx")







CIIU %>%
  filter(`1011` != 0) %>%
  arrange(desc(`1011`)) %>%
  ggplot(aes(x = reorder(Departamento, `1011`), y = `1011`, fill = Departamento, label = paste0(round(`1011` / sum(`1011`) * 100, 2), "%"))) +
  geom_bar(stat = "identity") +
  geom_text(vjust = -0.5) +
  coord_flip() +
  theme_minimal() +
  labs(x = "Departamento", y = "Valor", fill = "Departamento", title = "Porcentaje de materia prima nacional comprada en la categoría 1011 Procesamiento y conservación de carne y productos cárnicos ")


CIIU %>%
  filter(`1020` != 0) %>%
  arrange(desc(`1020`)) %>%
  ggplot(aes(x = reorder(Departamento, `1020`), y = `1020`, fill = Departamento, label = paste0(round(`1020` / sum(`1020`) * 100, 2), "%"))) +
  geom_bar(stat = "identity") +
  geom_text(vjust = -0.5) +
  coord_flip() +
  theme_minimal() +
  labs(x = "Departamento", y = "Valor", fill = "Departamento", title = "Porcentaje de materia prima nacional comprada en la categoría 1020 Procesamiento y conservación de frutas, legumbres, hortalizas y tubérculos")

CIIU %>%
  filter(`1051` != 0) %>%
  arrange(desc(`1051`)) %>%
  ggplot(aes(x = reorder(Departamento, `1051`), y = `1051`, fill = Departamento, label = paste0(round(`1051` / sum(`1051`) * 100, 2), "%"))) +
  geom_bar(stat = "identity") +
  geom_text(vjust = -0.5) +
  coord_flip() +
  theme_minimal() +
  labs(x = "Departamento", y = "Valor", fill = "Departamento", title = "Porcentaje de materia prima nacional comprada en la categoría 1051 Elaboración de productos de molinería  ")

CIIU %>%
  filter(`1052` != 0) %>%
  arrange(desc(`1052`)) %>%
  ggplot(aes(x = reorder(Departamento, `1052`), y = `1052`, fill = Departamento, label = paste0(round(`1052` / sum(`1052`) * 100, 2), "%"))) +
  geom_bar(stat = "identity") +
  geom_text(vjust = -0.5) +
  coord_flip() +
  theme_minimal() +
  labs(x = "Departamento", y = "Valor", fill = "Departamento", title = "Porcentaje de materia prima nacional comprada en la categoría 1052 Elaboración de almidones y productos derivados del almidón")

CIIU %>%
  filter(`1061` != 0) %>%
  arrange(desc(`1061`)) %>%
  ggplot(aes(x = reorder(Departamento, `1061`), y = `1061`, fill = Departamento, label = paste0(round(`1061` / sum(`1061`) * 100, 2), "%"))) +
  geom_bar(stat = "identity") +
  geom_text(vjust = -0.5) +
  coord_flip() +
  theme_minimal() +
  labs(x = "Departamento", y = "Valor", fill = "Departamento", title = "Porcentaje de materia prima nacional comprada en la categoría 1061 Trilla de café")


CIIU %>%
  filter(`1062` != 0) %>%
  arrange(desc(`1062`)) %>%
  ggplot(aes(x = reorder(Departamento, `1062`), y = `1062`, fill = Departamento, label = paste0(round(`1062` / sum(`1062`) * 100, 2), "%"))) +
  geom_bar(stat = "identity") +
  geom_text(vjust = -0.5) +
  coord_flip() +
  theme_minimal() +
  labs(x = "Departamento", y = "Valor", fill = "Departamento", title = "Porcentaje de materia prima nacional comprada en la categoría 1062 Descafeinado, tostión y molienda del café")

CIIU %>%
  filter(`1082` != 0) %>%
  arrange(desc(`1062`)) %>%
  ggplot(aes(x = reorder(Departamento, `1082`), y = `1082`, fill = Departamento, label = paste0(round(`1082` / sum(`1082`) * 100, 2), "%"))) +
  geom_bar(stat = "identity") +
  geom_text(vjust = -0.5) +
  coord_flip() +
  theme_minimal() +
  labs(x = "Departamento", y = "Valor", fill = "Departamento", title = "Porcentaje de materia prima nacional comprada en la categoría 1082 Elaboración de cacao, chocolate y productos de confitería")

CIIU %>%
  filter(`1090` != 0) %>%
  arrange(desc(`1090`)) %>%
  ggplot(aes(x = reorder(Departamento, `1090`), y = `1090`, fill = Departamento, label = paste0(round(`1090` / sum(`1090`) * 100, 2), "%"))) +
  geom_bar(stat = "identity") +
  geom_text(vjust = -0.5) +
  coord_flip() +
  theme_minimal() +
  labs(x = "Departamento", y = "Valor", fill = "Departamento", title = "Porcentaje de materia prima nacional comprada en la categoría 1090 Elaboración de alimentos preparados para animales")

CIIU %>%
  filter(`1511` != 0) %>%
  arrange(desc(`1511`)) %>%
  ggplot(aes(x = reorder(Departamento, `1511`), y = `1511`, fill = Departamento, label = paste0(round(`1511` / sum(`1511`) * 100, 2), "%"))) +
  geom_bar(stat = "identity") +
  geom_text(vjust = -0.5) +
  coord_flip() +
  theme_minimal() +
  labs(x = "Departamento", y = "Valor", fill = "Departamento", title = "Porcentaje de materia prima nacional comprada en la categoría 1511 Curtido y recurtido de cueros; recurtido y teñido de pieles")

CIIU %>%
  filter(`1512` != 0) %>%
  arrange(desc(`1512`)) %>%
  ggplot(aes(x = reorder(Departamento, `1512`), y = `1512`, fill = Departamento, label = paste0(round(`1512` / sum(`1512`) * 100, 2), "%"))) +
  geom_bar(stat = "identity") +
  geom_text(vjust = -0.5) +
  coord_flip() +
  theme_minimal() +
  labs(x = "Departamento", y = "Valor", fill = "Departamento", title = "Porcentaje de materia prima nacional comprada en la categoría 1512 Fabricación de artículos de viaje, bolsos de mano y artículos similares elaborados en cuero, 
       y fabricación de artículos de talabartería y guarnicionería.")

CIIU %>%
  filter(`1521` != 0) %>%
  arrange(desc(`1521`)) %>%
  ggplot(aes(x = reorder(Departamento, `1521`), y = `1521`, fill = Departamento, label = paste0(round(`1521` / sum(`1521`) * 100, 2), "%"))) +
  geom_bar(stat = "identity") +
  geom_text(vjust = -0.5) +
  coord_flip() +
  theme_minimal() +
  labs(x = "Departamento", y = "Valor", fill = "Departamento", title = "Porcentaje de materia prima nacional comprada en la categoría 1521 Fabricación de calzado de cuero y piel, con cualquier tipo de suela")
