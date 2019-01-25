---
title: privilegedOperationEvent リソースの種類
description: 監査イベントによって生成される特権 Id 管理の役割の操作など、管理者特権を持つロールを管理する、ユーザーが自分の役割を有効にユーザーが自分のロールを非アクティブ化を表します。
localization_priority: Normal
ms.openlocfilehash: 2ad8f7e5db956dfbb2fa0d74f441b01f2b5d68aa
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29525592"
---
# <a name="privilegedoperationevent-resource-type"></a>privilegedOperationEvent リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

監査イベントによって生成される特権 Id 管理の役割の操作など、管理者特権を持つロールを管理する、ユーザーが自分の役割を有効にユーザーが自分のロールを非アクティブ化を表します。


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[リスト privilegedOperationEvent](../api/privilegedoperationevent-list.md) | [privilegedOperationEvent](privilegedoperationevent.md)コレクションです。 |PrivilegedOperationEvent オブジェクトのコレクションを取得します。|

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|について|string|詳細情報イベントです。|
|creationDateTime|dateTimeOffset|イベントが作成されたときの時刻を示します。|
|expirationDateTime|dateTimeOffset|修飾子の一覧は、「Activate」、およびロールのアクティブ化の有効期限を示します場合にのみ使用されます。|
|id|string|PrivilegedOperationEvent の一意の識別子です。 読み取り専用です。|
|referenceKey|string|ロールのアクティブ化中に問題と要求のチケット番号です。 ロールのアクティブ化時にチケット番号を指定した場合にのみ値が表示されます。|
|referenceSystem|string|チケット tole のライセンス認証中に提供されたシステム要求問題です。 ロールのアクティブ化時にチケット システムが用意されている場合にのみ値が表示されます。|
|RequestType|string|要求された操作の種類です。 修飾子の一覧を指定できます: ```Assign``` (ロールの割り当て)、 ```Activate``` (ロールのアクティブ化)、 ```Unassign``` (ロールの割り当てを削除する)、 ```Deactivate``` (ロールの無効化)、 ```ScanAlersNow``` (セキュリティの警告をスキャンする)、 ```DismissAlert``` (セキュリティの警告を無視する)、 ```FixAlertItem``` (セキュリティの修正アラートの問題)、 ```AccessReview_Review``` (確認のアクセスを確認する)、 ```AccessReview_Create``` (、アクセス確認を作成する) ```AccessReview_Update``` (更新のアクセスを確認する)、および```AccessReview_Delete```(削除、アクセスを確認)。|
|requestorId|string|操作を開始した要求元のユーザー id です。|
|requestorName|string|操作を開始した要求元のユーザー名です。|
|roleId|string|操作に関連付けられているロールの id です。|
|役割名|string|ロールの名前です。|
|tenant_id|string|テナント (組織) の id です。|
|userId|string|操作に関連付けられているユーザーの id です。|
|userMail|string|ユーザーの電子メール。|
|userName|string|ユーザーの表示名。|

## <a name="relationships"></a>リレーションシップ
なし


## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.privilegedOperationEvent"
}-->

```json
{
  "additionalInformation": "string",
  "creationDateTime": "String (timestamp)",
  "expirationDateTime": "String (timestamp)",
  "id": "string (identifier)",
  "requestType": "string",
  "requestorId": "string",
  "requestorName": "string",
  "roleId": "string",
  "roleName": "string",
  "tenantId": "string",
  "userId": "string",
  "userMail": "string",
  "userName": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "privilegedOperationEvent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/privilegedoperationevent.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
