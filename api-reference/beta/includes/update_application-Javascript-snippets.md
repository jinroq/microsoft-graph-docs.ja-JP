---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 82c74e311ca9950ebda94559940b8d6bf1d28098
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34465644"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const application = {
  allowPublicClient: false,
  displayName: "New display name"
};

let res = await client.api('/applications/{id}')
    .version('beta')
    .update({application : application});

```