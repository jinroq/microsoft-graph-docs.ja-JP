---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 228c3890adee6bf5c7f308d255268667ec4df6dd
ms.sourcegitcommit: 56c0b609dfb1bc5d900956f407d107cdab7086e8
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/30/2019
ms.locfileid: "35933965"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().drive().items("{item-id}").unfollow()
    .buildRequest()
    .delete();

```