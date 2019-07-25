---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 9d8cd1af3ded6dc3399971c3dc2ddaeb7b2d85f8
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35888092"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Content content = graphClient.me().drive().items("{item-id}").thumbnails("{thumb-id}").{size}().content()
    .buildRequest()
    .get();

```