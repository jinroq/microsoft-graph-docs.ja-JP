---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 8c7a60acc5aeacfa557e2158c834dfd8b35a2c72
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35326247"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/mailFolders/AAMkAGVmMDEzN')
    .get();

```