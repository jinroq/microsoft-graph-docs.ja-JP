---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 27b09df3845d18e5985d6367dcdb7c11f3659ea6
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/27/2019
ms.locfileid: "36637932"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const hybridAgentUpdaterConfiguration = {
    "allowUpdateConfigurationOverride" : false
};

let res = await client.api('/onPremisesPublishingProfiles/provisioning/hybridAgentUpdaterConfiguration')
    .version('beta')
    .update(hybridAgentUpdaterConfiguration);

```