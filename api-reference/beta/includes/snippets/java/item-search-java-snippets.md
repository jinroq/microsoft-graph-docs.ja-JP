---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 97db53acb30c7289186089511fe2602a9a9d8d33
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36324265"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IDriveItemCollectionPage search = graphClient.me().drive().root()
    .search("{search-query}")
    .buildRequest()
    .get();

```