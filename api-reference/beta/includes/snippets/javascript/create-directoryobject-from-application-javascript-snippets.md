---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 599544c41109e7013e96661e372e6edd367074b4
ms.sourcegitcommit: 56c0b609dfb1bc5d900956f407d107cdab7086e8
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/30/2019
ms.locfileid: "35930450"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const directoryObject = {
@odata.id: "https://graph.microsoft.com/beta/directoryObjects/{id}"
};

let res = await client.api('/applications/{id}/owners/$ref')
    .version('beta')
    .post({directoryObject : directoryObject});

```