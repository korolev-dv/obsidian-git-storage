---
24-04-2023
---

Для работы со сложными сточки зрения сериализации значений могут использоваться следующие методы:

ЗаписатьXML()
ПрочитатьXML()

Метод ВозможностьЧтенияXML() определяет, возможно ли считывание значения из объекта ЧтениеXML.

Пример записи в XML
```bsl
ЗаписатьXML(ЗаписьXML, ДокументОбъект, НазначениеТипаXML.Явное);
```

Пример чтения из XML

```bsl
Если ЧтениеXML.Прочитать() Тогда
	Если ВозможностьЧтенияXML(ЧтениеXML) Тогда
		Объект = ПрочитатьXML(ЧтениеXML);
		Объект.Записать();
	КонецЕсли;
КонецЕсли;
```

[[1С]]
[[Программирование]]