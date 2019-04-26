---
title: 同期ジョブを再開します。
description: 同期ジョブを再開して、ディレクトリ内のすべてのオブジェクトを強制的に再処理するようにします。 必要に応じて、既存の同期状態および以前のエラーをクリアします。
localization_priority: Normal
ms.openlocfilehash: 8ef1a4ede6cee7e1ed86e90e329401bcf801e129
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33330424"
---
# <a name="restart-synchronizationjob"></a>同期ジョブを再開します。

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

同期ジョブを再開して、ディレクトリ内のすべてのオブジェクトを強制的に再処理するようにします。 必要に応じて、既存の同期状態および以前のエラーをクリアします。

## <a name="permissions"></a>アクセス許可
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類                        | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント)     |Directory.ReadWrite.All  |
|委任 (個人用 Microsoft アカウント) |サポートされていません。 |
|アプリケーション                            |サポートされていません。  | 

## <a name="http-request"></a>HTTP 要求
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/synchronization/jobs/{jobId}/restart
```

## <a name="request-headers"></a>要求ヘッダー

| 名前           | 型    | 説明|
|:---------------|:--------|:-----------|
| Authorization  | string  | ベアラー {トークン}。必須。 |

## <a name="request-body"></a>要求本文

要求本文で、次のパラメーターを使用して JSON オブジェクトを指定します。

| パラメーター     | 型      | 説明    |
|:--------------|:----------|:---------------|
|criteria       |[synchronizationJobRestartCriteria](../resources/synchronization-synchronizationjobrestartcriteria.md) |再起動の条件|

## <a name="response"></a>応答

成功した場合は`204 No Content` 、応答を返します。 応答本文には何も返されません。

## <a name="example"></a>例

##### <a name="request"></a>要求
要求の例を次に示します。
<!-- {
  "blockType": "request",
  "name": "synchronizationjob_restart"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/restart
Authorization: Bearer <token>
Content-type: application/json

{
   "criteria": {
       "resetScope": "ConnectorDataStore, Escrows, QuarantineState"
   }
}
```

##### <a name="response"></a>応答
応答の例を次に示します。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationJob: restart",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
