---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 99c6bdfa3d816653da885e95fbf56a68c0ba25d7
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/27/2019
ms.locfileid: "36637834"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const calendar = {
  name: "Social events"
};

let res = await client.api('/me/calendar')
    .version('beta')
    .update(calendar);

```