---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: e5e5057e8a0381c3b1a45c5dbed20e5020ddbbd4
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34471663"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/education/synchronizationProfiles/{id}/profileStatus')
    .version('beta')
    .get();

```