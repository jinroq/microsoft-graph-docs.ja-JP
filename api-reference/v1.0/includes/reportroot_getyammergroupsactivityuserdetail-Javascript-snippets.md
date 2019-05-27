---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: dbdca17511e8b2bca5c4cc69825f8db8e1dd7595
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34440535"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getYammerGroupsActivityDetail(period='D7')')
    .get();

```