---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 45a1c143054dae06e329730f1867c020bb71af56
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35710400"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const alert = {
  value: [
    {
      assignedTo: "String",
      closedDateTime: "String (timestamp)",
      comments: ["String"],
      feedback: {@odata.type: "microsoft.graph.alertFeedback"},
      id: "String (identifier)",
      status: {@odata.type: "microsoft.graph.alertStatus"},
      tags: ["String"],
      vendorInformation:
        {
          provider: "String",
          vendor: "String"
        }
    }
  ]
};

let res = await client.api('/security/alerts/updateAlerts')
    .version('beta')
    .post(alert);

```