---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 0363adf0e351f521aed0e0e447d91cc2826e1b2c
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35527621"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const calendar = {
  name: "Volunteer"
};

let res = await client.api('/me/calendars')
    .version('beta')
    .post({calendar : calendar});

```