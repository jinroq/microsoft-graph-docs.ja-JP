---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: f2b953204c9bb83daf296b4d9552ac17f647e435
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36307744"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IWorkbookRangeViewCollectionPage rows = graphClient.me().drive().root().workbook().worksheets("{id}")
    .range("A1:Z10")
    .visibleView().rows()
    .buildRequest()
    .get();

```