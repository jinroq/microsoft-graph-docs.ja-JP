---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: b4791b15b1e80059dab83cddde4903c6671ff633
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34458114"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const directoryObject = {
    ids:["84b80893874940a3-97b7-68513b600544","5d6059b6368d-45f8-91e18e07d485f1d0"],
    types:["user"]
};

let res = await client.api('/directoryObjects/getByIds')
    .post(directoryObject);

```