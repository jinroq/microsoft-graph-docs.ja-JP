---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: d39f0d02f67a4458097b3fbf20855db6f7c29c31
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35707089"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/devices/{id}')
    .version('beta')
    .delete();

```