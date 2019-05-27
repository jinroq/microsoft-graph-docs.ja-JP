---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 6d2488ce8ef0a8e0afd944ab044c0c981be38d5c
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34472673"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/mailFolders/searchfolders/childFolders')
    .version('beta')
    .get();

```