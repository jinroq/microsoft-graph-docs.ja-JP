---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 5c5cbb57b66927d9b4246e3303bd3a76218be5e8
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35472522"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getYammerActivityCounts(period='D7')')
    .get();

```