---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 870a83db65e5f5b4fb1f92660bf227d347c4cc65
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35717898"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/security/securityActions/{id}/cancelSecurityAction')
    .version('beta')
    .post();

```