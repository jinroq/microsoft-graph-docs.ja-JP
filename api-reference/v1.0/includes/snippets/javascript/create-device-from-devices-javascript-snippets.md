---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 95a6ac778661e3ae64195528eba8c3c8f7a5353e
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35715638"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const device = {
  accountEnabled:false,
  alternativeSecurityIds:
  [
    {
      type:2,
      key:"base64Y3YxN2E1MWFlYw=="
    }
  ],
  deviceId:"4c299165-6e8f-4b45-a5ba-c5d250a707ff",
  displayName:"Test device",
  operatingSystem:"linux",
  operatingSystemVersion:"1"
};

let res = await client.api('/devices')
    .post({device : device});

```