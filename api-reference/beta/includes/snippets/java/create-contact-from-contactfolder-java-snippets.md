---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 5f58edae71fb91e5cf6baa6d2ec67b0aa7257923
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35863173"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Contact contact = new Contact();
contact.parentFolderId = "parentFolderId-value";
contact.birthday = "2016-10-19T10:37:00Z";
contact.fileAs = "fileAs-value";
contact.displayName = "displayName-value";
contact.givenName = "givenName-value";
contact.initials = "initials-value";

graphClient.me().contactFolders("{id}").contacts()
    .buildRequest()
    .post(contact);

```