---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: ドライブを一覧表示する
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 5dbebad65bacae554c1e2739c01634d0647d1660
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35861555"
---
# <a name="list-available-drives"></a><span data-ttu-id="49af6-102">利用可能なドライブの一覧表示</span><span class="sxs-lookup"><span data-stu-id="49af6-102">List available drives</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="49af6-103">ターゲットとなる User、Group、または [Site](../resources/site.md) が利用可能な [Drive](../resources/drive.md) リソースの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="49af6-103">Retrieve the list of [Drive](../resources/drive.md) resources available for a target User, Group, or [Site](../resources/site.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="49af6-104">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="49af6-104">Permissions</span></span>

<span data-ttu-id="49af6-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="49af6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="49af6-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="49af6-107">Permission type</span></span>      | <span data-ttu-id="49af6-108">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="49af6-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="49af6-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="49af6-109">Delegated (work or school account)</span></span> | <span data-ttu-id="49af6-110">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49af6-110">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="49af6-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="49af6-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="49af6-112">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49af6-112">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="49af6-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="49af6-113">Application</span></span> | <span data-ttu-id="49af6-114">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49af6-114">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="list-a-groups-drives"></a><span data-ttu-id="49af6-115">グループのドライブを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="49af6-115">List a group's drives</span></span>

<span data-ttu-id="49af6-116">グループのドキュメント ライブラリを一覧表示するために、アプリが Group の **drives** リレーションシップを要求します。</span><span class="sxs-lookup"><span data-stu-id="49af6-116">To list the document libraries for a group, your app requests the **drives** relationship on the Group.</span></span>

### <a name="http-request"></a><span data-ttu-id="49af6-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="49af6-117">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="49af6-118">プロトコル</span><span class="sxs-lookup"><span data-stu-id="49af6-118">HTTP</span></span>](#tab/http)
<!-- {"blockType": "request", "name": "group-list-drives", "scopes": "groups.read.all" } -->

```http
GET /groups/{groupId}/drives
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="49af6-119">C#</span><span class="sxs-lookup"><span data-stu-id="49af6-119">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-list-drives-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="49af6-120">Javascript</span><span class="sxs-lookup"><span data-stu-id="49af6-120">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-list-drives-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="49af6-121">目的-C</span><span class="sxs-lookup"><span data-stu-id="49af6-121">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-list-drives-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="49af6-122">Java</span><span class="sxs-lookup"><span data-stu-id="49af6-122">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-list-drives-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="list-a-sites-drives"></a><span data-ttu-id="49af6-123">サイトのドライブを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="49af6-123">List a site's drives</span></span>

<span data-ttu-id="49af6-124">サイトのドキュメント ライブラリを一覧表示するために、アプリは Site の **drives** リレーションシップを要求します。</span><span class="sxs-lookup"><span data-stu-id="49af6-124">To list the document libraries for a site, your app requests the **drives** relationship on the Site.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="49af6-125">プロトコル</span><span class="sxs-lookup"><span data-stu-id="49af6-125">HTTP</span></span>](#tab/http)
<!-- {"blockType": "request", "name": "site-list-drives", "scopes": "sites.read.all" } -->

```http
GET /sites/{siteId}/drives
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="49af6-126">C#</span><span class="sxs-lookup"><span data-stu-id="49af6-126">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/site-list-drives-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="49af6-127">Javascript</span><span class="sxs-lookup"><span data-stu-id="49af6-127">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/site-list-drives-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="49af6-128">目的-C</span><span class="sxs-lookup"><span data-stu-id="49af6-128">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/site-list-drives-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="49af6-129">Java</span><span class="sxs-lookup"><span data-stu-id="49af6-129">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/site-list-drives-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="list-a-users-drives"></a><span data-ttu-id="49af6-130">ユーザーのドライブを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="49af6-130">List a user's drives</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="49af6-131">プロトコル</span><span class="sxs-lookup"><span data-stu-id="49af6-131">HTTP</span></span>](#tab/http)
<!-- {"blockType": "request", "name": "user-list-drives", "scopes": "files.read.all" } -->

```http
GET /users/{userId}/drives
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="49af6-132">C#</span><span class="sxs-lookup"><span data-stu-id="49af6-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-list-drives-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="49af6-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="49af6-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-list-drives-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="49af6-134">目的-C</span><span class="sxs-lookup"><span data-stu-id="49af6-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-list-drives-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="49af6-135">Java</span><span class="sxs-lookup"><span data-stu-id="49af6-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-list-drives-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="list-the-current-users-drives"></a><span data-ttu-id="49af6-136">現在のユーザーのドライブを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="49af6-136">List the current user's drives</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="49af6-137">プロトコル</span><span class="sxs-lookup"><span data-stu-id="49af6-137">HTTP</span></span>](#tab/http)
<!-- {"blockType": "request", "name": "enum-drives", "scopes": "files.read" } -->

```http
GET /me/drives
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="49af6-138">C#</span><span class="sxs-lookup"><span data-stu-id="49af6-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/enum-drives-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="49af6-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="49af6-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/enum-drives-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="49af6-140">目的-C</span><span class="sxs-lookup"><span data-stu-id="49af6-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/enum-drives-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="49af6-141">Java</span><span class="sxs-lookup"><span data-stu-id="49af6-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/enum-drives-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="optional-query-parameters"></a><span data-ttu-id="49af6-142">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="49af6-142">Optional query parameters</span></span>

<span data-ttu-id="49af6-143">このメソッドは、応答をカスタマイズするための `$expand`、`$select`、`$skipToken`、`$top`、`$orderby` の [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="49af6-143">This method supports the `$expand`, `$select`, `$skipToken`, `$top`, and `$orderby` [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="response"></a><span data-ttu-id="49af6-144">応答</span><span class="sxs-lookup"><span data-stu-id="49af6-144">Response</span></span>

<span data-ttu-id="49af6-145">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [Drive](../resources/drive.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="49af6-145">If successful, this method returns a `200 OK` response code and collection of [Drive](../resources/drive.md) objects in the response body.</span></span>

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

## <a name="remarks"></a><span data-ttu-id="49af6-146">備考</span><span class="sxs-lookup"><span data-stu-id="49af6-146">Remarks</span></span>

<span data-ttu-id="49af6-147">ほとんどのユーザーには、ドライブ リソースが 1 つしかありません。</span><span class="sxs-lookup"><span data-stu-id="49af6-147">Most users will only have a single Drive resource.</span></span>

<span data-ttu-id="49af6-148">Group と Site には、複数の Drive リソースが利用可能である場合があります。</span><span class="sxs-lookup"><span data-stu-id="49af6-148">Groups and Sites may have multiple Drive resources available.</span></span>

<span data-ttu-id="49af6-149">[system][] ファセットのあるドライブは既定では非表示です。</span><span class="sxs-lookup"><span data-stu-id="49af6-149">Drives with the [system][] facet are hidden by default.</span></span>
<span data-ttu-id="49af6-150">それらを一覧表示するには、`$select` ステートメントに `system` を含めます。</span><span class="sxs-lookup"><span data-stu-id="49af6-150">To list them, include `system` in your `$select` statement.</span></span>

[system]: ../resources/systemfacet.md

<!--
{
  "type": "#page.annotation",
  "description": "List the available drives for a user, group, or site.",
  "keywords": "drive,onedrive.drive,list drives",
  "section": "documentation",
  "tocPath": "Drives/List drives",
  "suppressions": [
  ]
}
-->
