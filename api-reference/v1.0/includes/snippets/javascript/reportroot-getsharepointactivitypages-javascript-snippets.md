---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: f6522b6e897e9d55798349b478bfc08bed3a7051
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35472393"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getSharePointActivityPages(period='D7')')
    .get();

```