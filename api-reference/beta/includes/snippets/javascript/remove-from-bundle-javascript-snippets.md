---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 422c6d56133a01a2ca49a96980d19503203502a2
ms.sourcegitcommit: 56c0b609dfb1bc5d900956f407d107cdab7086e8
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/30/2019
ms.locfileid: "35932838"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/drive/bundles/{bundle-id}/children/{item-id}')
    .version('beta')
    .delete();

```