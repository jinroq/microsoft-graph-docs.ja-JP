---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 42065907c79dc236739bc60e80781173d06bad8b
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34478385"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const directoryObject = {
  directoryObject: {
  }
};

let res = await client.api('/devices/{id}/registeredUsers')
    .post({directoryObject : directoryObject});

```