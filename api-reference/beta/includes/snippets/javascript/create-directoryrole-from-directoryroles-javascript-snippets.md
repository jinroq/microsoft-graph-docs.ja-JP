---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 6cf0afcd82be742971e9e64a7449365d86ddf4b7
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/27/2019
ms.locfileid: "36637800"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const directoryRole = {
  description: "description-value",
  displayName: "displayName-value",
  roleTemplateId: "roleTemplateId-value"
};

let res = await client.api('/directoryRoles')
    .version('beta')
    .post(directoryRole);

```