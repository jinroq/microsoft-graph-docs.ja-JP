---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 08fff3ff7878abe74ec5f504af809a60575a3031
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35472019"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groups')
    .get();

```