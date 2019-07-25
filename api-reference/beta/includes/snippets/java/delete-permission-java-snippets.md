---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: aee750c1a4d2c276bd66a8815055a96e681793d7
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35877006"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().drive().root().items().{item-id}().permissions().{perm-id}()
    .buildRequest()
    .delete();

```