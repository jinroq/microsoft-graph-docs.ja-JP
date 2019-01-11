---
title: governancePermission リソースの種類
description: '特定の governanceResource に、governanceSubject を持つアクセス許可を表します。  '
localization_priority: Normal
ms.openlocfilehash: e082ca50e5642e865b3e30859eea607df63a03b4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27882874"
---
# <a name="governancepermission-resource-type"></a>governancePermission リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

特定の[governanceResource](../resources/governanceresource.md)に、 [governanceSubject](../resources/governancesubject.md)を持つアクセス許可を表します。  


## <a name="properties"></a>プロパティ
| プロパティ     | 種類   |説明|
|:---------------|:--------|:----------|
|accessLevel|String|アクセス レベルです。 有効な値: ``None``、 ``UserRead``、``AdminRead``と``AdminReadWrite``。|
|isActive|ブール型|指定する場合、リクエスターが、アクティブなロールの割り当てのアクセス レベルを持ちます。|
|isEligible|ブール型|リクエスターは、対象となるロールの割り当てのアクセス レベルを指定します。|

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

```json
{
  "accessLevel": "String",
  "isActive": true,
  "isEligible": true
}

```
