---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 183ac8343e76ac87eb3931798eb5e55c4e1058e9
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35740984"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/contactFolders/delta')
    .header('Prefer','odata.maxpagesize=2')
    .get();

```