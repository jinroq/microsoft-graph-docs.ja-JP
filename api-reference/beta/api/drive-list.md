---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: ドライブを一覧表示する
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: 70b611829c407faf7e7522815232339c3a02af23
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33589710"
---
# <a name="list-available-drives"></a><span data-ttu-id="de82e-102">利用可能なドライブの一覧表示</span><span class="sxs-lookup"><span data-stu-id="de82e-102">List available drives</span></span>

<span data-ttu-id="de82e-103">ターゲットとなる User、Group、または [Site](../resources/site.md) が利用可能な [Drive](../resources/drive.md) リソースの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="de82e-103">Retrieve the list of [Drive](../resources/drive.md) resources available for a target User, Group, or [Site](../resources/site.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="de82e-104">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="de82e-104">Permissions</span></span>

<span data-ttu-id="de82e-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="de82e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="de82e-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="de82e-107">Permission type</span></span>      | <span data-ttu-id="de82e-108">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="de82e-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="de82e-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="de82e-109">Delegated (work or school account)</span></span> | <span data-ttu-id="de82e-110">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="de82e-110">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="de82e-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="de82e-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="de82e-112">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="de82e-112">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="de82e-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="de82e-113">Application</span></span> | <span data-ttu-id="de82e-114">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="de82e-114">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="list-a-groups-drives"></a><span data-ttu-id="de82e-115">グループのドライブを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="de82e-115">List a group's drives</span></span>

<span data-ttu-id="de82e-116">グループのドキュメント ライブラリを一覧表示するために、アプリが Group の **drives** リレーションシップを要求します。</span><span class="sxs-lookup"><span data-stu-id="de82e-116">To list the document libraries for a group, your app requests the **drives** relationship on the Group.</span></span>

### <a name="http-request"></a><span data-ttu-id="de82e-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="de82e-117">HTTP request</span></span>

<!-- {"blockType": "request", "name": "group-list-drives", "scopes": "groups.read.all", "tags": "service.graph" } -->

```http
GET /groups/{groupId}/drives
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="de82e-118">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="de82e-118">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="de82e-119">Visual</span><span class="sxs-lookup"><span data-stu-id="de82e-119">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/group-list-drives-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="de82e-120">Java</span><span class="sxs-lookup"><span data-stu-id="de82e-120">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/group-list-drives-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="list-a-sites-drives"></a><span data-ttu-id="de82e-121">サイトのドライブを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="de82e-121">List a site's drives</span></span>

<span data-ttu-id="de82e-122">サイトのドキュメント ライブラリを一覧表示するために、アプリは Site の **drives** リレーションシップを要求します。</span><span class="sxs-lookup"><span data-stu-id="de82e-122">To list the document libraries for a site, your app requests the **drives** relationship on the Site.</span></span>

<!-- {"blockType": "request", "name": "site-list-drives", "scopes": "sites.read.all", "tags": "service.graph" } -->

```http
GET /sites/{siteId}/drives
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="de82e-123">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="de82e-123">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="de82e-124">Visual</span><span class="sxs-lookup"><span data-stu-id="de82e-124">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/site-list-drives-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="de82e-125">Java</span><span class="sxs-lookup"><span data-stu-id="de82e-125">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/site-list-drives-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="list-a-users-drives"></a><span data-ttu-id="de82e-126">ユーザーのドライブを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="de82e-126">List a user's drives</span></span>

<!-- {"blockType": "request", "name": "user-list-drives", "scopes": "files.read", "tags": "service.graph" } -->

```http
GET /users/{userId}/drives
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="de82e-127">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="de82e-127">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="de82e-128">Visual</span><span class="sxs-lookup"><span data-stu-id="de82e-128">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/user-list-drives-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="de82e-129">Java</span><span class="sxs-lookup"><span data-stu-id="de82e-129">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/user-list-drives-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="list-the-current-users-drives"></a><span data-ttu-id="de82e-130">現在のユーザーのドライブを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="de82e-130">List the current user's drives</span></span>

<!-- {"blockType": "request", "name": "enum-drives", "scopes": "files.read", "tags": "service.graph" } -->

```http
GET /me/drives
```

## <a name="optional-query-parameters"></a><span data-ttu-id="de82e-131">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="de82e-131">Optional query parameters</span></span>

<span data-ttu-id="de82e-132">このメソッドは、応答をカスタマイズするための `$expand`、`$select`、`$skipToken`、`$top`、`$orderby` の [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="de82e-132">This method supports the `$expand`, `$select`, `$skipToken`, `$top`, and `$orderby` [OData query parameters](/graph/query-parameters) to customize the response.</span></span>


## <a name="response"></a><span data-ttu-id="de82e-133">応答</span><span class="sxs-lookup"><span data-stu-id="de82e-133">Response</span></span>

<span data-ttu-id="de82e-134">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [Drive](../resources/drive.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="de82e-134">If successful, this method returns a `200 OK` response code and collection of [Drive](../resources/drive.md) objects in the response body.</span></span>

<!-- { "blockType": "response", 
       "@odata.type": "Collection(microsoft.graph.drive)",
       "name": ["group-list-drives", "site-list-drives", "user-list-drives", "enum-drives"],
       "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "942CAEB0-13AE-491B-85E4-7557CDC0F25F",
      "driveType": "documentLibrary",
      "name": "Shared Documents",
      "owner": {
        "user": {
          "id": "AE2A1EE9-81A7-423C-ABE4-B945F47509BB",
          "displayName": "Ryan Gregg"
        }
      }
    },
    {
      "id": "C1CD3ED9-0E98-4B0B-82D3-C8FB784B9DCC",
      "driveType": "documentLibrary",
      "name": "Contoso Project Files",
      "owner": {
        "user": {
          "id": "406B2281-18E8-4416-9857-38C531B904F1",
          "displayName": "Daron Spektor"
        }
      }
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="de82e-135">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="de82e-135">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="de82e-136">Visual</span><span class="sxs-lookup"><span data-stu-id="de82e-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/enum-drives-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="de82e-137">Java</span><span class="sxs-lookup"><span data-stu-id="de82e-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/enum-drives-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="remarks"></a><span data-ttu-id="de82e-138">備考</span><span class="sxs-lookup"><span data-stu-id="de82e-138">Remarks</span></span>

<span data-ttu-id="de82e-139">ほとんどのユーザーには、ドライブ リソースが 1 つしかありません。</span><span class="sxs-lookup"><span data-stu-id="de82e-139">Most users will only have a single Drive resource.</span></span>

<span data-ttu-id="de82e-140">Group と Site には、複数の Drive リソースが利用可能である場合があります。</span><span class="sxs-lookup"><span data-stu-id="de82e-140">Groups and Sites may have multiple Drive resources available.</span></span>

<span data-ttu-id="de82e-141">[system][] ファセットのあるドライブは既定では非表示です。</span><span class="sxs-lookup"><span data-stu-id="de82e-141">Drives with the [system][] facet are hidden by default.</span></span>
<span data-ttu-id="de82e-142">それらを一覧表示するには、`$select` ステートメントに `system` を含めます。</span><span class="sxs-lookup"><span data-stu-id="de82e-142">To list them, include `system` in your `$select` statement.</span></span>

[system]: ../resources/systemfacet.md

<!-- {
  "type": "#page.annotation",
  "description": "List the available drives for a user, group, or site.",
  "keywords": "drive,onedrive.drive,list drives",
  "section": "documentation",
  "tocPath": "Drives/List drives",
  "suppressions": [
    "Error: /api-reference/v1.0/api/drive-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/drive-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/v1.0/api/drive-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/drive-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/v1.0/api/drive-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/drive-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/v1.0/api/drive-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/drive-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
} -->
