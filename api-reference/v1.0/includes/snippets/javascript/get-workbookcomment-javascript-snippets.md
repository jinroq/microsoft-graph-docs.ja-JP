---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: b2b1cacc6d897e4b97e1a495a6ead644a06b2ecd
ms.sourcegitcommit: d8a58221ed1f2b7b7073fd621da4737e11ba53c5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/11/2019
ms.locfileid: "36839157"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/drive/root/workbook/comments/{id}')
    .get();

```