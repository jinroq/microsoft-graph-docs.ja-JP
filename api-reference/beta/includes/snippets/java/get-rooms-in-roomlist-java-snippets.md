---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 93658075abf9a35ad236766e7288624c6e377462
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35876796"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IRoomCollectionPage rooms = graphClient.places("bldg2@contoso.com").microsoft.graph.roomlist().rooms()
    .buildRequest()
    .get();

```