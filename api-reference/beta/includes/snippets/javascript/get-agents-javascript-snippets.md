---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 10658d8b0edd166df60879b81eec0c0000a56d8c
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35878678"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/onPremisesPublishingProfiles/provisioning/agents')
    .version('beta')
    .expand('agentGroups')
    .get();

```