---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 6c58804f8215d3d90dfc528d22d554e5c819f12e
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35714288"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/education/users/13019')
    .version('beta')
    .delete();

```