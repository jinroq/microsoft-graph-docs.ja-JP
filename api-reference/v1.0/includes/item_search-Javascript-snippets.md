---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: fd2c61e2d0a327cfcb5562c1744d683df3cd6bdb
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34482277"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/root/search(q='{search-query}')')
    .get();

```