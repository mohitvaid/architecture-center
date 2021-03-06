---
title: Visual Assistant

titleSuffix: Azure Solution Ideas
author: adamboeglin
ms.date: 12/16/2019
description: Visual assistant provides rich information based on content of the image with capabilities such as reading business card, identifying barcode, and recognizing popular people, places, objects, artworks, and monuments.
ms.custom: acom-architecture, ai-ml, visual assistant, cognitive services, visual capabilities, visual assistant scenarios, interactive-diagram, 'https://azure.microsoft.com/solutions/architecture/visual-assistant/'
ms.service: architecture-center
ms.subservice: solution-idea
---
# Visual Assistant


[!INCLUDE [header_file](../header.md)]

Visual assistant provides rich information based on content of the image with capabilities such as reading business card, identifying barcode, and recognizing popular people, places, objects, artworks, and monuments.

## Architecture

![Architecture diagram](../media/visual-assistant.svg)


## Data Flow

1. Users interact with bot
1. Bot understands context from LUIS
1. Bot passes visual context to the Bing Visual Search API
1. Bot gets additional information from Bing Entity Search for rich context on people, place, artwork, monument, and objects.
1. Bot gets additional information for barcodes.
1. Optionally Bot gets more information on barcodes/queries exclusively from your domain through the Bing Custom Search API.
1. Assistant renders similar products/destinations from your domain or provides more information around celebrity/place/monuments/artworks.



