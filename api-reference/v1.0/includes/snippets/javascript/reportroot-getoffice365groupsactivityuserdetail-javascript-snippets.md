---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: e83d326662cd5aa86ea0f65d86d9524d0cfde494
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35514390"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getOffice365GroupsActivityDetail(period='D7')')
    .get();

```