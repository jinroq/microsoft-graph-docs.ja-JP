---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 86021fd7e606eab6baf025d12852367fe04e4966
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34469168"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const mailFolder = {
  displayName: "displayName-value",
};

let res = await client.api('/me/mailFolders/AAMkAGVmMDEzM')
    .version('beta')
    .update({mailFolder : mailFolder});

```