---
title: governancePermission リソースの種類
description: '特定の governanceResource に、governanceSubject を持つアクセス許可を表します。  '
ms.openlocfilehash: d7b3e1eb70c89c278ccc2a8b3e9a16e265e4ae97
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27071072"
---
# <a name="governancepermission-resource-type"></a>governancePermission リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

特定の[governanceResource](../resources/governanceresource.md)に、 [governanceSubject](../resources/governancesubject.md)を持つアクセス許可を表します。  


## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|accessLevel|String|アクセス レベルです。 有効な値: ``None``、 ``UserRead``、``AdminRead``と``AdminReadWrite``。|
|isActive|ブール値|指定する場合、リクエスターが、アクティブなロールの割り当てのアクセス レベルを持ちます。|
|isEligible|ブール値|リクエスターは、対象となるロールの割り当てのアクセス レベルを指定します。|

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

```json
{
  "accessLevel": "String",
  "isActive": true,
  "isEligible": true
}

```