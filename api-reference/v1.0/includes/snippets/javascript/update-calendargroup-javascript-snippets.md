---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: e0a1372f8f0fecfde1126b49b720dc073a805ed5
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35495779"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const calendarGroup = {
  name: "name-value"
};

let res = await client.api('/me/calendarGroups/{id}')
    .update({calendarGroup : calendarGroup});

```