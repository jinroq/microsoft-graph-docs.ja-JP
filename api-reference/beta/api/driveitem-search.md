---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: ファイルを検索する
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 13e33a66cb2e32702d2afd1205959fd19477ead1
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33325385"
---
# <a name="search-for-a-driveitems-within-a-drive"></a><span data-ttu-id="9e31a-102">ドライブ内の DriveItems を検索する</span><span class="sxs-lookup"><span data-stu-id="9e31a-102">Search for a DriveItems within a drive</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9e31a-103">クエリと一致するアイテムを対象にアイテムの階層を検索します。</span><span class="sxs-lookup"><span data-stu-id="9e31a-103">Search the hierarchy of items for items matching a query.</span></span>
<span data-ttu-id="9e31a-104">フォルダー階層内、ドライブ全体、現在のユーザーと共有されるファイル内で検索できます。</span><span class="sxs-lookup"><span data-stu-id="9e31a-104">You can search within a folder hierarchy, a whole drive, or files shared with the current user.</span></span>

## <a name="permissions"></a><span data-ttu-id="9e31a-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="9e31a-105">Permissions</span></span>

<span data-ttu-id="9e31a-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9e31a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9e31a-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9e31a-108">Permission type</span></span>      | <span data-ttu-id="9e31a-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="9e31a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9e31a-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9e31a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9e31a-111">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9e31a-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="9e31a-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9e31a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9e31a-113">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9e31a-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="9e31a-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9e31a-114">Application</span></span> | <span data-ttu-id="9e31a-115">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9e31a-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9e31a-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9e31a-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/root/search(q='{search-text}')
GET /groups/{group-id}/drive/root/search(q='{search-text}')
GET /me/drive/root/search(q='{search-text}')
GET /sites/{site-id}/drive/root/search(q='{search-text}')
GET /users/{user-id}/drive/root/search(q='{search-text}')
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9e31a-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="9e31a-117">Optional query parameters</span></span>

<span data-ttu-id="9e31a-118">このメソッドは、応答をカスタマイズするための `$expand`、`$select`、`$skipToken`、`$top`、`$orderby` の [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="9e31a-118">This method supports the `$expand`, `$select`, `$skipToken`, `$top`, and `$orderby` [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="function-parameters"></a><span data-ttu-id="9e31a-119">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="9e31a-119">Function parameters</span></span>

| <span data-ttu-id="9e31a-120">パラメーター</span><span class="sxs-lookup"><span data-stu-id="9e31a-120">Parameter</span></span> | <span data-ttu-id="9e31a-121">型</span><span class="sxs-lookup"><span data-stu-id="9e31a-121">Type</span></span>  | <span data-ttu-id="9e31a-122">説明</span><span class="sxs-lookup"><span data-stu-id="9e31a-122">Description</span></span>                                                                                                                          |
|:-----|:-------|:-------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="9e31a-123">q</span><span class="sxs-lookup"><span data-stu-id="9e31a-123">q</span></span>  | <span data-ttu-id="9e31a-124">string</span><span class="sxs-lookup"><span data-stu-id="9e31a-124">string</span></span> | <span data-ttu-id="9e31a-p103">アイテムの検索に使用するクエリ テキスト。値は、ファイル名、メタデータ、およびファイルのコンテンツを含む複数のフィールドに渡って照合できます。</span><span class="sxs-lookup"><span data-stu-id="9e31a-p103">The query text used to search for items. Values may be matched across several fields including filename, metadata, and file content.</span></span> |

## <a name="example"></a><span data-ttu-id="9e31a-127">例</span><span class="sxs-lookup"><span data-stu-id="9e31a-127">Example</span></span>

### <a name="request"></a><span data-ttu-id="9e31a-128">要求</span><span class="sxs-lookup"><span data-stu-id="9e31a-128">Request</span></span>

<span data-ttu-id="9e31a-129">ここでは、現在のユーザーの OneDrive を検索する要求の例を示します。</span><span class="sxs-lookup"><span data-stu-id="9e31a-129">Here is an example of the request searching the current user's OneDrive</span></span>

<!-- { "blockType": "request", "name": "item_search" }-->

```http
GET /me/drive/root/search(q='{search-query}')
```

### <a name="response"></a><span data-ttu-id="9e31a-130">応答</span><span class="sxs-lookup"><span data-stu-id="9e31a-130">Response</span></span>

<span data-ttu-id="9e31a-p104">このメソッドは、検索条件に一致する [DriveItems](../resources/driveitem.md) のコレクション含んでいるオブジェクトを返します。アイテムが見つからない場合は、空のコレクションが返されます。</span><span class="sxs-lookup"><span data-stu-id="9e31a-p104">This method returns an object containing an collection of [DriveItems](../resources/driveitem.md) that match the search criteria. If no items were found, an empty collection is returned.</span></span>

<span data-ttu-id="9e31a-p105">一致が多すぎる場合は、応答はページ化され、**@odata.nextLink** プロパティには、後続の結果ページへの URL が含まれます。`$top` クエリ パラメーターを使用すると、ページ内のアイテム数を指定できます。</span><span class="sxs-lookup"><span data-stu-id="9e31a-p105">If there are too many matches the response will be paged and an **@odata.nextLink** property will contain a URL to the next page of results. You can use the `$top` query parameter to specify the number of items in the page.</span></span>

<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.driveItem)", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
      {
        "id": "0123456789abc!123",
        "name": "Contoso Project",
        "folder": {},
        "searchResult": { "onClickTelemetryUrl": "https://bing.com/0123456789abc!123" }
      },
      {
        "id": "0123456789abc!456",
        "name": "Contoso Project 2016",
        "folder": {},
        "searchResult": { "onClickTelemetryUrl": "https://bing.com/0123456789abc!456" }
      }
    ],
    "@odata.nextLink": "https://graph.microsoft.com/v1.0/me/drive/root/search(query='contoso project')&skipToken=1asdlnjnkj1nalkm!asd"
}
```

## <a name="searching-for-items-a-user-can-access"></a><span data-ttu-id="9e31a-135">ユーザーがアクセスできるアイテムの検索</span><span class="sxs-lookup"><span data-stu-id="9e31a-135">Searching for items a user can access</span></span>

<span data-ttu-id="9e31a-p106">ドライブ内のアイテムの検索に加えて、アプリでは現在のユーザーと共有されるアイテムを含めるように、検索範囲を広げることができます。検索範囲を広げるには、[Drive](../resources/drive.md) リソースの **search** メソッドを使用します。</span><span class="sxs-lookup"><span data-stu-id="9e31a-p106">In addition to searching for items within a drive, your app can search more broadly to include items shared with the current user. To broaden the search scope, use the **search** method on the [Drive](../resources/drive.md) resource.</span></span>

### <a name="example"></a><span data-ttu-id="9e31a-138">例</span><span class="sxs-lookup"><span data-stu-id="9e31a-138">Example</span></span>

<!-- { "blockType": "request", "name": "item_search_all" }-->

```http
GET /me/drive/search(q='{search-query}')
```

### <a name="response"></a><span data-ttu-id="9e31a-139">応答</span><span class="sxs-lookup"><span data-stu-id="9e31a-139">Response</span></span>

<span data-ttu-id="9e31a-p107">**ドライブ** リソースからの検索時の応答には、ドライブの外部のアイテム (現在のユーザーと共有されているアイテム) が含まれていることがあります。こうしたアイテムには、それらが対象のドライブの外部に保存されていることを示す、[**remoteItem**](../resources/remoteitem.md) ファセットが含まれます。</span><span class="sxs-lookup"><span data-stu-id="9e31a-p107">Responses when searching from the **drive** resource may include items outside of the drive (items shared with the current user). These items will include the [**remoteItem**](../resources/remoteitem.md) facet to indicate they are stored outside of the target drive.</span></span> 

<!-- { "blockType": "response", "truncated": true, "@odata.type": "Collection(microsoft.graph.driveItem)" } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
      {
        "id": "0123456789abc!123",
        "name": "Contoso Project",
        "folder": {},
        "searchResult": { "onClickTelemetryUrl": "https://bing.com/0123456789abc!123" },
        "remoteItem": { "id": "!23141901", "driveId": "s!1020101jlkjl12lx" }
      },
      {
        "id": "0123456789abc!456",
        "name": "Contoso Project 2016",
        "folder": {},
        "searchResult": { "onClickTelemetryUrl": "https://bing.com/0123456789abc!456" }
      }
    ],
    "@odata.nextLink": "https://graph.microsoft.com/v1.0/me/drive/root/search(query='contoso project')&skipToken=1asdlnjnkj1nalkm!asd"
}
```

## <a name="error-responses"></a><span data-ttu-id="9e31a-142">エラー応答</span><span class="sxs-lookup"><span data-stu-id="9e31a-142">Error responses</span></span>

<span data-ttu-id="9e31a-143">エラーがどのように返されるかについては、「[エラー応答][error-response]」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9e31a-143">See [Error Responses][error-response] for more information about how errors are returned.</span></span>

[error-response]: /graph/errors
[item-resource]: ../resources/driveitem.md
[odata-query-parameters]: /graph/query-parameters

<!--
{
  "type": "#page.annotation",
  "description": "Search for a file across a OneDrive.",
  "keywords": "search,query,bing,filename,content",
  "section": "documentation",
  "tocPath": "Items/Search",
  "suppressions": []
}
-->
