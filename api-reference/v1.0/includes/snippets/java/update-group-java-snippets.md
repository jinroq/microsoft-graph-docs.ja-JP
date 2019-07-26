---
description: 自動生成されたファイル。 変更しないでください
ms.openlocfilehash: a04a0be5cc6b297a879a668d12337b49bd94d572
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35885323"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Group group = new Group();
group.description = "description-value";
group.displayName = "displayName-value";
LinkedList<String> groupTypesList = new LinkedList<String>();
groupTypesList.add("groupTypes-value");
group.groupTypes = groupTypesList;
group.mail = "mail-value";
group.mailEnabled = true;
group.mailNickname = "mailNickname-value";

graphClient.groups("{id}")
    .buildRequest()
    .patch(group);

```