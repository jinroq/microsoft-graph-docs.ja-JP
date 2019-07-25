---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 6e59bfa7171a935d0be9967bdd27f4dcf5188211
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35885856"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new QueryOption("expand", "fields"));

ListItemVersion listItemVersion = graphClient.sites("{site-id}").lists("{list-id}").items("{item-id}").versions("{version-id}")
    .buildRequest( requestOptions )
    .get();

```