---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: fc4507ae44b2338c7646909aa1f9dafaf0ee16b6
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35878736"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/onPremisesPublishingProfiles/provisioning/agents/1234b780-965f-4149-85c5-a8c73e58b67d/')
    .version('beta')
    .expand('agentGroups')
    .get();

```