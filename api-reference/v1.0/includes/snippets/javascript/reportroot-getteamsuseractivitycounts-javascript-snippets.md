---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 46d6ac5bafa257a840563c40beb68d4e50c7bcbe
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35471399"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getTeamsUserActivityCounts(period='D7')')
    .get();

```