---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: b52e605d9319f349c70317c22c4ec03586b784bc
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35705858"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/search(q='{search-query}')')
    .version('beta')
    .get();

```