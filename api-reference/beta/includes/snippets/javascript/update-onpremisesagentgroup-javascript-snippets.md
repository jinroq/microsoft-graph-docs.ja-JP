---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 7117d2042eb3056a4300811d934333ee3f880c1d
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35878322"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const onPremisesAgentGroup = {
    displayName: "Group New Name"
};

let res = await client.api('/onPremisesPublishingProfiles/provisioning/agentGroups/8832388F-3814-4952-B288-FFB62081FE25/')
    .version('beta')
    .update({onPremisesAgentGroup : onPremisesAgentGroup});

```