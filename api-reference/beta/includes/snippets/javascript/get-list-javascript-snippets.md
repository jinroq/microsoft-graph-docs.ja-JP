---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 0780a954208438e9fd60076f510ae345bb825709
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35485020"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/sites/{site-id}/lists/{list-id}')
    .version('beta')
    .get();

```