---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 6471722119cd53243baf9e2270c11efe2b6ef3aa
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34475759"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getOffice365GroupsActivityStorage(period='D7')')
    .get();

```