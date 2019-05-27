---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 0f0d13c781508ca5f0d1db64eeb2955bfe2b417e
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34468471"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/sharedWithMe')
    .get();

```