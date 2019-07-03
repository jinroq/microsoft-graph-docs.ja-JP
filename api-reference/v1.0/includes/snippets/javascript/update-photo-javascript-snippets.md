---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: fadb8821c1009fedf629dc391e973d94f6ee8c76
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35514317"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const profilePhoto = {
  height: 99,
  width: 99,
  id: "id-value"
};

let res = await client.api('/users/{id|userPrincipalName}/photo')
    .update({profilePhoto : profilePhoto});

```