---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: ba604b293d5b2eba531ed5f929b356df6c795444
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35877832"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

OrgContact orgContact = new OrgContact();
LinkedList<String> businessPhonesList = new LinkedList<String>();
businessPhonesList.add("businessPhones-value");
orgContact.businessPhones = businessPhonesList;
orgContact.city = "city-value";
orgContact.companyName = "companyName-value";
orgContact.country = "country-value";
orgContact.department = "department-value";
orgContact.displayName = "displayName-value";

graphClient.contacts("{id}")
    .buildRequest()
    .patch(orgContact);

```