---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 81a8c6be7627fdb048e997e452f111ef6798c170
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34472701"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/mailFolders/AAMkAGVmMDEzM/childFolders')
    .version('beta')
    .get();

```