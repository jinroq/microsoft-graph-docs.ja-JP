---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: af3bb08b5a35275970f92aafb7a4e10d97ffc697
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35713080"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/domains/contoso.com')
    .version('beta')
    .delete();

```