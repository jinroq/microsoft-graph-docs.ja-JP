---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 396fee202c9d61260f8c73a0cd833b9856fed7da
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34459794"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/identityProviders/Amazon-OAuth')
    .delete();

```