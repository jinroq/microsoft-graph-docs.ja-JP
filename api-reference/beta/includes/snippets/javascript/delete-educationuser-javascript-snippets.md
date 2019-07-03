---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 6c58804f8215d3d90dfc528d22d554e5c819f12e
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35526549"
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