---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 749155d0b15d0d2e203495ab6e2dc908d1ca80ff
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/27/2019
ms.locfileid: "36637875"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const calendarGroup = {
  name: "name-value",
  classId: "classId-value",
  changeKey: "changeKey-value"
};

let res = await client.api('/me/calendarGroups')
    .version('beta')
    .post(calendarGroup);

```