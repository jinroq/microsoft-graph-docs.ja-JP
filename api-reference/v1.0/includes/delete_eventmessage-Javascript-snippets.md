---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: a4bfc7172adb61ed99b9f7d2fbc8f25a2c0e2177
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34459208"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/messages/{id}')
    .delete();

```