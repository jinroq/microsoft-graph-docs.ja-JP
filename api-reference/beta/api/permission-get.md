---
author: JeremyKelley
description: 特定のアクセス許可リソースに対する、有効な共有アクセス許可を返します。
ms.date: 09/10/2017
title: アクセス許可の取得
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
ms.openlocfilehash: 1a102867af744ebe78cdb6db75caf19ddcef37d2
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35983510"
---
# <a name="get-sharing-permission-for-a-file-or-folder"></a><span data-ttu-id="87879-103">ファイルまたはフォルダーの共有アクセス許可を取得する</span><span class="sxs-lookup"><span data-stu-id="87879-103">Get sharing permission for a file or folder</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="87879-104">特定のアクセス許可リソースに対する、有効な共有アクセス許可を返します。</span><span class="sxs-lookup"><span data-stu-id="87879-104">Return the effective sharing permission for a particular permission resource.</span></span>

<span data-ttu-id="87879-105">アイテムの有効なアクセス許可は、アイテム自体に直接設定されたアクセス許可、またはアイテムの先祖から継承したアクセス許可の 2 つのソースから取得できます。</span><span class="sxs-lookup"><span data-stu-id="87879-105">Effective permissions of an item can come from two sources: permissions set directly on the item itself or permissions that are inherited from the item's ancestors.</span></span>

<span data-ttu-id="87879-p101">呼び出し元は、`inheritedFrom` プロパティを確認することで、アクセス許可が継承されたものかどうかを区別できます。このプロパティは、アクセス許可の継承元になる先祖を参照する [ItemReference](../resources/itemreference.md) リソースです。</span><span class="sxs-lookup"><span data-stu-id="87879-p101">Callers can differentiate if the permission is inherited or not by checking the `inheritedFrom` property. This property is an [ItemReference](../resources/itemreference.md) resource referencing the ancestor that the permission is inherited from.</span></span>

<span data-ttu-id="87879-p102">アイテムに設定された SharePoint アクセス許可レベルは、'SP' というプレフィックス付きで返されます。 たとえば、SP.View Only、SP.Limited Access、SP.View Web Analytics Data などです。 [SharePoint ロールの完全なリスト](https://technet.microsoft.com/en-us/library/cc721640.aspx#section1)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="87879-p102">SharePoint permission levels set on an item are returned with an 'SP' prefix. For example, SP.View Only, SP.Limited Access, SP.View Web Analytics Data. See [Full list of SharePoint roles](https://technet.microsoft.com/en-us/library/cc721640.aspx#section1).</span></span>

## <a name="permissions"></a><span data-ttu-id="87879-111">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="87879-111">Permissions</span></span>

<span data-ttu-id="87879-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="87879-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="87879-114">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="87879-114">Permission type</span></span>      | <span data-ttu-id="87879-115">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="87879-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="87879-116">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="87879-116">Delegated (work or school account)</span></span> | <span data-ttu-id="87879-117">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="87879-117">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="87879-118">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="87879-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="87879-119">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="87879-119">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="87879-120">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="87879-120">Application</span></span> | <span data-ttu-id="87879-121">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="87879-121">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="87879-122">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="87879-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/permissions/{perm-id}
GET /groups/{group-id}/drive/items/{item-id}/permissions/{perm-id}
GET /me/drive/items/{item-id}/permissions/{perm-id}
GET /sites/{site-id}/drive/items/{item-id}/permissions/{perm-id}
GET /users/{user-id}/drive/items/{item-id}/permissions/{perm-id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="87879-123">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="87879-123">Optional query parameters</span></span>

<span data-ttu-id="87879-124">応答を形成するため、このメソッドは、[$select クエリ パラメーター](/graph/query-parameters) をサポートしています。</span><span class="sxs-lookup"><span data-stu-id="87879-124">This method support the [$select query parameter](/graph/query-parameters) to shape the response.</span></span>

## <a name="response"></a><span data-ttu-id="87879-125">応答</span><span class="sxs-lookup"><span data-stu-id="87879-125">Response</span></span>

<span data-ttu-id="87879-126">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [Permission](../resources/permission.md) リソースを返します。</span><span class="sxs-lookup"><span data-stu-id="87879-126">If successful, this method returns a `200 OK` response code and [Permission](../resources/permission.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="87879-127">例</span><span class="sxs-lookup"><span data-stu-id="87879-127">Example</span></span>

### <a name="request"></a><span data-ttu-id="87879-128">要求</span><span class="sxs-lookup"><span data-stu-id="87879-128">Request</span></span>

<span data-ttu-id="87879-129">以下は、フォルダーのアクセス許可にアクセスするための要求の例です。</span><span class="sxs-lookup"><span data-stu-id="87879-129">Here is an example of the request to access a permission on a folder.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="87879-130">プロトコル</span><span class="sxs-lookup"><span data-stu-id="87879-130">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-item-permission", "scopes": "files.read" } -->

```http
GET https://graph.microsoft.com/beta/me/drive/items/{item-id}/permissions/{perm-id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="87879-131">C#</span><span class="sxs-lookup"><span data-stu-id="87879-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-item-permission-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="87879-132">Javascript</span><span class="sxs-lookup"><span data-stu-id="87879-132">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-item-permission-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="87879-133">目的-C</span><span class="sxs-lookup"><span data-stu-id="87879-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-item-permission-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="87879-134">Java</span><span class="sxs-lookup"><span data-stu-id="87879-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-item-permission-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="87879-135">応答</span><span class="sxs-lookup"><span data-stu-id="87879-135">Response</span></span>

<span data-ttu-id="87879-136">成功した場合、このメソッドは、指定された ID の [Permission](../resources/permission.md) リソースを返します。</span><span class="sxs-lookup"><span data-stu-id="87879-136">If successful, this method returns a [Permission](../resources/permission.md) resource for the specified ID.</span></span> 

<!-- {"blockType": "response", "@odata.type": "microsoft.graph.permission", "truncated": true} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "grantedTo": {
    "user": {
      "displayName": "Ryan Gregg",
      "id": "efee1b77-fb3b-4f65-99d6-274c11914d12"
    }
  },
  "id": "1",
  "roles": [ "write" ]
}
```

## <a name="remarks"></a><span data-ttu-id="87879-137">備考</span><span class="sxs-lookup"><span data-stu-id="87879-137">Remarks</span></span>

<span data-ttu-id="87879-138">[アクセス権](../resources/permission.md)リソースは、_ファセット_を使用してリソースによって表されるアクセス許可の種類に関する情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="87879-138">The [Permission](../resources/permission.md) resource uses _facets_ to provide information about the kind of permission represented by the resource.</span></span>

<span data-ttu-id="87879-p104">[**リンク**](../resources/sharinglink.md) ファセットのあるアクセス許可は、項目上に作成された共有するリンクを表します。共有リンクは、リンクを持つすべてのユーザーのアイテムへのアクセス許可を提供する固有のトークンを含みます。</span><span class="sxs-lookup"><span data-stu-id="87879-p104">Permissions with a [**link**](../resources/sharinglink.md) facet represent sharing links created on the item. Sharing links contain a unique token that provides access to the item for anyone with the link.</span></span>

<span data-ttu-id="87879-141">[**招待**](../resources/sharinginvitation.md) ファセットを持つアクセス許可は、指定のユーザーやグループをファイルへのアクセスへ招待することで追加されたアクセス許可を表します。</span><span class="sxs-lookup"><span data-stu-id="87879-141">Permissions with a [**invitation**](../resources/sharinginvitation.md) facet represent permissions added by inviting specific users or groups to have access to the file.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get a DriveItem's sharing permissions",
  "keywords": "permission, permissions, sharing",
  "section": "documentation",
  "tocPath": "OneDrive/Item/Get permission",
  "suppressions": [
  ]
}
-->
