---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: baec57142e0f460e1801b6969163874f0e326e5c
ms.sourcegitcommit: 56c0b609dfb1bc5d900956f407d107cdab7086e8
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/30/2019
ms.locfileid: "35932839"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/drive/bundles?filter=bundle/album%20ne%20null')
    .version('beta')
    .filter('bundle/album ne null')
    .get();

```