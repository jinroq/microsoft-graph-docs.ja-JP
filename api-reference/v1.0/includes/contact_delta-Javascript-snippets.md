---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 2cd945556cf542085a742ecd641a5ed8a79277db
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34467038"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/contactFolders/{id}/contacts/delta')
    .header('Prefer','odata.maxpagesize=2')
    .select('displayName')
    .get();

```