---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 1ce72091d0feacdaceb68cf4f4daba1e88581f0d
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35892905"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().onenote().pages("{id}")
    .buildRequest()
    .delete();

```