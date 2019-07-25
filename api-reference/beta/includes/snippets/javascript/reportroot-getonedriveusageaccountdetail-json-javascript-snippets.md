---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 11cde529aaa743e5e21e988cd85a695a314cdb6a
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35727195"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getOneDriveUsageAccountDetail(period='D7')')
    .version('beta')
    .get();

```