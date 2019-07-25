---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 3f59e5537c413e2dd0117eb3350564f55349fec8
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35717939"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const secureScoreControlProfile = {
  controlStateUpdates: "controlStateUpdates-value"
};

let res = await client.api('/security/secureScoreControlProfiles/AdminMFA')
    .version('beta')
    .update({secureScoreControlProfile : secureScoreControlProfile});

```