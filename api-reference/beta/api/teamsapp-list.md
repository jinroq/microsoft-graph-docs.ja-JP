---
title: マイクロソフト チーム アプリケーション カタログから公開されているアプリケーションを一覧表示します。
description: 'マイクロソフト チーム アプリケーション カタログからアプリケーションを一覧表示します。 '
author: nkramer
ms.openlocfilehash: 77867d5b75721fcb169da6ad6a8ff39c46de196e
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27326468"
---
# <a name="list-the-published-apps-from-the-microsoft-teams-app-catalog"></a>マイクロソフト チーム アプリケーション カタログから公開されているアプリケーションを一覧表示します。

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

マイクロソフト チーム アプリケーション カタログから[アプリケーション](../resources/teamsapp.md)を一覧表示します。 これには、組織のアプリケーション カタログ (テナント アプリケーション カタログ) からアプリケーションと同様に、マイクロソフトのチーム ・ ストアからのアプリが含まれます。 組織のアプリケーションのカタログのみからアプリケーションを取得するのには次のように指定します。 `Organization` [teamsCatalogApp](../resources/teamsapp.md)リソースで**distributionMethod**とします。

## <a name="permissions"></a>アクセス許可

この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](https://developer.microsoft.com/graph/docs/concepts/permissions_reference)」を参照してください。

>**注:** グローバル管理者だけでは、この API を呼び出すことができます。 

| アクセス許可の種類                        | アクセス許可 (特権の小さいものから大きいものへ)|
|:----------------------------------     |:-------------|
| 委任 (職場または学校のアカウント)     | AppCatalog.ReadWrite.All |
| 委任 (個人用 Microsoft アカウント) | サポートされていません|
| アプリケーション                            | 非サポート|

## <a name="http-request"></a>HTTP 要求
<!-- { "blockType": "ignored" } -->
```http
GET /appCatalogs/teamsApps
```

## <a name="optional-query-parameters"></a>オプションのクエリ パラメーター
このメソッドは、$filter、$select をサポートしていて、$ は、応答をカスタマイズするために[OData クエリ パラメーター](/graph/query-parameters)を展開します。

## <a name="request-headers"></a>要求ヘッダー

| ヘッダー        | 値           |
|:--------------|:--------------  |
| Authorization | ベアラー {トークン}。必須。  |

## <a name="request-body"></a>要求本文
なし。

>**注:** 任意の結果の一覧を短縮するための[teamsCatalogApp](../resources/teamsapp.md)オブジェクトのフィールドをフィルターできます。 次のフィルター操作のいずれかを使用することができます: 等しい、等しくない、またはではなく。

## <a name="response"></a>応答
かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文内の[teamsCatalogApp](../resources/teamsapp.md)オブジェクトの一覧です。

## <a name="examples"></a>例
### <a name="example-1"></a>例 1
次の例では、テナントに固有のすべてのアプリケーションが一覧表示されます。

#### <a name="request"></a>要求
```
GET https://graph.microsoft.com/beta/appCatalogs/teamsApps?$filter=distributionMethod eq 'organization'
```

#### <a name="response"></a>応答
```
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "b1c5353a-7aca-41b3-830f-27d5218fe0e5",
      "externalId": "f31b1263-ba99-435a-a679-911d24850d7c",
      "name": "Test App",
      "version": "1.0.1",
      "distributionMethod":"Organization"
    }
  ]
}
```

### <a name="example-2"></a>例 2

次の使用例は指定された ID を使用してアプリケーションを一覧表示します。

#### <a name="request"></a>要求
```
GET https://graph.microsoft.com/beta/appCatalogs/teamsApps?$filter=id%20eq%20'b1c5353a-7aca-41b3-830f-27d5218fe0e5'
```

#### <a name="response"></a>応答
```
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "b1c5353a-7aca-41b3-830f-27d5218fe0e5",
      "externalId": "f31b1263-ba99-435a-a679-911d24850d7c",
      "name": "Test App",
      "version": "1.0.1",
      "distributionMethod":"Organization"
    }
  ]
}
```

