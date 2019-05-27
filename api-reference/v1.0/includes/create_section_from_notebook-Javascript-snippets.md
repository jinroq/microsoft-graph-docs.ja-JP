---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: cc71407e30ba0bf8342b4f4023e5ddeba3179644
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34460054"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const onenoteSection = {
  displayName: "Section name"
};

let res = await client.api('/me/onenote/notebooks/{id}/sections')
    .post({onenoteSection : onenoteSection});

```