---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 3bf80dfaadcdaf8ef4a247700875952b3196d50d
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35721677"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/mailFolders/AAMkAGVmMDEzM/')
    .version('beta')
    .delete();

```