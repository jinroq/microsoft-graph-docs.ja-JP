---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 7fb25fdf35d5c90368acae26844468dffbc05881
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/27/2019
ms.locfileid: "36637878"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const timeOffReason = {
  displayName: "Vacation",
  iconType: "plane",
  isActive: true
};

let res = await client.api('/teams/{teamId}/schedule/timeOffReasons/{timeOffReasonId}')
    .version('beta')
    .put(timeOffReason);

```