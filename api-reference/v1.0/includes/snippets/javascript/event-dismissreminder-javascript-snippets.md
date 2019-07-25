---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: ad4cb296e95947f0081d7c77059ab85e7a13cea1
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35732606"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/events/{id}/dismissReminder')
    .post();

```