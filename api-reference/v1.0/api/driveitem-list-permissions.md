---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: ファイルへのアクセス権を持つユーザーを一覧表示する
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 9ecbb197eb93c6251d5eac0b2bc1baea4b7efe87
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35888035"
---
# <a name="list-sharing-permissions-on-a-driveitem"></a><span data-ttu-id="3eb06-102">DriveItem の共有アクセス許可を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="3eb06-102">List sharing permissions on a DriveItem</span></span>

<span data-ttu-id="3eb06-103">[DriveItem](../resources/driveitem.md) の有効な共有アクセス許可を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="3eb06-103">List the effective sharing permissions of on a [DriveItem](../resources/driveitem.md).</span></span>

## <a name="access-to-sharing-permissions"></a><span data-ttu-id="3eb06-104">共有アクセス許可へのアクセス</span><span class="sxs-lookup"><span data-stu-id="3eb06-104">Access to sharing permissions</span></span>

<span data-ttu-id="3eb06-105">アクセス許可のコレクションには、機密情報が含まれている可能性があり、呼び出し元によっては使用できないこともあります。</span><span class="sxs-lookup"><span data-stu-id="3eb06-105">The permissions collection includes potentially sensitive information and may not be available for every caller.</span></span>

* <span data-ttu-id="3eb06-106">アイテムのオーナーの場合は、すべての共有アクセス許可が返されます。</span><span class="sxs-lookup"><span data-stu-id="3eb06-106">For the owner of the item, all sharing permissions will be returned.</span></span> <span data-ttu-id="3eb06-107">これには、共同所有者が含まれます。</span><span class="sxs-lookup"><span data-stu-id="3eb06-107">This includes co-owners.</span></span>
* <span data-ttu-id="3eb06-108">所有者以外の呼び出し元の場合、その呼び出し元に適用される共有アクセス許可のみが返されます。</span><span class="sxs-lookup"><span data-stu-id="3eb06-108">For a non-owner caller, only the sharing permissions that apply to the caller are returned.</span></span>
* <span data-ttu-id="3eb06-109">秘密 (`shareId` や `webUrl` など) を含む共有アクセス許可のプロパティは、その共有アクセス許可を作成できる呼び出し元にのみ返されます。</span><span class="sxs-lookup"><span data-stu-id="3eb06-109">Sharing permission properties that contain secrets (e.g. `shareId` and `webUrl`) are only returned for callers that are able to create the sharing permission.</span></span>

## <a name="permissions"></a><span data-ttu-id="3eb06-110">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="3eb06-110">Permissions</span></span>

<span data-ttu-id="3eb06-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3eb06-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3eb06-113">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3eb06-113">Permission type</span></span>      | <span data-ttu-id="3eb06-114">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="3eb06-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3eb06-115">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3eb06-115">Delegated (work or school account)</span></span> | <span data-ttu-id="3eb06-116">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3eb06-116">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="3eb06-117">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3eb06-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3eb06-118">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3eb06-118">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="3eb06-119">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3eb06-119">Application</span></span> | <span data-ttu-id="3eb06-120">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3eb06-120">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3eb06-121">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3eb06-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/permissions
GET /groups/{group-id}/drive/items/{item-id}/permissions
GET /me/drive/items/{item-id}/permissions
GET /me/drive/root:/{path}:/permissions
GET /sites/{siteId}/drive/items/{itemId}/permissions
GET /users/{userId}/drive/items/{itemId}/permissions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3eb06-122">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="3eb06-122">Optional query parameters</span></span>

<span data-ttu-id="3eb06-123">このメソッドは、応答をカスタマイズするための `$select` の [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="3eb06-123">This method supports the `$select` [OData Query Parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="optional-request-headers"></a><span data-ttu-id="3eb06-124">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3eb06-124">Optional request headers</span></span>

| <span data-ttu-id="3eb06-125">名前</span><span class="sxs-lookup"><span data-stu-id="3eb06-125">Name</span></span>          | <span data-ttu-id="3eb06-126">型</span><span class="sxs-lookup"><span data-stu-id="3eb06-126">Type</span></span>   | <span data-ttu-id="3eb06-127">説明</span><span class="sxs-lookup"><span data-stu-id="3eb06-127">Description</span></span>                                                                                                                                     |
|:--------------|:-------|:------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="3eb06-128">if-none-match</span><span class="sxs-lookup"><span data-stu-id="3eb06-128">if-none-match</span></span> | <span data-ttu-id="3eb06-129">string</span><span class="sxs-lookup"><span data-stu-id="3eb06-129">string</span></span> | <span data-ttu-id="3eb06-130">この要求ヘッダーが含まれている場合、指定された etag がアイテムの現在の etag に一致すると、`HTTP 304 Not Modified` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="3eb06-130">If this request header is included and the etag provided matches the current etag on the item, an `HTTP 304 Not Modified` response is returned.</span></span> |

## <a name="response"></a><span data-ttu-id="3eb06-131">応答</span><span class="sxs-lookup"><span data-stu-id="3eb06-131">Response</span></span>

<span data-ttu-id="3eb06-132">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [Permission](../resources/permission.md) リソースのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="3eb06-132">If successful, this method returns a `200 OK` response code and collection of [Permission](../resources/permission.md) resources in the response body.</span></span>

<span data-ttu-id="3eb06-133">DriveItem の有効な共有アクセス許可は、次の 2 つのソースが元になります。</span><span class="sxs-lookup"><span data-stu-id="3eb06-133">Effective sharing permissions of a DriveItem can come from two sources:</span></span>

* <span data-ttu-id="3eb06-134">DriveItem 自体に直接適用される共有アクセス許可</span><span class="sxs-lookup"><span data-stu-id="3eb06-134">Sharing permissions applied directly on the DriveItem itself</span></span>
* <span data-ttu-id="3eb06-135">DriveItem の先祖から継承された共有アクセス許可</span><span class="sxs-lookup"><span data-stu-id="3eb06-135">Sharing permissions inherited from the DriveItem's ancestors</span></span>

<span data-ttu-id="3eb06-p103">呼び出し元は、**inheritedFrom** プロパティを確認して、アクセス許可が継承されているかどうかによって区別できます。このプロパティは、アクセス許可が継承された先祖を参照する [**itemReference**](../resources/itemreference.md) リソースです。</span><span class="sxs-lookup"><span data-stu-id="3eb06-p103">Callers can differentiate if the permission is inherited or not by checking the **inheritedFrom** property. This property is an [**itemReference**](../resources/itemreference.md) resource referencing the ancestor that the permission is inherited from.</span></span>

<span data-ttu-id="3eb06-p104">アイテムに設定された SharePoint アクセス許可レベルは、'SP' というプレフィックス付きで返されます。 たとえば、SP.View Only、SP.Limited Access、SP.View Web Analytics Data などです。 [SharePoint ロールの完全なリスト](https://technet.microsoft.com/en-us/library/cc721640.aspx#section1)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3eb06-p104">SharePoint permission levels set on an item are returned with an 'SP' prefix. For example, SP.View Only, SP.Limited Access, SP.View Web Analytics Data. See [Full list of SharePoint roles](https://technet.microsoft.com/en-us/library/cc721640.aspx#section1).</span></span>

## <a name="example"></a><span data-ttu-id="3eb06-141">例</span><span class="sxs-lookup"><span data-stu-id="3eb06-141">Example</span></span>

<span data-ttu-id="3eb06-142">この例では、サインイン ユーザーのドライブ内のアイテムに対するアクセス許可のコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="3eb06-142">This example retrieves the collection of permissions on an item in the signed in user's drive.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="3eb06-143">プロトコル</span><span class="sxs-lookup"><span data-stu-id="3eb06-143">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-item-permissions", "scopes": "files.read", "tags": "service.graph" } -->

```http
GET /me/drive/items/{item-id}/permissions
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="3eb06-144">C#</span><span class="sxs-lookup"><span data-stu-id="3eb06-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-item-permissions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3eb06-145">Javascript</span><span class="sxs-lookup"><span data-stu-id="3eb06-145">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-item-permissions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="3eb06-146">目的-C</span><span class="sxs-lookup"><span data-stu-id="3eb06-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-item-permissions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="3eb06-147">Java</span><span class="sxs-lookup"><span data-stu-id="3eb06-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-item-permissions-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="3eb06-148">応答</span><span class="sxs-lookup"><span data-stu-id="3eb06-148">Response</span></span>

<span data-ttu-id="3eb06-149">この応答例には、3 つのアクセス許可が含まれています。1 つ目は編集権限を伴う共有リンク、2 つ目は親フォルダーから継承された、John という名前のユーザーへの明示的なアクセス許可、3 つ目はアプリケーションによって作成された読み取り/書き込み共有リンクです。</span><span class="sxs-lookup"><span data-stu-id="3eb06-149">This example response includes three permissions, the first is a sharing link with edit permissions, the second is an explicit permission for a user named John, which was inherited from a parent folder, and the third is a read-write sharing link created by an application.</span></span>

<!-- {"blockType": "response", "@odata.type": "Collection(microsoft.graph.permission)", "truncated": true} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "1",
      "roles": ["write"],
      "link": {
        "webUrl": "https://onedrive.live.com/redir?resid=5D33DD65C6932946!70859&authkey=!AL7N1QAfSWcjNU8&ithint=folder%2cgif",
        "type": "edit"
      }
    },
    {
      "id": "2",
      "roles": ["write"],
      "grantedTo": {
        "user": {
          "id": "5D33DD65C6932946",
          "displayName": "John Doe"
        }
      },
      "inheritedFrom": {
        "driveId": "1234567890ABD",
        "id": "1234567890ABC!123",
        "path": "/drive/root:/Documents" }
    },
    {
      "id": "3",
      "roles": ["write"],
      "link": {
        "webUrl": "https://onedrive.live.com/redir?resid=5D33DD65C6932946!70859&authkey=!AL7N1QAfSWcjNU8&ithint=folder%2cgif",
        "type": "edit",
        "application": {
          "id": "12345",
          "displayName": "Contoso Time Manager"
        }
      }
    }
  ]
}
```

## <a name="remarks"></a><span data-ttu-id="3eb06-150">備考</span><span class="sxs-lookup"><span data-stu-id="3eb06-150">Remarks</span></span>

<span data-ttu-id="3eb06-p105">DriveItem の **permissions** リレーションシップは、[DriveItem の取得](driveitem-get.md)または DriveItem のコレクションの取得の一環として展開することはできません。permissions プロパティに直接アクセスする必要があります。</span><span class="sxs-lookup"><span data-stu-id="3eb06-p105">The **permissions** relationship of DriveItem cannot be expanded as part of a call to [get DriveItem](driveitem-get.md) or a collection of DriveItems. You must access the permissions property directly.</span></span>

## <a name="error-responses"></a><span data-ttu-id="3eb06-153">エラー応答</span><span class="sxs-lookup"><span data-stu-id="3eb06-153">Error responses</span></span>

<span data-ttu-id="3eb06-154">エラーがどのような形で返されるかについては、「[エラー応答][error-response]」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3eb06-154">Read the [Error Responses][error-response] topic for more information about how errors are returned.</span></span>

[error-response]: /graph/errors

<!-- {
  "type": "#page.annotation",
  "description": "List an item's permissions",
  "keywords": "permission, permissions, sharing",
  "section": "documentation",
  "tocPath": "Sharing/Permissions",
  "suppressions": [
  ]
} -->
