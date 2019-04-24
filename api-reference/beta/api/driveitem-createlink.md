---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: ファイルをリンクで共有する
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 3f119ea285b3fa9e59ec8c67d5a7b3fd304fd196
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32454583"
---
# <a name="create-a-sharing-link-for-a-driveitem"></a>DriveItem の共有リンクを作成する

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**createLink** アクションを使用して、共有リンクを使って [DriveItem](../resources/driveitem.md) を共有できます。

**createLink** アクションは、呼び出し元のアプリケーションに指定されたリンクの種類が存在しない場合に、新しい共有リンクを作成します。指定された種類の共有リンクがアプリで既に存在している場合、既存の共有リンクが返されます。

DriveItem リソースは、そのリソースの先祖から共有アクセス許可を継承します。

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
POST /drives/{driveId}/items/{itemId}/createLink
POST /groups/{groupId}/drive/items/{itemId}/createLink
POST /me/drive/items/{itemId}/createLink
POST /sites/{siteId}/drive/items/{itemId}/createLink
POST /users/{userId}/drive/items/{itemId}/createLink
```

### <a name="request-body"></a>要求本文

要求本文はアプリケーションが要求する共有リンクのプロパティを定義します。
要求は、次のプロパティを含む JSON オブジェクトである必要があります。

|   名前    |  型  |                                 説明                                  |
| :-------- | :----- | :--------------------------------------------------------------------------- |
| **type**  | string | 作成する共有リンクの種類。`view`、`edit`、または `embed` です。       |
| **scope** | string | 省略可能。 作成するリンクのスコープ。 `anonymous` または `organization` のどちらかです。 |


### <a name="link-types"></a>リンクの種類

**type** パラメーターには次の値を使用できます。

| 種類の値 | 説明                                                                                  |
|:-----------|:---------------------------------------------------------------------------------------------|
| `view`     | その DriveItem への読み取り専用リンクを作成します。                                                        |
| `edit`     | その DriveItem への読み取り/書き込みリンクを作成します。                                                       |
| `embed`    | その DriveItem への埋め込み可能なリンクを作成します。 このオプションは OneDrive 個人用のファイルでのみ選択可能です。 |

### <a name="scope-types"></a>スコープの種類

**scope** パラメーターには次の値を使用できます。
**scope** パラメーターが指定されていない場合、組織の既定のリンクの種類が作成されます。

| 種類の値     | 説明                                                                                                                   |
|:---------------|:------------------------------------------------------------------------------------------------------------------------------|
| `anonymous`    | DriveItem への、すべてのユーザーがアクセス可能なリンクを作成します。 匿名リンクは管理者により無効にされることがあります。                 |
| `organization` | DriveItem への、ユーザーの組織内のだれでもアクセス可能なリンクを作成します。 組織のリンク スコープは、OneDrive 個人用では使用できません。 |

## <a name="response"></a>応答

正常に実行されると、このメソッドは要求された共有アクセス許可を表す応答本文で、単一の[アクセス許可](../resources/permission.md)リソースを返します。

応答は、アイテムに新しい共有リンクが作成される場合は `201 Created`、既存のリンクが返される場合は `200 OK` となります。

## <a name="example"></a>例

次の例では、ユーザーの OneDrive の {itemId} で指定された DriveItem に対して共有リンクを作成することを要求します。
共有リンクは、読み取り専用でそのリンクによってだれでも使用可能になるよう構成されます。

### <a name="request"></a>要求

<!-- {
  "blockType": "request",
  "name": "item_createlink"
}-->

```http
POST /me/drive/items/{itemId}/createLink
Content-type: application/json

{
  "type": "view",
  "scope": "anonymous"
}
```

### <a name="response"></a>応答

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.permission" } -->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "123ABC",
  "roles": ["write"],
  "link": {
    "type": "view",
    "scope": "anonymous",
    "webUrl": "https://1drv.ms/A6913278E564460AA616C71B28AD6EB6",
    "application": {
      "id": "1234",
      "displayName": "Sample Application"
    },
  }
}
```

## <a name="creating-company-sharable-links"></a>会社の共有可能リンクを作成する

OneDrive for Business および SharePoint は、会社の共有可能リンクをサポートしています。
これらは匿名リンクに似ていますが、所有組織のメンバーだけが使用できる点が異なります。
会社の共有可能リンクを作成するには、**scope** パラメーターで値 `organization` を指定して使用します。

### <a name="request"></a>要求

<!-- { "blockType": "request", "name": "create-link-scoped", "scopes": "files.readwrite service.sharepoint" } -->

```http
POST /me/drive/items/{item-id}/createLink
Content-Type: application/json

{
  "type": "edit",
  "scope": "organization"
}
```

### <a name="response"></a>応答

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.permission" } -->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "123ABC",
  "roles": ["write"],
  "link": {
    "type": "edit",
    "scope": "organization",
    "webUrl": "https://contoso-my.sharepoint.com/personal/ellen_contoso_com/...",
    "application": {
      "id": "1234",
      "displayName": "Sample Application"
    },
  }
}
```

## <a name="creating-embeddable-links"></a>埋め込み可能なリンクを作成する

リンクの種類で `embed` を使用する場合、返される webUrl は `<iframe>` HTML 要素に埋め込むことができます。埋め込みリンクが作成されると、`webHtml` プロパティに `<iframe>` がコンテンツをホストするための HTML コードが含まれます。

**注:** 埋め込みリンクは、OneDrive 個人用でのみサポートされます。

### <a name="request"></a>要求

<!-- { "blockType": "request", "name": "create-embedded-link", "scopes": "files.readwrite service.onedrive" } -->

```http
POST /me/drive/items/{item-id}/createLink
Content-Type: application/json

{
  "type": "embed"
}
```

### <a name="response"></a>応答

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.permission" } -->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "123ABC",
  "roles": ["read"],
  "link": {
    "type": "embed",
    "webHtml": "<IFRAME src=\"https://onedrive.live.com/...\"></IFRAME>",
    "webUrl": "https://onedive.live.com/...",
    "application": {
      "id": "1234",
      "displayName": "Sample Application"
    },
  }
}
```

## <a name="remarks"></a>注釈

* 組織に既定の有効期限ポリシーが適用されている場合を除き、このアクションを使用して作成されたリンクに期限はありません。
* リンクはそのアイテムの共有アクセス許可に表示され、アイテムの所有者はそれを削除できます。
* リンクは、そのアイテムがチェックアウトされない限り、常にアイテムの現在のバージョンをポイントします (SharePoint の場合のみ)。

<!--
{
  "type": "#page.annotation",
  "description": "Create a new sharing link for an item.",
  "keywords": "create,sharing,sharing link",
  "section": "documentation",
  "tocPath": "Sharing/Create link",
  "suppressions": [
    "Error: /api-reference/beta/api/driveitem-createlink.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
