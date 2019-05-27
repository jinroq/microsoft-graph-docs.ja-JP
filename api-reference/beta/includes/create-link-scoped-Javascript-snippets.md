---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 61393570191320e984864693f2bfe29a820c5cda
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34460784"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const permission = {
  type: "edit",
  scope: "organization"
};

let res = await client.api('/me/drive/items/{item-id}/createLink')
    .version('beta')
    .post(permission);

```