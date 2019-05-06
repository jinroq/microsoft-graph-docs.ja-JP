---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: アクセス許可の取得
localization_priority: Normal
ms.openlocfilehash: ca401e0cbbd76a44e1b87a7cb581a2a340b3a844
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33595722"
---
# <a name="get-sharing-permission-for-a-file-or-folder"></a><span data-ttu-id="41bcc-102">ファイルまたはフォルダーの共有アクセス許可を取得する</span><span class="sxs-lookup"><span data-stu-id="41bcc-102">Get sharing permission for a file or folder</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="41bcc-103">特定のアクセス許可リソースに対する、有効な共有アクセス許可を返します。</span><span class="sxs-lookup"><span data-stu-id="41bcc-103">Return the effective sharing permission for a particular permission resource.</span></span>

<span data-ttu-id="41bcc-104">アイテムの有効なアクセス許可は、アイテム自体に直接設定されたアクセス許可、またはアイテムの先祖から継承したアクセス許可の 2 つのソースから取得できます。</span><span class="sxs-lookup"><span data-stu-id="41bcc-104">Effective permissions of an item can come from two sources: permissions set directly on the item itself or permissions that are inherited from the item's ancestors.</span></span>

<span data-ttu-id="41bcc-p101">呼び出し元は、`inheritedFrom` プロパティを確認することで、アクセス許可が継承されたものかどうかを区別できます。このプロパティは、アクセス許可の継承元になる先祖を参照する [ItemReference](../resources/itemreference.md) リソースです。</span><span class="sxs-lookup"><span data-stu-id="41bcc-p101">Callers can differentiate if the permission is inherited or not by checking the `inheritedFrom` property. This property is an [ItemReference](../resources/itemreference.md) resource referencing the ancestor that the permission is inherited from.</span></span>

<span data-ttu-id="41bcc-p102">アイテムに設定された SharePoint アクセス許可レベルは、'SP' というプレフィックス付きで返されます。 たとえば、SP.View Only、SP.Limited Access、SP.View Web Analytics Data などです。 [SharePoint ロールの完全なリスト](https://technet.microsoft.com/en-us/library/cc721640.aspx#section1)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="41bcc-p102">SharePoint permission levels set on an item are returned with an 'SP' prefix. For example, SP.View Only, SP.Limited Access, SP.View Web Analytics Data. See [Full list of SharePoint roles](https://technet.microsoft.com/en-us/library/cc721640.aspx#section1).</span></span>

## <a name="permissions"></a><span data-ttu-id="41bcc-110">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="41bcc-110">Permissions</span></span>

<span data-ttu-id="41bcc-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="41bcc-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="41bcc-113">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="41bcc-113">Permission type</span></span>      | <span data-ttu-id="41bcc-114">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="41bcc-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="41bcc-115">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="41bcc-115">Delegated (work or school account)</span></span> | <span data-ttu-id="41bcc-116">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="41bcc-116">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="41bcc-117">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="41bcc-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="41bcc-118">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="41bcc-118">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="41bcc-119">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="41bcc-119">Application</span></span> | <span data-ttu-id="41bcc-120">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="41bcc-120">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="41bcc-121">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="41bcc-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/permissions/{perm-id}
GET /groups/{group-id}/drive/items/{item-id}/permissions/{perm-id}
GET /me/drive/items/{item-id}/permissions/{perm-id}
GET /sites/{site-id}/drive/items/{item-id}/permissions/{perm-id}
GET /users/{user-id}/drive/items/{item-id}/permissions/{perm-id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="41bcc-122">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="41bcc-122">Optional query parameters</span></span>

<span data-ttu-id="41bcc-123">応答を形成するため、このメソッドは、[$select クエリ パラメーター](/graph/query-parameters) をサポートしています。</span><span class="sxs-lookup"><span data-stu-id="41bcc-123">This method support the [$select query parameter](/graph/query-parameters) to shape the response.</span></span>

## <a name="response"></a><span data-ttu-id="41bcc-124">応答</span><span class="sxs-lookup"><span data-stu-id="41bcc-124">Response</span></span>

<span data-ttu-id="41bcc-125">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [Permission](../resources/permission.md) リソースを返します。</span><span class="sxs-lookup"><span data-stu-id="41bcc-125">If successful, this method returns a `200 OK` response code and [Permission](../resources/permission.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="41bcc-126">例</span><span class="sxs-lookup"><span data-stu-id="41bcc-126">Example</span></span>

### <a name="request"></a><span data-ttu-id="41bcc-127">要求</span><span class="sxs-lookup"><span data-stu-id="41bcc-127">Request</span></span>

<span data-ttu-id="41bcc-128">以下は、フォルダーのアクセス許可にアクセスするための要求の例です。</span><span class="sxs-lookup"><span data-stu-id="41bcc-128">Here is an example of the request to access a permission on a folder.</span></span>

<!-- { "blockType": "request", "name": "get-item-permission", "scopes": "files.read" } -->

```http
GET https://graph.microsoft.com/beta/me/drive/items/{item-id}/permissions/{perm-id}
```
### <a name="response"></a><span data-ttu-id="41bcc-129">応答</span><span class="sxs-lookup"><span data-stu-id="41bcc-129">Response</span></span>

<span data-ttu-id="41bcc-130">成功した場合、このメソッドは、指定された ID の [Permission](../resources/permission.md) リソースを返します。</span><span class="sxs-lookup"><span data-stu-id="41bcc-130">If successful, this method returns a [Permission](../resources/permission.md) resource for the specified ID.</span></span> 

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="41bcc-131">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="41bcc-131">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="41bcc-132">Visual</span><span class="sxs-lookup"><span data-stu-id="41bcc-132">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-item-permission-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="41bcc-133">Java</span><span class="sxs-lookup"><span data-stu-id="41bcc-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-item-permission-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="remarks"></a><span data-ttu-id="41bcc-134">備考</span><span class="sxs-lookup"><span data-stu-id="41bcc-134">Remarks</span></span>

<span data-ttu-id="41bcc-135">[アクセス権](../resources/permission.md)リソースは、_ファセット_を使用してリソースによって表されるアクセス許可の種類に関する情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="41bcc-135">The [Permission](../resources/permission.md) resource uses _facets_ to provide information about the kind of permission represented by the resource.</span></span>

<span data-ttu-id="41bcc-p104">[**リンク**](../resources/sharinglink.md) ファセットのあるアクセス許可は、項目上に作成された共有するリンクを表します。共有リンクは、リンクを持つすべてのユーザーのアイテムへのアクセス許可を提供する固有のトークンを含みます。</span><span class="sxs-lookup"><span data-stu-id="41bcc-p104">Permissions with a [**link**](../resources/sharinglink.md) facet represent sharing links created on the item. Sharing links contain a unique token that provides access to the item for anyone with the link.</span></span>

<span data-ttu-id="41bcc-138">[**招待**](../resources/sharinginvitation.md) ファセットを持つアクセス許可は、指定のユーザーやグループをファイルへのアクセスへ招待することで追加されたアクセス許可を表します。</span><span class="sxs-lookup"><span data-stu-id="41bcc-138">Permissions with a [**invitation**](../resources/sharinginvitation.md) facet represent permissions added by inviting specific users or groups to have access to the file.</span></span>

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
    "Error: /api-reference/beta/api/permission-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/permission-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
