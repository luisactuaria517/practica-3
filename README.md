# practica-3
intro series de tiempo

pob <- sample(100:120, 15, replace = F) #vector con rango 100 a 120 con 15 datos
pob
pobts <- ts (pob, frequency = 1,start = 2000)
pobts
end (pobts)
plot(pobts)
plot(aggregate(pobts))

infor<-ts(read.csv(("C:\\Users\\luisa\\OneDrive\\Documentos\\r series de tiempo\\IndicadoresENOE_2017-02-08.xls.csv"), header = T), frequency = 4, start = 2005);
infor

info1<-read.csv("C:\\Users\\luisa\\OneDrive\\Documentos\\r series de tiempo\\IndicadoresENOE_2017-02-08a.xls.csv")#,header = T), frequency = 4, start = 2005)
info1ts<- ts(info1[,1], frequency = 4, start = 2005, end = 2015)
info1ts
plot(info1ts)

#### ts ocupacion
info1ts1<- ts(info1[,2], frequency = 4, start = 2005, end = 2015)
info1ts1
plot(info1ts1)

#### ts salario
info1ts2<- ts(info1[,3], frequency = 4, start = 2005, end = 2015)
info1ts2
plot(info1ts2)

#### ts condiciones
info1ts3<- ts(info1[,4], frequency = 4, start = 2005, end = 2015)
info1ts3
plot(info1ts3)
