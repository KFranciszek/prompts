# Dokładna lista elementów BPMN w kodzie XML draw.io

## Struktura podstawowa XML draw.io

```xml
<mxGraphModel>
  <root>
    <mxCell id="0"/>
    <mxCell id="1" parent="0"/>
    <!-- Elementy BPMN tutaj -->
  </root>
</mxGraphModel>
```

## 1. ZDARZENIA (Events)

### Start Event (Zdarzenie początkowe)
```xml
<mxCell id="2" value="" style="ellipse;whiteSpace=wrap;html=1;aspect=fixed;" vertex="1" parent="1">
  <mxGeometry x="100" y="100" width="40" height="40" as="geometry"/>
</mxCell>
```

### End Event (Zdarzenie końcowe)
```xml
<mxCell id="3" value="" style="ellipse;whiteSpace=wrap;html=1;aspect=fixed;strokeWidth=3;" vertex="1" parent="1">
  <mxGeometry x="300" y="100" width="40" height="40" as="geometry"/>
</mxCell>
```

### Intermediate Event (Zdarzenie pośrednie)
```xml
<mxCell id="4" value="" style="ellipse;whiteSpace=wrap;html=1;aspect=fixed;strokeWidth=2;" vertex="1" parent="1">
  <mxGeometry x="200" y="100" width="40" height="40" as="geometry"/>
</mxCell>
```

### Message Start Event (Zdarzenie początkowe z wiadomością)
```xml
<mxCell id="5" value="" style="ellipse;whiteSpace=wrap;html=1;aspect=fixed;points=[[0.145,0.145,0],[0.5,0,0],[0.855,0.145,0],[1,0.5,0],[0.855,0.855,0],[0.5,1,0],[0.145,0.855,0],[0,0.5,0]];" vertex="1" parent="1">
  <mxGeometry x="100" y="200" width="40" height="40" as="geometry"/>
</mxCell>
<!-- Ikona wiadomości wewnątrz zdarzenia -->
<mxCell id="6" value="" style="shape=message;html=1;html=1;fillColor=#ffffff;strokeColor=#000000;" vertex="1" parent="1">
  <mxGeometry x="110" y="210" width="20" height="14" as="geometry"/>
</mxCell>
```

### Timer Start Event (Zdarzenie czasowe)
```xml
<mxCell id="7" value="" style="ellipse;whiteSpace=wrap;html=1;aspect=fixed;" vertex="1" parent="1">
  <mxGeometry x="100" y="300" width="40" height="40" as="geometry"/>
</mxCell>
<!-- Ikona zegara -->
<mxCell id="8" value="" style="shape=mxgraph.bpmn.timer;html=1;" vertex="1" parent="1">
  <mxGeometry x="110" y="310" width="20" height="20" as="geometry"/>
</mxCell>
```

## 2. ZADANIA (Tasks)

### Basic Task (Zadanie podstawowe)
```xml
<mxCell id="9" value="Zadanie" style="rounded=1;whiteSpace=wrap;html=1;" vertex="1" parent="1">
  <mxGeometry x="150" y="200" width="100" height="60" as="geometry"/>
</mxCell>
```

### User Task (Zadanie użytkownika)
```xml
<mxCell id="10" value="Zadanie użytkownika" style="rounded=1;whiteSpace=wrap;html=1;" vertex="1" parent="1">
  <mxGeometry x="150" y="300" width="100" height="60" as="geometry"/>
</mxCell>
<!-- Ikona użytkownika -->
<mxCell id="11" value="" style="shape=mxgraph.bpmn.user_task;html=1;" vertex="1" parent="1">
  <mxGeometry x="155" y="340" width="15" height="15" as="geometry"/>
</mxCell>
```

### Service Task (Zadanie serwisowe)
```xml
<mxCell id="12" value="Zadanie serwisowe" style="rounded=1;whiteSpace=wrap;html=1;" vertex="1" parent="1">
  <mxGeometry x="150" y="400" width="100" height="60" as="geometry"/>
</mxCell>
<!-- Ikona narzędzia -->
<mxCell id="13" value="" style="shape=mxgraph.bpmn.service_task;html=1;" vertex="1" parent="1">
  <mxGeometry x="155" y="440" width="15" height="15" as="geometry"/>
</mxCell>
```

### Script Task (Zadanie skryptowe)
```xml
<mxCell id="14" value="Zadanie skryptowe" style="rounded=1;whiteSpace=wrap;html=1;" vertex="1" parent="1">
  <mxGeometry x="150" y="500" width="100" height="60" as="geometry"/>
</mxCell>
<!-- Ikona skryptu -->
<mxCell id="15" value="" style="shape=mxgraph.bpmn.script_task;html=1;" vertex="1" parent="1">
  <mxGeometry x="155" y="540" width="15" height="15" as="geometry"/>
</mxCell>
```

### Manual Task (Zadanie manualne)
```xml
<mxCell id="16" value="Zadanie manualne" style="rounded=1;whiteSpace=wrap;html=1;" vertex="1" parent="1">
  <mxGeometry x="300" y="300" width="100" height="60" as="geometry"/>
</mxCell>
<!-- Ikona ręki -->
<mxCell id="17" value="" style="shape=mxgraph.bpmn.manual_task;html=1;" vertex="1" parent="1">
  <mxGeometry x="305" y="340" width="15" height="15" as="geometry"/>
</mxCell>
```

### Business Rule Task (Zadanie reguł biznesowych)
```xml
<mxCell id="18" value="Reguły biznesowe" style="rounded=1;whiteSpace=wrap;html=1;" vertex="1" parent="1">
  <mxGeometry x="300" y="400" width="100" height="60" as="geometry"/>
</mxCell>
<!-- Ikona tabeli -->
<mxCell id="19" value="" style="shape=mxgraph.bpmn.business_rule_task;html=1;" vertex="1" parent="1">
  <mxGeometry x="305" y="440" width="15" height="15" as="geometry"/>
</mxCell>
```

### Receive Task (Zadanie odbierające)
```xml
<mxCell id="20" value="Zadanie odbierające" style="rounded=1;whiteSpace=wrap;html=1;" vertex="1" parent="1">
  <mxGeometry x="300" y="500" width="100" height="60" as="geometry"/>
</mxCell>
<!-- Ikona wiadomości przychodzącej -->
<mxCell id="21" value="" style="shape=mxgraph.bpmn.receive_task;html=1;" vertex="1" parent="1">
  <mxGeometry x="305" y="540" width="15" height="15" as="geometry"/>
</mxCell>
```

### Send Task (Zadanie wysyłające)
```xml
<mxCell id="22" value="Zadanie wysyłające" style="rounded=1;whiteSpace=wrap;html=1;" vertex="1" parent="1">
  <mxGeometry x="450" y="300" width="100" height="60" as="geometry"/>
</mxCell>
<!-- Ikona wiadomości wychodzącej -->
<mxCell id="23" value="" style="shape=mxgraph.bpmn.send_task;html=1;fillColor=#000000;" vertex="1" parent="1">
  <mxGeometry x="455" y="340" width="15" height="15" as="geometry"/>
</mxCell>
```

## 3. BRAMKI (Gateways)

### Exclusive Gateway (Bramka wyłączająca)
```xml
<mxCell id="24" value="" style="rhombus;whiteSpace=wrap;html=1;" vertex="1" parent="1">
  <mxGeometry x="280" y="180" width="40" height="40" as="geometry"/>
</mxCell>
<!-- Symbol X -->
<mxCell id="25" value="X" style="text;html=1;align=center;verticalAlign=middle;fontSize=16;fontWeight=bold;" vertex="1" parent="1">
  <mxGeometry x="295" y="195" width="10" height="10" as="geometry"/>
</mxCell>
```

### Parallel Gateway (Bramka równoległa)
```xml
<mxCell id="26" value="" style="rhombus;whiteSpace=wrap;html=1;" vertex="1" parent="1">
  <mxGeometry x="380" y="180" width="40" height="40" as="geometry"/>
</mxCell>
<!-- Symbol + -->
<mxCell id="27" value="+" style="text;html=1;align=center;verticalAlign=middle;fontSize=16;fontWeight=bold;" vertex="1" parent="1">
  <mxGeometry x="395" y="195" width="10" height="10" as="geometry"/>
</mxCell>
```

### Inclusive Gateway (Bramka włączająca)
```xml
<mxCell id="28" value="" style="rhombus;whiteSpace=wrap;html=1;" vertex="1" parent="1">
  <mxGeometry x="480" y="180" width="40" height="40" as="geometry"/>
</mxCell>
<!-- Symbol okręgu -->
<mxCell id="29" value="○" style="text;html=1;align=center;verticalAlign=middle;fontSize=16;fontWeight=bold;" vertex="1" parent="1">
  <mxGeometry x="495" y="195" width="10" height="10" as="geometry"/>
</mxCell>
```

### Event-based Gateway (Bramka oparta na zdarzeniach)
```xml
<mxCell id="30" value="" style="rhombus;whiteSpace=wrap;html=1;" vertex="1" parent="1">
  <mxGeometry x="580" y="180" width="40" height="40" as="geometry"/>
</mxCell>
<!-- Symbol pięciokąta -->
<mxCell id="31" value="" style="shape=pentagon;perimeter=pentagonPerimeter2;whiteSpace=wrap;html=1;fixedSize=1;" vertex="1" parent="1">
  <mxGeometry x="590" y="190" width="20" height="20" as="geometry"/>
</mxCell>
```

## 4. PRZEPŁYWY (Flows)

### Sequence Flow (Przepływ sekwencyjny)
```xml
<mxCell id="32" value="" style="edgeStyle=orthogonalEdgeStyle;rounded=0;html=1;jettySize=auto;orthogonalLoop=1;strokeWidth=2;endArrow=block;endFill=1;" edge="1" parent="1" source="9" target="24">
  <mxGeometry relative="1" as="geometry"/>
</mxCell>
```

### Message Flow (Przepływ wiadomości)
```xml
<mxCell id="33" value="" style="edgeStyle=orthogonalEdgeStyle;rounded=0;html=1;jettySize=auto;orthogonalLoop=1;strokeWidth=1;endArrow=block;endFill=0;startArrow=oval;startFill=1;dashed=1;" edge="1" parent="1" source="pool1" target="pool2">
  <mxGeometry relative="1" as="geometry"/>
</mxCell>
```

### Association (Skojarzenie)
```xml
<mxCell id="34" value="" style="edgeStyle=orthogonalEdgeStyle;rounded=0;html=1;jettySize=auto;orthogonalLoop=1;strokeWidth=1;endArrow=none;endFill=0;dashed=1;dashPattern=1 4;" edge="1" parent="1" source="annotation" target="task">
  <mxGeometry relative="1" as="geometry"/>
</mxCell>
```

## 5. SWIMLANES

### Pool (Pula)
```xml
<mxCell id="35" value="Pula procesu" style="swimlane;html=1;childLayout=stackLayout;resizeParent=1;resizeParentMax=0;horizontal=1;startSize=20;horizontalStack=0;" vertex="1" parent="1">
  <mxGeometry x="80" y="80" width="640" height="200" as="geometry"/>
</mxCell>
```

### Lane (Ścieżka)
```xml
<mxCell id="36" value="Ścieżka 1" style="swimlane;html=1;startSize=20;" vertex="1" parent="35">
  <mxGeometry y="20" width="640" height="90" as="geometry"/>
</mxCell>

<mxCell id="37" value="Ścieżka 2" style="swimlane;html=1;startSize=20;" vertex="1" parent="35">
  <mxGeometry y="110" width="640" height="90" as="geometry"/>
</mxCell>
```

## 6. SUB-PROCESY

### Sub-Process (Podproces)
```xml
<mxCell id="38" value="Podproces" style="rounded=1;whiteSpace=wrap;html=1;" vertex="1" parent="1">
  <mxGeometry x="200" y="400" width="120" height="80" as="geometry"/>
</mxCell>
<!-- Symbol + na dole -->
<mxCell id="39" value="+" style="text;html=1;align=center;verticalAlign=middle;fontSize=12;fontWeight=bold;" vertex="1" parent="1">
  <mxGeometry x="255" y="465" width="10" height="10" as="geometry"/>
</mxCell>
```

### Call Activity (Wywołanie aktywności)
```xml
<mxCell id="40" value="Wywołanie aktywności" style="rounded=1;whiteSpace=wrap;html=1;strokeWidth=3;" vertex="1" parent="1">
  <mxGeometry x="350" y="400" width="120" height="80" as="geometry"/>
</mxCell>
```

## 7. ARTEFAKTY (Artifacts)

### Data Object (Obiekt danych)
```xml
<mxCell id="41" value="Dane" style="shape=note;whiteSpace=wrap;html=1;backgroundOutline=1;" vertex="1" parent="1">
  <mxGeometry x="500" y="400" width="60" height="80" as="geometry"/>
</mxCell>
```

### Data Store (Magazyn danych)
```xml
<mxCell id="42" value="Baza danych" style="shape=datastore;whiteSpace=wrap;html=1;" vertex="1" parent="1">
  <mxGeometry x="600" y="400" width="60" height="60" as="geometry"/>
</mxCell>
```

### Text Annotation (Adnotacja tekstowa)
```xml
<mxCell id="43" value="To jest adnotacja" style="shape=note;whiteSpace=wrap;html=1;backgroundOutline=1;darkOpacity=0.05;" vertex="1" parent="1">
  <mxGeometry x="500" y="300" width="80" height="60" as="geometry"/>
</mxCell>
```

### Group (Grupa)
```xml
<mxCell id="44" value="" style="rounded=0;whiteSpace=wrap;html=1;dashed=1;dashPattern=5 5;fillColor=none;" vertex="1" parent="1">
  <mxGeometry x="180" y="500" width="200" height="100" as="geometry"/>
</mxCell>
<!-- Etykieta grupy -->
<mxCell id="45" value="Grupa elementów" style="text;html=1;align=center;verticalAlign=middle;" vertex="1" parent="1">
  <mxGeometry x="280" y="580" width="80" height="15" as="geometry"/>
</mxCell>
```

## 8. SPECJALNE STYLE MXGRAPH.BPMN

### Używanie standardowych ikon BPMN
```xml
<!-- Ikona użytkownika -->
<mxCell value="" style="shape=mxgraph.bpmn.user_task;html=1;" vertex="1" parent="1"/>

<!-- Ikona serwisu -->
<mxCell value="" style="shape=mxgraph.bpmn.service_task;html=1;" vertex="1" parent="1"/>

<!-- Ikona skryptu -->
<mxCell value="" style="shape=mxgraph.bpmn.script_task;html=1;" vertex="1" parent="1"/>

<!-- Ikona ręki -->
<mxCell value="" style="shape=mxgraph.bpmn.manual_task;html=1;" vertex="1" parent="1"/>

<!-- Ikona reguł -->
<mxCell value="" style="shape=mxgraph.bpmn.business_rule_task;html=1;" vertex="1" parent="1"/>

<!-- Ikona wysyłania -->
<mxCell value="" style="shape=mxgraph.bpmn.send_task;html=1;fillColor=#000000;" vertex="1" parent="1"/>

<!-- Ikona odbierania -->
<mxCell value="" style="shape=mxgraph.bpmn.receive_task;html=1;" vertex="1" parent="1"/>

<!-- Ikona zegara -->
<mxCell value="" style="shape=mxgraph.bpmn.timer;html=1;" vertex="1" parent="1"/>

<!-- Ikona wiadomości -->
<mxCell value="" style="shape=message;html=1;" vertex="1" parent="1"/>

<!-- Ikona błędu -->
<mxCell value="" style="shape=mxgraph.bpmn.error;html=1;" vertex="1" parent="1"/>

<!-- Ikona sygnału -->
<mxCell value="" style="shape=triangle;html=1;" vertex="1" parent="1"/>
```

## 9. CHOREOGRAFIA BPMN 2.0

### Choreography Task (Zadanie choreografii)
```xml
<mxCell id="46" value="Choreografia" style="rounded=1;whiteSpace=wrap;html=1;strokeWidth=2;" vertex="1" parent="1">
  <mxGeometry x="200" y="600" width="150" height="100" as="geometry"/>
</mxCell>
<!-- Pasek uczestnika -->
<mxCell id="47" value="Uczestnik A" style="rounded=0;whiteSpace=wrap;html=1;fillColor=#cccccc;" vertex="1" parent="1">
  <mxGeometry x="200" y="600" width="150" height="25" as="geometry"/>
</mxCell>
<!-- Pasek drugiego uczestnika -->
<mxCell id="48" value="Uczestnik B" style="rounded=0;whiteSpace=wrap;html=1;fillColor=#cccccc;" vertex="1" parent="1">
  <mxGeometry x="200" y="675" width="150" height="25" as="geometry"/>
</mxCell>
```

## 10. KONWERSACJE

### Conversation (Konwersacja)
```xml
<mxCell id="49" value="Konwersacja" style="hexagon;whiteSpace=wrap;html=1;" vertex="1" parent="1">
  <mxGeometry x="400" y="600" width="100" height="60" as="geometry"/>
</mxCell>
```

## UWAGI TECHNICZNE:

1. **Kompresja**: Draw.io może kompresować XML - aby uzyskać czytelny format, użyj opcji "Uncompressed" podczas eksportu.

2. **ID**: Każdy element musi mieć unikalny identyfikator `id`.

3. **Parent**: Elementy muszą wskazywać na swojego rodzica (`parent="1"` dla głównego obszaru roboczego).

4. **Geometry**: Każdy element wizualny musi mieć zdefiniowaną geometrię z pozycją (x,y) i rozmiarem (width, height).

5. **Style**: Wszystkie właściwości wizualne są zdefiniowane w atrybucie `style` jako lista par klucz=wartość oddzielona średnikami.

6. **Vertex/Edge**: Elementy mogą być typu `vertex="1"` (kształty) lub `edge="1"` (połączenia).

