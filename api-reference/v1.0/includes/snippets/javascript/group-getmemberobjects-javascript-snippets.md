---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 0f559bdc28bd55166cfe984f65ed867547a0dd59
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35732424"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const String = {
  securityEnabledOnly: false
};

let res = await client.api('/groups/{id}/getMemberObjects')
    .post(String);

```