---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 255904f4500b7ba27d9904214ef191b1bc6d99fd
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/27/2019
ms.locfileid: "36637908"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const publishedResource = {
    displayName: "Demo provisioning (updated)"
};

let res = await client.api('/onPremisesPublishingProfiles/provisioning/publishedResources/1234b780-965f-4149-85c5-a8c73e58b67d')
    .version('beta')
    .update(publishedResource);

```