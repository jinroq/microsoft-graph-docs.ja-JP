---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 95aa02f03dba39d669e1f75c245f3edff4b6b8f1
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35715155"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const String = {
  groupIds: [
    "groupIds-value"
  ]
};

let res = await client.api('/me/checkMemberGroups')
    .post(String);

```