---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 6cb6f3a5536be484e8d0ede0f89c8bacfd1b9ecb
ms.sourcegitcommit: f50b1feff72182d1e19bfa346304beaf29558b68
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/19/2019
ms.locfileid: "36461411"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/roleManagement/directory/roleAssignments')
    .version('beta')
    .filter('principalId eq 'a98eb769-7bd4-4489-86f6-ad96e1d58b62'')
    .get();

```