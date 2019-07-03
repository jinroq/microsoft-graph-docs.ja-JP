---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: fd2c61e2d0a327cfcb5562c1744d683df3cd6bdb
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35496088"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/root/search(q='{search-query}')')
    .get();

```