---
title: Microsoft Teams アプリカタログから発行されたアプリを一覧表示する
description: 'Microsoft Teams アプリカタログのアプリを一覧表示します。 '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 1e4d9348cbb28ed0daf1ec48459378935d78e0a2
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32544681"
---
# <a name="list-the-published-apps-from-the-microsoft-teams-app-catalog"></a>Microsoft Teams アプリカタログから発行されたアプリを一覧表示する

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Microsoft Teams アプリカタログの[アプリ](../resources/teamsapp.md)を一覧表示します。
これには、Microsoft Teams ストアからのアプリや、組織のアプリカタログ (テナントのアプリカタログ) からのアプリが含まれます。 組織のアプリカタログからアプリのみを取得するには`Organization` 、 [teamsCatalogApp](../resources/teamsapp.md)リソースの "の" として、を指定します。 ****

## <a name="permissions"></a>アクセス許可

この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions_reference)」を参照してください。

> **注:** この API は、グローバル管理者のみが呼び出すことができます。

| アクセス許可の種類                        | アクセス許可 (特権の小さいものから大きいものへ) |
|:---------------------------------------|:------------------------------------|
| 委任 (職場または学校のアカウント)     | AppCatalog.ReadWrite.All            |
| 委任 (個人用 Microsoft アカウント) | サポートされていません                       |
| アプリケーション                            | 非サポート                       |

## <a name="http-request"></a>HTTP 要求

<!-- { "blockType": "ignored" } -->

```http
GET /appCatalogs/teamsApps
```

## <a name="optional-query-parameters"></a>オプションのクエリ パラメーター

このメソッドは、応答をカスタマイズするための $filter、$select、および $expand [OData クエリ パラメーター](/graph/query-parameters)をサポートします。

## <a name="request-headers"></a>要求ヘッダー

| ヘッダー        | 値                     |
|:--------------|:--------------------------|
| Authorization | ベアラー {トークン}。必須。 |

## <a name="request-body"></a>要求本文

なし。

> **注:**[teamsCatalogApp](../resources/teamsapp.md)オブジェクトの任意のフィールドでフィルター処理して、結果の一覧を短縮できます。 次のいずれかのフィルター操作を使用できます: equal、not equal、and、or not。

## <a name="response"></a>応答

成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[teamsCatalogApp](../resources/teamsapp.md)オブジェクトのリストを返します。

## <a name="examples"></a>例

### <a name="example-1-list-all-applications"></a>例 1: すべてのアプリケーションを一覧表示する

次の例では、テナント固有のすべてのアプリケーションを一覧表示します。

#### <a name="request"></a>要求

```http
GET https://graph.microsoft.com/beta/appCatalogs/teamsApps?$filter=distributionMethod eq 'organization'
```

<!-- markdownlint-disable MD024 -->

#### <a name="response"></a>応答

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "b1c5353a-7aca-41b3-830f-27d5218fe0e5",
      "externalId": "f31b1263-ba99-435a-a679-911d24850d7c",
      "name": "Test App",
      "version": "1.0.1",
      "distributionMethod": "Organization"
    }
  ]
}
```

### <a name="example-2-list-applications-with-a-given-id"></a>例 2: 指定された ID を持つアプリケーションを一覧表示する

次の例では、指定された ID を持つアプリケーションを一覧表示します。

#### <a name="request"></a>要求

```http
GET https://graph.microsoft.com/beta/appCatalogs/teamsApps?$filter=id%20eq%20'b1c5353a-7aca-41b3-830f-27d5218fe0e5'
```

#### <a name="response"></a>応答

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "b1c5353a-7aca-41b3-830f-27d5218fe0e5",
      "externalId": "f31b1263-ba99-435a-a679-911d24850d7c",
      "name": "Test App",
      "version": "1.0.1",
      "distributionMethod": "Organization"
    }
  ]
}
```

<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/teamsapp-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
