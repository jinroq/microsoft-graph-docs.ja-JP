---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: daa172e4dc18e6b9b12cfd178e912e7aecfd667d
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35471260"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const directoryObject = {
  @odata.id: "https://graph.microsoft.com/v1.0/directoryObjects/{id}"
};

let res = await client.api('/directoryRoles/{id}/members/$ref')
    .post({directoryObject : directoryObject});

```