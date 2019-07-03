---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: a9863db4e3c60bd7aaa90679e2bae7ebe6bc05ab
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35485411"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getTeamsDeviceUsageUserDetail(period='D7')')
    .version('beta')
    .get();

```