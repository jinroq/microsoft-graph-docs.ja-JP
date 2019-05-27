---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: e2e6aeb839929f019d81d4d8bae77d045a50fa87
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34465504"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/ownedDevices')
    .get();

```