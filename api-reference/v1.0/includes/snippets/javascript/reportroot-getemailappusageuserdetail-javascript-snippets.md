---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 861b6a3f6d88f4d62ca54fcbbfc4afac9611c7ac
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35513324"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getEmailAppUsageUserDetail(period='D7')')
    .get();

```