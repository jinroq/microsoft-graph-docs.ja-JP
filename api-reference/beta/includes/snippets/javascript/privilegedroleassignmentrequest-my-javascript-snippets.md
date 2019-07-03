---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: a1bd8b70883aefeae797752f6c2b31e0f37e8d22
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35464416"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/privilegedRoleAssignmentRequests/my')
    .version('beta')
    .get();

```