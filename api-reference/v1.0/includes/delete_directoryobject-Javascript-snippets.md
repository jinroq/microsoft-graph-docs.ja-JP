---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 5be5741b63ac25fcd298bfc1cd9613147a75b842
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34459294"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/directoryObjects/{id}')
    .delete();

```