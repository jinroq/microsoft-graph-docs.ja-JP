---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: ファイルまたはフォルダーをコピーする
localization_priority: Normal
ms.openlocfilehash: 8289bd3c15575e1469fe18baf45c6c2f937ed2dd
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27879444"
---
# <a name="copy-a-driveitem"></a>DriveItem をコピーする

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

新しい親アイテムの下に、または新しい名前を指定して、[driveItem][item-resource] (すべての子を含む) のコピーを非同期に作成します。

## <a name="permissions"></a>アクセス許可

この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類      | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) | Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All    |
|委任 (個人用 Microsoft アカウント) | Files.ReadWrite、Files.ReadWrite.All    |
|アプリケーション | Files.ReadWrite.All、Sites.ReadWrite.All |

## <a name="http-request"></a>HTTP 要求

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/copy
POST /groups/{groupId}/drive/items/{itemId}/copy
POST /me/drive/items/{item-id}/copy
POST /sites/{siteId}/drive/items/{itemId}/copy
POST /users/{userId}/drive/items/{itemId}/copy
```

### <a name="request-body"></a>要求本文

要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。


| 名前            | 値                                          | 説明                                                                                                 |
|:----------------|:-----------------------------------------------|:------------------------------------------------------------------------------------------------------------|
| parentReference | [ItemReference](../resources/itemreference.md) | 省略可能。コピーが作成される親アイテムへの参照。                                         |
| name            | 文字列                                         | 省略可能。コピーの新しい名前。これを指定しない場合は、元の名前と同じ名前が使用されます。    |

**注:** _parentReference_ には、ターゲット フォルダーの `driveId` と `id` パラメーターを含める必要があります。

## <a name="example"></a>例

この例では、`{item-id}` で識別されるファイルを `driveId` および `id` の値で識別されるフォルダーにコピーします。
ファイルの新しいコピーの名前は `contoso plan (copy).txt` になります。

<!-- { "blockType": "request", "name": "copy-item", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /me/drive/items/{item-id}/copy
Content-Type: application/json

{
  "parentReference": {
    "driveId": "6F7D00BF-FC4D-4E62-9769-6AEA81F3A21B",
    "id": "DCD0D3AD-8989-4F23-A5A2-2C086050513F"
  },
  "name": "contoso plan (copy).txt"
}
```

## <a name="response"></a>応答

要求の受け入れ時に、コピーの[進行状況を監視する](/graph/long-running-actions-overview)方法についての詳細を返します。

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 202 Accepted
Location: https://contoso.sharepoint.com/_api/v2.0/monitor/4A3407B5-88FC-4504-8B21-0AABD3412717
```

`Location` ヘッダーの値は、コピー操作の現在の状況を返すサービスの URL を提供します。
この情報を使用して、[コピーがいつ終了したかを判断する](/graph/long-running-actions-overview)ことができます。

### <a name="remarks"></a>備考

多くの場合、コピー操作は非同期で実行されます。API からの応答は、コピー操作が受け入れられたか、コピー先のファイル名が既に使用中のためという理由で拒否されたことのみを示します。

[item-resource]: ../resources/driveitem.md

<!-- {
  "type": "#page.annotation",
  "description": "Create a copy of an existing item.",
  "keywords": "copy existing item",
  "section": "documentation",
  "tocPath": "Items/Copy"
} -->
