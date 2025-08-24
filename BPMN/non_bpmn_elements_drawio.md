# Inne elementy które mogą być używane podczas tworzenia BPMN w draw.io

## 1. ELEMENTY Z BIBLIOTEKI GENERAL

### Podstawowe kształty geometryczne
```xml
<!-- Prostokąt -->
<mxCell id="1" value="Proces" style="whiteSpace=wrap;html=1;" vertex="1" parent="1">
  <mxGeometry x="100" y="100" width="120" height="60" as="geometry"/>
</mxCell>

<!-- Elipsa/Owale -->
<mxCell id="2" value="Start" style="ellipse;whiteSpace=wrap;html=1;" vertex="1" parent="1">
  <mxGeometry x="50" y="50" width="80" height="40" as="geometry"/>
</mxCell>

<!-- Romb (często używany jako bramka) -->
<mxCell id="3" value="Decyzja?" style="rhombus;whiteSpace=wrap;html=1;" vertex="1" parent="1">
  <mxGeometry x="200" y="80" width="80" height="80" as="geometry"/>
</mxCell>

<!-- Koło -->
<mxCell id="4" value="" style="ellipse;whiteSpace=wrap;html=1;aspect=fixed;" vertex="1" parent="1">
  <mxGeometry x="300" y="300" width="40" height="40" as="geometry"/>
</mxCell>

<!-- Sześciokąt -->
<mxCell id="5" value="Przygotowanie" style="hexagon;whiteSpace=wrap;html=1;" vertex="1" parent="1">
  <mxGeometry x="400" y="100" width="120" height="60" as="geometry"/>
</mxCell>

<!-- Trójkąt -->
<mxCell id="6" value="" style="triangle;whiteSpace=wrap;html=1;" vertex="1" parent="1">
  <mxGeometry x="500" y="200" width="60" height="40" as="geometry"/>
</mxCell>

<!-- Równoległobok -->
<mxCell id="7" value="Dane wejściowe" style="parallelogram;whiteSpace=wrap;html=1;" vertex="1" parent="1">
  <mxGeometry x="100" y="300" width="120" height="60" as="geometry"/>
</mxCell>
```

### Strzałki i wskaźniki
```xml
<!-- Strzałka blokowa -->
<mxCell id="8" value="" style="shape=singleArrow;whiteSpace=wrap;html=1;" vertex="1" parent="1">
  <mxGeometry x="200" y="400" width="100" height="30" as="geometry"/>
</mxCell>

<!-- Strzałka kierunkowa -->
<mxCell id="9" value="" style="shape=step;perimeter=stepPerimeter;whiteSpace=wrap;html=1;fixedSize=1;" vertex="1" parent="1">
  <mxGeometry x="350" y="400" width="80" height="40" as="geometry"/>
</mxCell>
```

## 2. ELEMENTY Z BIBLIOTEKI FLOWCHART

### Klasyczne kształty schematów blokowych
```xml
<!-- Start/End flowchart (owal terminatorski) -->
<mxCell id="10" value="Start" style="strokeWidth=2;html=1;shape=mxgraph.flowchart.start_1;whiteSpace=wrap;" vertex="1" parent="1">
  <mxGeometry x="100" y="500" width="100" height="40" as="geometry"/>
</mxCell>

<!-- Process rectangle (prostokąt procesowy) -->
<mxCell id="11" value="Proces" style="strokeWidth=2;html=1;shape=mxgraph.flowchart.process;whiteSpace=wrap;" vertex="1" parent="1">
  <mxGeometry x="250" y="500" width="100" height="60" as="geometry"/>
</mxCell>

<!-- Decision diamond (romb decyzyjny) -->
<mxCell id="12" value="Decyzja?" style="strokeWidth=2;html=1;shape=mxgraph.flowchart.decision;whiteSpace=wrap;" vertex="1" parent="1">
  <mxGeometry x="400" y="480" width="100" height="100" as="geometry"/>
</mxCell>

<!-- Document shape (dokument) -->
<mxCell id="13" value="Dokument" style="strokeWidth=2;html=1;shape=mxgraph.flowchart.document;whiteSpace=wrap;" vertex="1" parent="1">
  <mxGeometry x="100" y="600" width="100" height="60" as="geometry"/>
</mxCell>

<!-- Data/Input-Output shape (równoległobok danych) -->
<mxCell id="14" value="Dane" style="strokeWidth=2;html=1;shape=mxgraph.flowchart.data;whiteSpace=wrap;" vertex="1" parent="1">
  <mxGeometry x="250" y="600" width="100" height="60" as="geometry"/>
</mxCell>

<!-- Stored data (baza danych) -->
<mxCell id="15" value="Baza" style="strokeWidth=2;html=1;shape=mxgraph.flowchart.stored_data;whiteSpace=wrap;" vertex="1" parent="1">
  <mxGeometry x="400" y="600" width="100" height="60" as="geometry"/>
</mxCell>

<!-- Manual operation (operacja manualna) -->
<mxCell id="16" value="Ręczne" style="strokeWidth=2;html=1;shape=mxgraph.flowchart.manual_operation;whiteSpace=wrap;" vertex="1" parent="1">
  <mxGeometry x="100" y="700" width="100" height="60" as="geometry"/>
</mxCell>

<!-- Predefined process (podproces) -->
<mxCell id="17" value="Podproces" style="strokeWidth=2;html=1;shape=mxgraph.flowchart.predefined_process;whiteSpace=wrap;" vertex="1" parent="1">
  <mxGeometry x="250" y="700" width="100" height="60" as="geometry"/>
</mxCell>

<!-- Connector (punkt łączący) -->
<mxCell id="18" value="" style="strokeWidth=2;html=1;shape=mxgraph.flowchart.connector;whiteSpace=wrap;" vertex="1" parent="1">
  <mxGeometry x="420" y="720" width="60" height="20" as="geometry"/>
</mxCell>

<!-- Off-page connector (łącznik między stronami) -->
<mxCell id="19" value="A" style="strokeWidth=2;html=1;shape=mxgraph.flowchart.off-page_connector;whiteSpace=wrap;" vertex="1" parent="1">
  <mxGeometry x="500" y="700" width="60" height="60" as="geometry"/>
</mxCell>

<!-- Delay/Wait -->
<mxCell id="20" value="Oczekiwanie" style="strokeWidth=2;html=1;shape=mxgraph.flowchart.delay;whiteSpace=wrap;" vertex="1" parent="1">
  <mxGeometry x="100" y="800" width="100" height="60" as="geometry"/>
</mxCell>

<!-- Preparation (przygotowanie) -->
<mxCell id="21" value="Przygotowanie" style="strokeWidth=2;html=1;shape=mxgraph.flowchart.preparation;whiteSpace=wrap;" vertex="1" parent="1">
  <mxGeometry x="250" y="800" width="100" height="60" as="geometry"/>
</mxCell>

<!-- Display (wyświetlanie) -->
<mxCell id="22" value="Ekran" style="strokeWidth=2;html=1;shape=mxgraph.flowchart.display;whiteSpace=wrap;" vertex="1" parent="1">
  <mxGeometry x="400" y="800" width="100" height="60" as="geometry"/>
</mxCell>
```

## 3. ELEMENTY Z BIBLIOTEKI ADVANCED

### Kontenery i swimlanes
```xml
<!-- Container (kontener) -->
<mxCell id="23" value="Kontener" style="swimlane;whiteSpace=wrap;html=1;" vertex="1" parent="1">
  <mxGeometry x="100" y="900" width="200" height="120" as="geometry"/>
</mxCell>

<!-- Table (tabela) -->
<mxCell id="24" value="" style="swimlane;childLayout=tableLayout;rowLines=1;columnLines=1;tableFilter=1;" vertex="1" parent="1">
  <mxGeometry x="350" y="900" width="200" height="120" as="geometry"/>
</mxCell>

<!-- Cross-functional flowchart container -->
<mxCell id="25" value="Diagram krzyżowo-funkcjonalny" style="swimlane;html=1;childLayout=stackLayout;resizeParent=1;resizeParentMax=0;horizontal=1;startSize=20;" vertex="1" parent="1">
  <mxGeometry x="100" y="1050" width="400" height="200" as="geometry"/>
</mxCell>

<mxCell id="26" value="Dział A" style="swimlane;html=1;startSize=20;" vertex="1" parent="25">
  <mxGeometry y="20" width="400" height="90" as="geometry"/>
</mxCell>

<mxCell id="27" value="Dział B" style="swimlane;html=1;startSize=20;" vertex="1" parent="25">
  <mxGeometry y="110" width="400" height="90" as="geometry"/>
</mxCell>
```

## 4. ELEMENTY TEKSTOWE I ADNOTACJE

### Elementy tekstowe
```xml
<!-- Zwykły tekst -->
<mxCell id="28" value="Opis procesu" style="text;html=1;align=center;verticalAlign=middle;" vertex="1" parent="1">
  <mxGeometry x="600" y="100" width="100" height="40" as="geometry"/>
</mxCell>

<!-- Etykieta -->
<mxCell id="29" value="Etykieta" style="text;html=1;strokeColor=none;fillColor=none;align=center;verticalAlign=middle;whiteSpace=wrap;rounded=0;" vertex="1" parent="1">
  <mxGeometry x="600" y="200" width="60" height="30" as="geometry"/>
</mxCell>

<!-- Note (notatka) -->
<mxCell id="30" value="Notatka explicativa" style="shape=note;whiteSpace=wrap;html=1;backgroundOutline=1;darkOpacity=0.05;" vertex="1" parent="1">
  <mxGeometry x="600" y="300" width="80" height="60" as="geometry"/>
</mxCell>

<!-- Callout (dymek) -->
<mxCell id="31" value="Uwaga!" style="shape=callout;whiteSpace=wrap;html=1;perimeter=calloutPerimeter;" vertex="1" parent="1">
  <mxGeometry x="600" y="400" width="120" height="80" as="geometry"/>
</mxCell>
```

## 5. CONNECTORS (POŁĄCZENIA)

### Różne typy połączeń
```xml
<!-- Standardowe połączenie -->
<mxCell id="32" value="" style="edgeStyle=orthogonalEdgeStyle;rounded=0;html=1;jettySize=auto;orthogonalLoop=1;" edge="1" parent="1" source="1" target="3">
  <mxGeometry relative="1" as="geometry"/>
</mxCell>

<!-- Zakrzywione połączenie -->
<mxCell id="33" value="" style="curved=1;endArrow=classic;html=1;rounded=0;" edge="1" parent="1" source="3" target="5">
  <mxGeometry width="50" height="50" relative="1" as="geometry"/>
</mxCell>

<!-- Połączenie przerywaną linią -->
<mxCell id="34" value="" style="endArrow=classic;html=1;rounded=0;dashed=1;" edge="1" parent="1" source="5" target="7">
  <mxGeometry width="50" height="50" relative="1" as="geometry"/>
</mxCell>

<!-- Dwukierunkowe połączenie -->
<mxCell id="35" value="" style="endArrow=classic;startArrow=classic;html=1;rounded=0;" edge="1" parent="1" source="7" target="1">
  <mxGeometry width="50" height="50" relative="1" as="geometry"/>
</mxCell>

<!-- Połączenie z etykietą -->
<mxCell id="36" value="TAK" style="endArrow=classic;html=1;rounded=0;" edge="1" parent="1" source="12" target="11">
  <mxGeometry width="50" height="50" relative="1" as="geometry"/>
</mxCell>
```

## 6. IKONY I SYMBOLE POMOCNICZE

### Ikony systemowe i techniczne
```xml
<!-- Ikona komputera -->
<mxCell id="37" value="" style="fontColor=#0066CC;verticalAlign=top;verticalLabelPosition=bottom;labelPosition=center;align=center;html=1;outlineConnect=0;fillColor=#CCCCCC;strokeColor=#6881B3;gradientColor=none;gradientDirection=north;strokeWidth=2;shape=mxgraph.networks.pc;" vertex="1" parent="1">
  <mxGeometry x="700" y="100" width="100" height="70" as="geometry"/>
</mxCell>

<!-- Ikona serwera -->
<mxCell id="38" value="" style="fontColor=#0066CC;verticalAlign=top;verticalLabelPosition=bottom;labelPosition=center;align=center;html=1;outlineConnect=0;fillColor=#CCCCCC;strokeColor=#6881B3;gradientColor=none;gradientDirection=north;strokeWidth=2;shape=mxgraph.networks.server;" vertex="1" parent="1">
  <mxGeometry x="700" y="200" width="105" height="105" as="geometry"/>
</mxCell>

<!-- Ikona bazy danych -->
<mxCell id="39" value="" style="shape=cylinder3;whiteSpace=wrap;html=1;boundedLbl=1;backgroundOutline=1;size=15;" vertex="1" parent="1">
  <mxGeometry x="700" y="350" width="60" height="80" as="geometry"/>
</mxCell>

<!-- Ikona użytkownika -->
<mxCell id="40" value="" style="shape=umlActor;verticalLabelPosition=bottom;verticalAlign=top;html=1;outlineConnect=0;" vertex="1" parent="1">
  <mxGeometry x="700" y="450" width="30" height="60" as="geometry"/>
</mxCell>

<!-- Ikona dokumentu -->
<mxCell id="41" value="" style="shape=document;whiteSpace=wrap;html=1;boundedLbl=1;" vertex="1" parent="1">
  <mxGeometry x="700" y="530" width="80" height="60" as="geometry"/>
</mxCell>
```

## 7. ELEMENTY DEKORACYJNE I POMOCNICZE

### Elementy wizualne
```xml
<!-- Linia prosta -->
<mxCell id="42" value="" style="endArrow=none;html=1;rounded=0;" edge="1" parent="1">
  <mxGeometry width="50" height="50" relative="1" as="geometry">
    <mxPoint x="100" y="1300" as="sourcePoint"/>
    <mxPoint x="300" y="1300" as="targetPoint"/>
  </mxGeometry>
</mxCell>

<!-- Ramka grupująca -->
<mxCell id="43" value="Grupa procesów" style="rounded=0;whiteSpace=wrap;html=1;dashed=1;dashPattern=5 5;fillColor=none;" vertex="1" parent="1">
  <mxGeometry x="50" y="1350" width="200" height="150" as="geometry"/>
</mxCell>

<!-- Chmura (dla elementów zewnętrznych) -->
<mxCell id="44" value="System zewnętrzny" style="ellipse;shape=cloud;whiteSpace=wrap;html=1;" vertex="1" parent="1">
  <mxGeometry x="300" y="1350" width="120" height="80" as="geometry"/>
</mxCell>
```

## 8. ELEMENTY UML (często mieszane z BPMN)

### Aktor i przypadki użycia
```xml
<!-- Aktor UML -->
<mxCell id="45" value="Użytkownik" style="shape=umlActor;verticalLabelPosition=bottom;verticalAlign=top;html=1;" vertex="1" parent="1">
  <mxGeometry x="500" y="1350" width="30" height="60" as="geometry"/>
</mxCell>

<!-- Use case -->
<mxCell id="46" value="Przypadek użycia" style="ellipse;whiteSpace=wrap;html=1;" vertex="1" parent="1">
  <mxGeometry x="580" y="1350" width="120" height="60" as="geometry"/>
</mxCell>
```

## 9. STYLE CZĘSTO UŻYWANE PRZY MIESZANIU Z BPMN

### Modyfikacje stylów dla lepszej integracji
```xml
<!-- Prostokąt w stylu BPMN (zaokrąglone rogi) -->
<mxCell id="47" value="Zadanie hybrydowe" style="rounded=1;whiteSpace=wrap;html=1;strokeWidth=1;" vertex="1" parent="1">
  <mxGeometry x="100" y="1550" width="120" height="60" as="geometry"/>
</mxCell>

<!-- Elipsa w stylu zdarzeń BPMN -->
<mxCell id="48" value="" style="ellipse;whiteSpace=wrap;html=1;aspect=fixed;strokeWidth=2;" vertex="1" parent="1">
  <mxGeometry x="280" y="1560" width="40" height="40" as="geometry"/>
</mxCell>

<!-- Romb z dodatkowym stylem -->
<mxCell id="49" value="?" style="rhombus;whiteSpace=wrap;html=1;strokeWidth=2;fillColor=#fff2cc;strokeColor=#d6b656;" vertex="1" parent="1">
  <mxGeometry x="380" y="1540" width="80" height="80" as="geometry"/>
</mxCell>
```

## UWAGI DOTYCZĄCE MIESZANIA ELEMENTÓW:

### 1. Konsistencja wizualna
- Używaj podobnej szerokości obrysu (`strokeWidth`)
- Zachowaj spójność kolorów
- Dopasuj rozmiary elementów

### 2. Semantyczna zgodność
- Elementy flowchart mogą zastąpić podstawowe zadania BPMN
- Ikony systemowe dobrze uzupełniają pule BPMN
- Adnotacje tekstowe wyjaśniają złożone procesy

### 3. Najczęstsze kombinacje
- **BPMN + General shapes**: dla uproszczonych diagramów
- **BPMN + Flowchart**: dla klasycznych schematów z elementami BPMN
- **BPMN + Advanced containers**: dla złożonych swimlanes
- **BPMN + UML actors**: dla diagramów z wyraźnymi rolami

### 4. Dobre praktyki
- Używaj legend do wyjaśnienia nietypowych elementów
- Grupuj podobne elementy w kontenerach
- Zachowaj czytelność poprzez ograniczenie różnorodności kształtów
- Stosuj spójne nazewnictwo w całym diagramie

