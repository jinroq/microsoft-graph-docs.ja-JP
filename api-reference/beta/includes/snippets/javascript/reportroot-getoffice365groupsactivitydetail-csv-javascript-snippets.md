---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 8141bebcf8ef89c3a33cb6aa5026ede1844fe2fa
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35719402"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getOffice365GroupsActivityDetail(period='D7')')
    .version('beta')
    .get();

```