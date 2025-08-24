# Prompt do konwersji opisu biznesowego na diagram BPMN

## Instrukcja główna
Przekształć poniższy opis procesu biznesowego w kompletny diagram BPMN 2.0, zawierający wszystkie elementy notacji. Wynikowy diagram powinien być w formacie XML kompatybilnym z Draw.io (diagrams.net).

## Wymagania analizy

### 1. Identyfikacja elementów procesu
Zidentyfikuj i wyodrębnij z opisu:

**Zdarzenia (Events):**
- Start Events (zdarzenia początkowe) - gdzie proces się rozpoczyna
- End Events (zdarzenia końcowe) - gdzie proces się kończy
- Intermediate Events (zdarzenia pośrednie) - przerwania, timery, sygnały, wiadomości
- Boundary Events (zdarzenia graniczne) - obsługa wyjątków, timeouty

**Aktywności (Activities):**
- User Tasks (zadania użytkownika) - czynności wykonywane przez człowieka
- Service Tasks (zadania serwisowe) - automatyczne operacje systemowe
- Manual Tasks (zadania manualne) - czynności bez wsparcia systemowego
- Script Tasks (zadania skryptowe) - automatyczne wykonanie skryptu
- Business Rule Tasks (zadania reguł biznesowych) - decyzje oparte na regułach
- Call Activities (wywołania podprocesów) - odwołania do innych procesów
- Sub-processes (podprocesy) - zgrupowane aktywności

**Bramki (Gateways):**
- Exclusive Gateway (XOR) - wybór jednej ścieżki z wielu
- Parallel Gateway (AND) - podział na równoległe ścieżki
- Inclusive Gateway (OR) - wybór jednej lub więcej ścieżek
- Event-based Gateway - decyzja oparta na zdarzeniach
- Complex Gateway - złożone warunki decyzyjne

**Przepływy (Flows):**
- Sequence Flows (przepływy sekwencyjne) - standardowe połączenia
- Conditional Flows (przepływy warunkowe) - z warunkami na połączeniach
- Default Flows (przepływy domyślne) - ścieżki alternatywne
- Message Flows (przepływy wiadomości) - komunikacja między pulami

**Artefakty (Artifacts):**
- Data Objects (obiekty danych) - dokumenty, dane wejściowe/wyjściowe
- Data Stores (magazyny danych) - bazy danych, repozytoria
- Groups (grupy) - logiczne grupowanie elementów
- Text Annotations (adnotacje) - dodatkowe opisy i komentarze

**Swimlanes:**
- Pools (pule) - organizacje lub systemy
- Lanes (tory) - role, departamenty, osoby

### 2. Analiza przepływu

**Ścieżki główne:**
- Zidentyfikuj główną ścieżkę procesu (happy path)
- Określ sekwencję kroków w normalnym przebiegu

**Ścieżki alternatywne:**
- Wszystkie możliwe odchylenia od głównej ścieżki
- Warunki prowadzące do alternatywnych ścieżek
- Punkty decyzyjne i kryteria wyboru

**Ścieżki wyjątkowe:**
- Obsługa błędów i wyjątków
- Procedury awaryjne
- Kompensacje i wycofywanie operacji

**Pętle i iteracje:**
- Czynności powtarzalne
- Warunki zakończenia pętli
- Maksymalna liczba iteracji

### 3. Szczegóły implementacyjne

**Dla każdego zadania określ:**
- Nazwę (krótką, opisową)
- Typ zadania
- Wykonawcę (rolę/system)
- Dane wejściowe
- Dane wyjściowe
- Czas trwania (jeśli podany)
- Warunki rozpoczęcia
- Warunki zakończenia

**Dla każdej bramki określ:**
- Typ bramki
- Warunki dla każdego wyjścia
- Priorytet ścieżek (jeśli istotny)
- Ścieżkę domyślną

**Dla każdego zdarzenia określ:**
- Typ zdarzenia
- Trigger (wyzwalacz)
- Rezultat
- Czy jest to zdarzenie przerwające/nieprzerwające

### 4. Reguły biznesowe i ograniczenia

- SLA (Service Level Agreements) - czasy wykonania
- Eskalacje - procedury gdy przekroczono czas
- Uprawnienia - kto może wykonać dane zadanie
- Walidacje - sprawdzanie poprawności danych
- Zależności między zadaniami
- Ograniczenia zasobowe

## Format wyjściowy

### Struktura XML dla Draw.io

Wygeneruj diagram w formacie:

```xml
<mxfile host="app.diagrams.net" modified="2024-01-01T00:00:00.000Z" agent="5.0" version="24.0.0" etag="xxx" type="device">
  <diagram id="unique-id" name="Nazwa Procesu">
    <mxGraphModel dx="1434" dy="796" grid="1" gridSize="10" guides="1" tooltips="1" connect="1" arrows="1" fold="1" page="1" pageScale="1" pageWidth="1169" pageHeight="827" math="0" shadow="0">
      <root>
        <mxCell id="0"/>
        <mxCell id="1" parent="0"/>
        
        <!-- Pools i Lanes -->
        [Definicje pul i torów]
        
        <!-- Start Events -->
        [Zdarzenia początkowe z odpowiednimi stylami BPMN]
        
        <!-- Tasks -->
        [Zadania z ikonami typu zadania]
        
        <!-- Gateways -->
        [Bramki z odpowiednimi symbolami]
        
        <!-- End Events -->
        [Zdarzenia końcowe]
        
        <!-- Sequence Flows -->
        [Połączenia z etykietami warunków]
        
        <!-- Data Objects -->
        [Obiekty danych i ich powiązania]
        
        <!-- Annotations -->
        [Adnotacje tekstowe]
        
      </root>
    </mxGraphModel>
  </diagram>
</mxfile>
```

### Styl elementów BPMN dla Draw.io

**Start Event:**
```xml
style="shape=mxgraph.bpmn.shape;html=1;verticalLabelPosition=bottom;labelBackgroundColor=#ffffff;verticalAlign=top;align=center;perimeter=ellipsePerimeter;outlineConnect=0;outline=standard;symbol=general;"
```

**User Task:**
```xml
style="shape=mxgraph.bpmn.task;html=1;outlineConnect=0;taskMarker=user;"
```

**Service Task:**
```xml
style="shape=mxgraph.bpmn.task;html=1;outlineConnect=0;taskMarker=service;"
```

**Exclusive Gateway:**
```xml
style="shape=mxgraph.bpmn.shape;html=1;verticalLabelPosition=bottom;labelBackgroundColor=#ffffff;verticalAlign=top;align=center;perimeter=rhombusPerimeter;background=gateway;outlineConnect=0;outline=standard;symbol=exclusiveGw;"
```

**Parallel Gateway:**
```xml
style="shape=mxgraph.bpmn.shape;html=1;verticalLabelPosition=bottom;labelBackgroundColor=#ffffff;verticalAlign=top;align=center;perimeter=rhombusPerimeter;background=gateway;outlineConnect=0;outline=standard;symbol=parallelGw;"
```

## Przykład użycia

### Input (opis procesu):
"Proces rozpoczyna się gdy klient składa zamówienie. Pracownik działu sprzedaży weryfikuje zamówienie. Jeśli wartość przekracza 10000 zł, wymagana jest akceptacja kierownika. Po akceptacji system automatycznie sprawdza dostępność towaru. Jeśli towar jest dostępny, generowane jest zlecenie dla magazynu i równolegle wysyłana jest faktura do klienta. Magazynier przygotowuje przesyłkę. Proces kończy się gdy kurier odbiera paczkę."

### Output (fragment XML):
```xml
<!-- Start Event -->
<mxCell id="start1" value="Złożenie zamówienia" style="shape=mxgraph.bpmn.shape;html=1;verticalLabelPosition=bottom;labelBackgroundColor=#ffffff;verticalAlign=top;align=center;perimeter=ellipsePerimeter;outlineConnect=0;outline=standard;symbol=general;" vertex="1" parent="1">
  <mxGeometry x="50" y="200" width="50" height="50" as="geometry"/>
</mxCell>

<!-- User Task -->
<mxCell id="task1" value="Weryfikacja zamówienia" style="shape=mxgraph.bpmn.task;html=1;outlineConnect=0;taskMarker=user;" vertex="1" parent="1">
  <mxGeometry x="150" y="180" width="120" height="80" as="geometry"/>
</mxCell>

<!-- Exclusive Gateway -->
<mxCell id="gw1" value="Wartość > 10000?" style="shape=mxgraph.bpmn.shape;html=1;verticalLabelPosition=bottom;labelBackgroundColor=#ffffff;verticalAlign=top;align=center;perimeter=rhombusPerimeter;background=gateway;outlineConnect=0;outline=standard;symbol=exclusiveGw;" vertex="1" parent="1">
  <mxGeometry x="320" y="195" width="50" height="50" as="geometry"/>
</mxCell>

<!-- Sequence Flow with condition -->
<mxCell id="flow1" value="TAK" style="edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;" edge="1" parent="1" source="gw1" target="task2">
  <mxGeometry relative="1" as="geometry"/>
</mxCell>
```

## Dodatkowe wytyczne

1. **Kompletność:** Uwzględnij WSZYSTKIE elementy i kroki opisane w tekście
2. **Czytelność:** Rozmieść elementy logicznie, unikaj przecinających się linii
3. **Standardy:** Używaj oficjalnej notacji BPMN 2.0
4. **Etykiety:** Każdy element powinien mieć czytelną nazwę
5. **Warunki:** Wszystkie przepływy warunkowe muszą mieć opisane warunki
6. **Komentarze:** Dodaj adnotacje dla nieoczywistych elementów
7. **Walidacja:** Sprawdź czy diagram ma przynajmniej jeden start i end event
8. **Spójność:** Każdy element musi być połączony z przepływem

## Weryfikacja końcowa

Przed wygenerowaniem ostatecznego XML sprawdź:
- [ ] Czy wszystkie opisane aktywności są uwzględnione?
- [ ] Czy wszystkie decyzje mają zdefiniowane warunki?
- [ ] Czy ścieżki alternatywne są kompletne?
- [ ] Czy role/wykonawcy są przypisani do zadań?
- [ ] Czy diagram można zaimportować do Draw.io?
- [ ] Czy zachowano standardy BPMN 2.