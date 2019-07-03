---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 5e72c61ae60ac6a69bc28309855f8cd914008220
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35496023"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/joinedTeams')
    .get();

```