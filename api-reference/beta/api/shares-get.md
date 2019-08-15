---
author: JeremyKelley
description: shareId または共有の URL を使用して、共有 DriveItem または共有アイテムのコレクションにアクセスします。
ms.date: 09/10/2017
title: 共有アイテムへのアクセス
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
ms.openlocfilehash: 705c7033309fe383ac0649609e783caa4c6acb63
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2019
ms.locfileid: "36410125"
---
# <a name="accessing-shared-driveitems"></a><span data-ttu-id="8946d-103">共有 DriveItems へのアクセス</span><span class="sxs-lookup"><span data-stu-id="8946d-103">Accessing shared DriveItems</span></span>

<span data-ttu-id="8946d-104">**shareId** または共有の URL を使用して、共有 [DriveItem](../resources/driveitem.md) または共有アイテムのコレクションにアクセスします。</span><span class="sxs-lookup"><span data-stu-id="8946d-104">Access a shared [DriveItem](../resources/driveitem.md) or a collection of shared items by using a **shareId** or sharing URL.</span></span>

<span data-ttu-id="8946d-105">この API で共有の URL を使用するには、アプリで [URL を共有のトークンに変換する](#encoding-sharing-urls)必要があります。</span><span class="sxs-lookup"><span data-stu-id="8946d-105">To use a sharing URL with this API, your app needs to [transform the URL into a sharing token](#encoding-sharing-urls).</span></span>

## <a name="permissions"></a><span data-ttu-id="8946d-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="8946d-106">Permissions</span></span>

<span data-ttu-id="8946d-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8946d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8946d-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8946d-109">Permission type</span></span>      | <span data-ttu-id="8946d-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="8946d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8946d-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8946d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="8946d-112">Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8946d-112">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="8946d-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8946d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8946d-114">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8946d-114">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="8946d-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8946d-115">Application</span></span> | <span data-ttu-id="8946d-116">Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8946d-116">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8946d-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8946d-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /shares/{shareIdOrEncodedSharingUrl}
```

### <a name="path-parameters"></a><span data-ttu-id="8946d-118">パス パラメーター</span><span class="sxs-lookup"><span data-stu-id="8946d-118">Path parameters</span></span>

| <span data-ttu-id="8946d-119">パラメーター名</span><span class="sxs-lookup"><span data-stu-id="8946d-119">Parameter Name</span></span>                 | <span data-ttu-id="8946d-120">値</span><span class="sxs-lookup"><span data-stu-id="8946d-120">Value</span></span>    | <span data-ttu-id="8946d-121">説明</span><span class="sxs-lookup"><span data-stu-id="8946d-121">Description</span></span>                                                                         |
|:-------------------------------|:---------|:------------------------------------------------------------------------------------|
| <span data-ttu-id="8946d-122">**Sharingidorencodedsharingurl**</span><span class="sxs-lookup"><span data-stu-id="8946d-122">**shareIdOrEncodedSharingUrl**</span></span> | `string` | <span data-ttu-id="8946d-123">必須。</span><span class="sxs-lookup"><span data-stu-id="8946d-123">Required.</span></span> <span data-ttu-id="8946d-124">API によって返される共有トークン、または適切にエンコードされた共有 URL。</span><span class="sxs-lookup"><span data-stu-id="8946d-124">A sharing token as returned by the API or a properly encoded sharing URL.</span></span> |

### <a name="encoding-sharing-urls"></a><span data-ttu-id="8946d-125">共有 URL をエンコードする</span><span class="sxs-lookup"><span data-stu-id="8946d-125">Encoding sharing URLs</span></span>

<span data-ttu-id="8946d-126">共有 URL をエンコードするには、次のロジックを使用します。</span><span class="sxs-lookup"><span data-stu-id="8946d-126">To encode a sharing URL, use the following logic:</span></span>

1. <span data-ttu-id="8946d-127">まず、base64 を使用して URL をエンコードします。</span><span class="sxs-lookup"><span data-stu-id="8946d-127">First, use base64 encode the URL.</span></span>
2. <span data-ttu-id="8946d-128">base64 でエンコードされた結果を [unpadded base64url 形式](https://en.wikipedia.org/wiki/Base64)に変換します (値の末尾から `=` 文字を削除し、`/` を `_`、`+` を `-` に置き換える)。</span><span class="sxs-lookup"><span data-stu-id="8946d-128">Convert the base64 encoded result to [unpadded base64url format](https://en.wikipedia.org/wiki/Base64) by removing `=` characters from the end of the value, replacing `/` with `_` and `+` with `-`.)</span></span>
3. <span data-ttu-id="8946d-129">文字列の先頭に `u!` を追加します。</span><span class="sxs-lookup"><span data-stu-id="8946d-129">Append `u!` to be beginning of the string.</span></span>

<span data-ttu-id="8946d-130">URL を C# でエンコードする例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="8946d-130">As an example, to encode a URL in C#:</span></span>

```csharp
string sharingUrl = "https://onedrive.live.com/redir?resid=1231244193912!12&authKey=1201919!12921!1";
string base64Value = System.Convert.ToBase64String(System.Text.Encoding.UTF8.GetBytes(sharingUrl));
string encodedUrl = "u!" + base64Value.TrimEnd('=').Replace('/','_').Replace('+','-');
```

## <a name="optional-request-headers"></a><span data-ttu-id="8946d-131">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8946d-131">Optional request headers</span></span>

| <span data-ttu-id="8946d-132">名前</span><span class="sxs-lookup"><span data-stu-id="8946d-132">Name</span></span>       | <span data-ttu-id="8946d-133">型</span><span class="sxs-lookup"><span data-stu-id="8946d-133">Type</span></span>   | <span data-ttu-id="8946d-134">説明</span><span class="sxs-lookup"><span data-stu-id="8946d-134">Description</span></span>                                                    |
|:-----------|:-------|:---------------------------------------------------------------|
| <span data-ttu-id="8946d-135">**Prefer**</span><span class="sxs-lookup"><span data-stu-id="8946d-135">**Prefer**</span></span> | <span data-ttu-id="8946d-136">string</span><span class="sxs-lookup"><span data-stu-id="8946d-136">string</span></span> | <span data-ttu-id="8946d-137">省略可能。</span><span class="sxs-lookup"><span data-stu-id="8946d-137">Optional.</span></span> <span data-ttu-id="8946d-138">以下に記載され`prefer`ている値の1つに設定します。</span><span class="sxs-lookup"><span data-stu-id="8946d-138">Set to one of the `prefer` values documented below.</span></span>  |

### <a name="prefer-header-values"></a><span data-ttu-id="8946d-139">ヘッダー値を優先する</span><span class="sxs-lookup"><span data-stu-id="8946d-139">Prefer header values</span></span>

| <span data-ttu-id="8946d-140">名前</span><span class="sxs-lookup"><span data-stu-id="8946d-140">Name</span></span>                          | <span data-ttu-id="8946d-141">説明</span><span class="sxs-lookup"><span data-stu-id="8946d-141">Description</span></span>                                                                                             |
|:------------------------------|:--------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="8946d-142">redeemSharingLink</span><span class="sxs-lookup"><span data-stu-id="8946d-142">redeemSharingLink</span></span>             | <span data-ttu-id="8946d-143">共有リンク\*\*\*\* の場合は、発信者に、アイテムへの永続的なアクセス権を付与します。</span><span class="sxs-lookup"><span data-stu-id="8946d-143">If the **shareIdOrEncodedSharingUrl** is a sharing link, grant the caller durable access to the item</span></span>    |
| <span data-ttu-id="8946d-144">redeemSharingLinkIfNecessary</span><span class="sxs-lookup"><span data-stu-id="8946d-144">redeemSharingLinkIfNecessary</span></span>  | <span data-ttu-id="8946d-145">RedeemSharingLink と同じですが、この要求の期間だけアクセスが許可されることが保証されます。</span><span class="sxs-lookup"><span data-stu-id="8946d-145">Same as redeemSharingLink, but access is only guaranteed to be granted for the duration of this request</span></span> |

<span data-ttu-id="8946d-146">redeemSharingLink は、発信者と同等であると考えて、共有リンクに移動します (共有ジェスチャに同意します)。 redeemSharingLinkIfNecessary は、リンクの場所を単にピークすることを目的としたシナリオに対して使用されます。metadata.</span><span class="sxs-lookup"><span data-stu-id="8946d-146">redeemSharingLink should be considered equivalent to the caller navigating to the sharing link the browser (accepting the sharing gesture), whereas redeemSharingLinkIfNecessary is intended for scenarios where the intention is simply to peek at the link's metadata.</span></span>

## <a name="response"></a><span data-ttu-id="8946d-147">応答</span><span class="sxs-lookup"><span data-stu-id="8946d-147">Response</span></span>

<span data-ttu-id="8946d-148">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [sharedDriveItem](../resources/shareddriveitem.md) リソースを返します。</span><span class="sxs-lookup"><span data-stu-id="8946d-148">If successful, this method returns a `200 OK` response code and a [sharedDriveItem](../resources/shareddriveitem.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8946d-149">例</span><span class="sxs-lookup"><span data-stu-id="8946d-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="8946d-150">要求</span><span class="sxs-lookup"><span data-stu-id="8946d-150">Request</span></span>

<span data-ttu-id="8946d-151">以下は、共有アイテムを取得する要求の例です。</span><span class="sxs-lookup"><span data-stu-id="8946d-151">Here is an example of the request to retrieve a shared item:</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="8946d-152">プロトコル</span><span class="sxs-lookup"><span data-stu-id="8946d-152">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-shared-root" } -->

```http
GET /shares/{shareIdOrEncodedSharingUrl}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="8946d-153">C#</span><span class="sxs-lookup"><span data-stu-id="8946d-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-shared-root-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8946d-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8946d-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-shared-root-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8946d-155">目的-C</span><span class="sxs-lookup"><span data-stu-id="8946d-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-shared-root-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="8946d-156">応答</span><span class="sxs-lookup"><span data-stu-id="8946d-156">Response</span></span>

<span data-ttu-id="8946d-157">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="8946d-157">Here is an example of the response.</span></span>

<!-- { "blockType": "response", "truncated": true, "@odata.type": "microsoft.graph.sharedDriveItem" } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "B64397C8-07AE-43E4-920E-32BFB4331A5B",
  "name": "contoso project.docx",
  "owner": {
    "user": {
      "id": "98E88F1C-F8DC-47CC-A406-C090248B30E5",
      "displayName": "Ryan Gregg"
    }
  }
}
```

## <a name="access-the-shared-item-directly"></a><span data-ttu-id="8946d-158">共有アイテムに直接アクセスする</span><span class="sxs-lookup"><span data-stu-id="8946d-158">Access the shared item directly</span></span>

<span data-ttu-id="8946d-p104">[**SharedDriveItem**](../resources/shareddriveitem.md) には、いくつかの有用な情報が含まれていますが、ほとんどのアプリは、共有の [DriveItem](../resources/driveitem.md)に直接アクセスする必要があります。**SharedDriveItem** リソースには、共有アイテムのスコープ内でコンテンツにアクセスできる、**root** と **items** のリレーションシップが含まれています。</span><span class="sxs-lookup"><span data-stu-id="8946d-p104">While the [**SharedDriveItem**](../resources/shareddriveitem.md) contains some useful information, most apps will want to directly access the shared [DriveItem](../resources/driveitem.md). The **SharedDriveItem** resource includes a **root** and **items** relationships which can access content within the scope of the shared item.</span></span>

## <a name="example-single-file"></a><span data-ttu-id="8946d-161">例 (単一ファイル)</span><span class="sxs-lookup"><span data-stu-id="8946d-161">Example (single file)</span></span>

### <a name="request"></a><span data-ttu-id="8946d-162">要求</span><span class="sxs-lookup"><span data-stu-id="8946d-162">Request</span></span>

<span data-ttu-id="8946d-163">**driveItem** リレーションシップを要求することで、共有された **DriveItem** が返されます。</span><span class="sxs-lookup"><span data-stu-id="8946d-163">By requesting the **driveItem** relationship, the **DriveItem** that was shared will be returned.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="8946d-164">プロトコル</span><span class="sxs-lookup"><span data-stu-id="8946d-164">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-shared-driveitem" } -->

```http
GET /shares/{shareIdOrUrl}/driveItem
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="8946d-165">C#</span><span class="sxs-lookup"><span data-stu-id="8946d-165">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-shared-driveitem-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8946d-166">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8946d-166">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-shared-driveitem-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8946d-167">目的-C</span><span class="sxs-lookup"><span data-stu-id="8946d-167">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-shared-driveitem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="8946d-168">応答</span><span class="sxs-lookup"><span data-stu-id="8946d-168">Response</span></span>

<!-- { "blockType": "response", "truncated": true, "@odata.type": "microsoft.graph.driveItem" } -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "id": "9FFFDB3C-5B87-4062-9606-1B008CA88E44",
  "name": "contoso project.docx",
  "eTag": "2246BD2D-7811-4660-BD0F-1CF36133677B,1",
  "file": {},
  "size": 109112
}
```

## <a name="example-shared-folder"></a><span data-ttu-id="8946d-169">例 (共有フォルダー)</span><span class="sxs-lookup"><span data-stu-id="8946d-169">Example (shared folder)</span></span>

### <a name="request"></a><span data-ttu-id="8946d-170">要求</span><span class="sxs-lookup"><span data-stu-id="8946d-170">Request</span></span>

<span data-ttu-id="8946d-171">**driveItem** リレーションシップを要求して、**children** コレクションを展開することで、共有されている **DriveItem** が共有フォルダー内のファイルとともに返されます。</span><span class="sxs-lookup"><span data-stu-id="8946d-171">By requesting the **driveItem** relationship and expanding the **children** collection, the **DriveItem** that was shared will be returned along with the files within the shared folder.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="8946d-172">プロトコル</span><span class="sxs-lookup"><span data-stu-id="8946d-172">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-shared-driveitem-expand-children" } -->

```http
GET /shares/{shareIdOrUrl}/driveItem?$expand=children
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="8946d-173">C#</span><span class="sxs-lookup"><span data-stu-id="8946d-173">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-shared-driveitem-expand-children-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8946d-174">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8946d-174">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-shared-driveitem-expand-children-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8946d-175">目的-C</span><span class="sxs-lookup"><span data-stu-id="8946d-175">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-shared-driveitem-expand-children-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="8946d-176">応答</span><span class="sxs-lookup"><span data-stu-id="8946d-176">Response</span></span>

<!-- { "blockType": "response", "truncated": true, "@odata.type": "microsoft.graph.driveItem" } -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "id": "9FFFDB3C-5B87-4062-9606-1B008CA88E44",
  "name": "Contoso Project",
  "eTag": "2246BD2D-7811-4660-BD0F-1CF36133677B,1",
  "folder": {},
  "size": 10911212,
  "children": [
    {
      "id": "AFBBDD79-868E-452D-AD4D-24697D4A4044",
      "name": "Propsoal.docx",
      "file": {},
      "size": 19001
    },
    {
      "id": "A91FE90A-2F2C-4EE6-B412-C4FFBA3F71A6",
      "name": "Update to Proposal.docx",
      "file": {},
      "size": 91001
    }
  ]
}
```

## <a name="error-responses"></a><span data-ttu-id="8946d-177">エラー応答</span><span class="sxs-lookup"><span data-stu-id="8946d-177">Error Responses</span></span>

<span data-ttu-id="8946d-178">エラーがどのような形で返されるかについては、「[エラー応答][error-response]」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8946d-178">Read the [Error Responses][error-response] topic for more information about how errors are returned.</span></span>

## <a name="remarks"></a><span data-ttu-id="8946d-179">備考</span><span class="sxs-lookup"><span data-stu-id="8946d-179">Remarks</span></span>

* <span data-ttu-id="8946d-180">OneDrive for Business と SharePoint の場合、Shares API には常に認証が必要です。また、ユーザー コンテキストを使用せずに、匿名で共有コンテンツにアクセスするためには使用できません。</span><span class="sxs-lookup"><span data-stu-id="8946d-180">For OneDrive for Business and SharePoint, the Shares API always requires authentication and cannot be used to access anonymously shared content without a user context.</span></span>

[error-response]: /graph/errors

<!-- {
  "type": "#page.annotation",
  "description": "Access the contents of a sharing link with the OneDrive API.",
  "keywords": "shares,shared,sharing,share link, sharing link, share id, share token",
  "section": "documentation",
  "tocPath": "Sharing/Use a link",
  "suppressions": [
  ]
} -->
