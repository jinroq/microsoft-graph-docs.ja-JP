---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: dba67adb7ad3c5923b4fb18d3801d69248c4f478
ms.sourcegitcommit: 56c0b609dfb1bc5d900956f407d107cdab7086e8
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/30/2019
ms.locfileid: "35932874"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/drive/items/{bundle-id}')
    .version('beta')
    .delete();

```