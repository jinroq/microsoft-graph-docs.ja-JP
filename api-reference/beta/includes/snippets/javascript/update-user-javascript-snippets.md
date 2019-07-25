---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 6fc26052e0b9848ceb750096bb949f343125d0e1
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35716231"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const user = {
  accountEnabled: true,
  assignedLicenses: [
    {
      disabledPlans: [ "bea13e0c-3828-4daa-a392-28af7ff61a0f" ],
      skuId: "skuId-value"
    }
  ],
  assignedPlans: [
    {
      assignedDateTime: "2016-10-19T10:37:00Z",
      capabilityStatus: "capabilityStatus-value",
      service: "service-value",
      servicePlanId: "bea13e0c-3828-4daa-a392-28af7ff61a0f"
    }
  ],
  businessPhones: [
    "businessPhones-value"
  ],
  city: "city-value"
};

let res = await client.api('/me')
    .version('beta')
    .update({user : user});

```