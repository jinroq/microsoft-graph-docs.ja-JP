---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: fd2c61e2d0a327cfcb5562c1744d683df3cd6bdb
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35730808"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/root/search(q='{search-query}')')
    .get();

```