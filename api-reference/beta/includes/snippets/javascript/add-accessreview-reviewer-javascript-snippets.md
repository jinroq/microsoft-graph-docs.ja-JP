---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: de90a74b56be163689a7e492c3b8a7a6f26d935e
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35711179"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const accessReviewReviewer = {
    id:"006111db-0810-4494-a6df-904d368bd81b"
};

let res = await client.api('/accessReviews/2b83cc42-09db-46f6-8c6e-16fec466a82d/reviewers')
    .version('beta')
    .post({accessReviewReviewer : accessReviewReviewer});

```