---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 5ea2a96f99eb2a9f1f4355d40d45ae5dc19410d8
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35718287"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/riskyUsers')
    .version('beta')
    .get();

```