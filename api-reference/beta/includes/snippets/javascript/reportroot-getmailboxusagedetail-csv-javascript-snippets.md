---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 2dd336e96f309110a8a1aae4eb7a5b58035b30d7
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35485375"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getMailboxUsageDetail(period='D7')')
    .version('beta')
    .get();

```