---
description: 自動生成されたファイル。 変更しないでください
ms.openlocfilehash: d3562450eecf2d2e4376018ac26b4ee912bb9df1
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36367250"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IDriveItemCollectionPage search = graphClient.me().drive()
    .search("{search-query}")
    .buildRequest()
    .get();

```