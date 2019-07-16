---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 3db31f97ed1d7e2c04a0a40e79326e643fcef0c6
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35739018"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/root')
    .get();

```