---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: a9e6a966a8cf722631f5e472fce6f3f45a5f198f
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34469819"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/calendar')
    .get();

```