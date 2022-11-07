---
title: How Parts are Made
description: Flow of Concepts to Parts
weight: 2
---

{{< mermaid >}}
graph TD
    A(Concept) --> B(Design Intent)
    B --> C(Design: CAD/Drawings)
    C --> D(CAM)
    D --> E(CNC Machine)
    E --> F[Final Part]
    E --> 1

    C --> 1(Manual Operations)
    1 --> F
{{< /mermaid >}}