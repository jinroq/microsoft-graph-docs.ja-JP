---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: 共有アイテムへのアクセス
localization_priority: Normal
ms.openlocfilehash: cd2bd6653d12aa3296889147c1b1c78eeaddc676
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35279290"
---
# <a name="accessing-shared-driveitems"></a><span data-ttu-id="7bc6f-102">共有 DriveItems へのアクセス</span><span class="sxs-lookup"><span data-stu-id="7bc6f-102">Accessing shared DriveItems</span></span>

<span data-ttu-id="7bc6f-103">**shareId** または共有の URL を使用して、共有 [DriveItem](../resources/driveitem.md) または共有アイテムのコレクションにアクセスします。</span><span class="sxs-lookup"><span data-stu-id="7bc6f-103">Access a shared [DriveItem](../resources/driveitem.md) or a collection of shared items by using a **shareId** or sharing URL.</span></span>

<span data-ttu-id="7bc6f-104">この API で共有の URL を使用するには、アプリで [URL を共有のトークンに変換する](#encoding-sharing-urls)必要があります。</span><span class="sxs-lookup"><span data-stu-id="7bc6f-104">To use a sharing URL with this API, your app needs to [transform the URL into a sharing token](#encoding-sharing-urls).</span></span>

## <a name="permissions"></a><span data-ttu-id="7bc6f-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="7bc6f-105">Permissions</span></span>

<span data-ttu-id="7bc6f-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7bc6f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7bc6f-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7bc6f-108">Permission type</span></span>      | <span data-ttu-id="7bc6f-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="7bc6f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7bc6f-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7bc6f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="7bc6f-111">Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7bc6f-111">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="7bc6f-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7bc6f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7bc6f-113">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7bc6f-113">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="7bc6f-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7bc6f-114">Application</span></span> | <span data-ttu-id="7bc6f-115">Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7bc6f-115">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7bc6f-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7bc6f-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /shares/{shareIdOrEncodedSharingUrl}
```

### <a name="path-parameters"></a><span data-ttu-id="7bc6f-117">パス パラメーター</span><span class="sxs-lookup"><span data-stu-id="7bc6f-117">Path parameters</span></span>

| <span data-ttu-id="7bc6f-118">パラメーター名</span><span class="sxs-lookup"><span data-stu-id="7bc6f-118">Parameter Name</span></span>                 | <span data-ttu-id="7bc6f-119">値</span><span class="sxs-lookup"><span data-stu-id="7bc6f-119">Value</span></span>    | <span data-ttu-id="7bc6f-120">説明</span><span class="sxs-lookup"><span data-stu-id="7bc6f-120">Description</span></span>                                                                         |
|:-------------------------------|:---------|:------------------------------------------------------------------------------------|
| <span data-ttu-id="7bc6f-121">**Sharingidorencodedsharingurl**</span><span class="sxs-lookup"><span data-stu-id="7bc6f-121">**shareIdOrEncodedSharingUrl**</span></span> | `string` | <span data-ttu-id="7bc6f-122">必須。</span><span class="sxs-lookup"><span data-stu-id="7bc6f-122">Required.</span></span> <span data-ttu-id="7bc6f-123">API によって返される共有トークン、または適切にエンコードされた共有 URL。</span><span class="sxs-lookup"><span data-stu-id="7bc6f-123">A sharing token as returned by the API or a properly encoded sharing URL.</span></span> |

### <a name="encoding-sharing-urls"></a><span data-ttu-id="7bc6f-124">共有 URL をエンコードする</span><span class="sxs-lookup"><span data-stu-id="7bc6f-124">Encoding sharing URLs</span></span>

<span data-ttu-id="7bc6f-125">共有 URL をエンコードするには、次のロジックを使用します。</span><span class="sxs-lookup"><span data-stu-id="7bc6f-125">To encode a sharing URL, use the following logic:</span></span>

1. <span data-ttu-id="7bc6f-126">まず、base64 を使用して URL をエンコードします。</span><span class="sxs-lookup"><span data-stu-id="7bc6f-126">First, use base64 encode the URL.</span></span>
2. <span data-ttu-id="7bc6f-127">base64 でエンコードされた結果を [unpadded base64url 形式](https://en.wikipedia.org/wiki/Base64)に変換します (値の末尾から `=` 文字を削除し、`/` を `_`、`+` を `-` に置き換える)。</span><span class="sxs-lookup"><span data-stu-id="7bc6f-127">Convert the base64 encoded result to [unpadded base64url format](https://en.wikipedia.org/wiki/Base64) by removing `=` characters from the end of the value, replacing `/` with `_` and `+` with `-`.)</span></span>
3. <span data-ttu-id="7bc6f-128">文字列の先頭に `u!` を追加します。</span><span class="sxs-lookup"><span data-stu-id="7bc6f-128">Append `u!` to be beginning of the string.</span></span>

<span data-ttu-id="7bc6f-129">URL を C# でエンコードする例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="7bc6f-129">As an example, to encode a URL in C#:</span></span>

```csharp
string sharingUrl = "https://onedrive.live.com/redir?resid=1231244193912!12&authKey=1201919!12921!1";
string base64Value = System.Convert.ToBase64String(System.Text.Encoding.UTF8.GetBytes(sharingUrl));
string encodedUrl = "u!" + base64Value.TrimEnd('=').Replace('/','_').Replace('+','-');
```

## <a name="optional-request-headers"></a><span data-ttu-id="7bc6f-130">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7bc6f-130">Optional request headers</span></span>

| <span data-ttu-id="7bc6f-131">名前</span><span class="sxs-lookup"><span data-stu-id="7bc6f-131">Name</span></span>       | <span data-ttu-id="7bc6f-132">型</span><span class="sxs-lookup"><span data-stu-id="7bc6f-132">Type</span></span>   | <span data-ttu-id="7bc6f-133">説明</span><span class="sxs-lookup"><span data-stu-id="7bc6f-133">Description</span></span>                                                    |
|:-----------|:-------|:---------------------------------------------------------------|
| <span data-ttu-id="7bc6f-134">**Prefer**</span><span class="sxs-lookup"><span data-stu-id="7bc6f-134">**Prefer**</span></span> | <span data-ttu-id="7bc6f-135">string</span><span class="sxs-lookup"><span data-stu-id="7bc6f-135">string</span></span> | <span data-ttu-id="7bc6f-136">省略可能。</span><span class="sxs-lookup"><span data-stu-id="7bc6f-136">Optional.</span></span> <span data-ttu-id="7bc6f-137">以下に記載され`prefer`ている値の1つに設定します。</span><span class="sxs-lookup"><span data-stu-id="7bc6f-137">Set to one of the `prefer` values documented below.</span></span>  |

### <a name="prefer-header-values"></a><span data-ttu-id="7bc6f-138">ヘッダー値を優先する</span><span class="sxs-lookup"><span data-stu-id="7bc6f-138">Prefer header values</span></span>

| <span data-ttu-id="7bc6f-139">名前</span><span class="sxs-lookup"><span data-stu-id="7bc6f-139">Name</span></span>                          | <span data-ttu-id="7bc6f-140">説明</span><span class="sxs-lookup"><span data-stu-id="7bc6f-140">Description</span></span>                                                                                             |
|:------------------------------|:--------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="7bc6f-141">redeemSharingLink</span><span class="sxs-lookup"><span data-stu-id="7bc6f-141">redeemSharingLink</span></span>             | <span data-ttu-id="7bc6f-142">共有リンク\*\*\*\* の場合は、発信者に、アイテムへの永続的なアクセス権を付与します。</span><span class="sxs-lookup"><span data-stu-id="7bc6f-142">If the **shareIdOrEncodedSharingUrl** is a sharing link, grant the caller durable access to the item</span></span>    |
| <span data-ttu-id="7bc6f-143">redeemSharingLinkIfNecessary</span><span class="sxs-lookup"><span data-stu-id="7bc6f-143">redeemSharingLinkIfNecessary</span></span>  | <span data-ttu-id="7bc6f-144">RedeemSharingLink と同じですが、この要求の期間だけアクセスが許可されることが保証されます。</span><span class="sxs-lookup"><span data-stu-id="7bc6f-144">Same as redeemSharingLink, but access is only guaranteed to be granted for the duration of this request</span></span> |

<span data-ttu-id="7bc6f-145">redeemSharingLink は、発信者と同等であると考えて、共有リンクに移動します (共有ジェスチャに同意します)。 redeemSharingLinkIfNecessary は、リンクの場所を単にピークすることを目的としたシナリオに対して使用されます。metadata.</span><span class="sxs-lookup"><span data-stu-id="7bc6f-145">redeemSharingLink should be considered equivalent to the caller navigating to the sharing link the browser (accepting the sharing gesture), whereas redeemSharingLinkIfNecessary is intended for scenarios where the intention is simply to peek at the link's metadata.</span></span>

## <a name="response"></a><span data-ttu-id="7bc6f-146">応答</span><span class="sxs-lookup"><span data-stu-id="7bc6f-146">Response</span></span>

<span data-ttu-id="7bc6f-147">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [sharedDriveItem](../resources/shareddriveitem.md) リソースを返します。</span><span class="sxs-lookup"><span data-stu-id="7bc6f-147">If successful, this method returns a `200 OK` response code and a [sharedDriveItem](../resources/shareddriveitem.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7bc6f-148">例</span><span class="sxs-lookup"><span data-stu-id="7bc6f-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="7bc6f-149">要求</span><span class="sxs-lookup"><span data-stu-id="7bc6f-149">Request</span></span>

<span data-ttu-id="7bc6f-150">以下は、共有アイテムを取得する要求の例です。</span><span class="sxs-lookup"><span data-stu-id="7bc6f-150">Here is an example of the request to retrieve a shared item:</span></span>

<!-- { "blockType": "request", "name": "get-shared-root" } -->

```http
GET /shares/{shareIdOrEncodedSharingUrl}
```

### <a name="response"></a><span data-ttu-id="7bc6f-151">応答</span><span class="sxs-lookup"><span data-stu-id="7bc6f-151">Response</span></span>

<span data-ttu-id="7bc6f-152">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="7bc6f-152">Here is an example of the response.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="7bc6f-153">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="7bc6f-153">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="7bc6f-154">C#</span><span class="sxs-lookup"><span data-stu-id="7bc6f-154">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-shared-root-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7bc6f-155">Javascript</span><span class="sxs-lookup"><span data-stu-id="7bc6f-155">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-shared-root-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="7bc6f-156">目的-C</span><span class="sxs-lookup"><span data-stu-id="7bc6f-156">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get-shared-root-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="access-the-shared-item-directly"></a><span data-ttu-id="7bc6f-157">共有アイテムに直接アクセスする</span><span class="sxs-lookup"><span data-stu-id="7bc6f-157">Access the shared item directly</span></span>

<span data-ttu-id="7bc6f-p104">[**SharedDriveItem**](../resources/shareddriveitem.md) には、いくつかの有用な情報が含まれていますが、ほとんどのアプリは、共有の [DriveItem](../resources/driveitem.md)に直接アクセスする必要があります。**SharedDriveItem** リソースには、共有アイテムのスコープ内でコンテンツにアクセスできる、**root** と **items** のリレーションシップが含まれています。</span><span class="sxs-lookup"><span data-stu-id="7bc6f-p104">While the [**SharedDriveItem**](../resources/shareddriveitem.md) contains some useful information, most apps will want to directly access the shared [DriveItem](../resources/driveitem.md). The **SharedDriveItem** resource includes a **root** and **items** relationships which can access content within the scope of the shared item.</span></span>

## <a name="example-single-file"></a><span data-ttu-id="7bc6f-160">例 (単一ファイル)</span><span class="sxs-lookup"><span data-stu-id="7bc6f-160">Example (single file)</span></span>

### <a name="request"></a><span data-ttu-id="7bc6f-161">要求</span><span class="sxs-lookup"><span data-stu-id="7bc6f-161">Request</span></span>

<span data-ttu-id="7bc6f-162">**driveItem** リレーションシップを要求することで、共有された **DriveItem** が返されます。</span><span class="sxs-lookup"><span data-stu-id="7bc6f-162">By requesting the **driveItem** relationship, the **DriveItem** that was shared will be returned.</span></span>

<!-- { "blockType": "request", "name": "get-shared-driveitem" } -->

```http
GET /shares/{shareIdOrUrl}/driveItem
```

### <a name="response"></a><span data-ttu-id="7bc6f-163">応答</span><span class="sxs-lookup"><span data-stu-id="7bc6f-163">Response</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="7bc6f-164">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="7bc6f-164">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="7bc6f-165">C#</span><span class="sxs-lookup"><span data-stu-id="7bc6f-165">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-shared-driveitem-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7bc6f-166">Javascript</span><span class="sxs-lookup"><span data-stu-id="7bc6f-166">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-shared-driveitem-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="7bc6f-167">目的-C</span><span class="sxs-lookup"><span data-stu-id="7bc6f-167">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get-shared-driveitem-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="example-shared-folder"></a><span data-ttu-id="7bc6f-168">例 (共有フォルダー)</span><span class="sxs-lookup"><span data-stu-id="7bc6f-168">Example (shared folder)</span></span>

### <a name="request"></a><span data-ttu-id="7bc6f-169">要求</span><span class="sxs-lookup"><span data-stu-id="7bc6f-169">Request</span></span>

<span data-ttu-id="7bc6f-170">**driveItem** リレーションシップを要求して、**children** コレクションを展開することで、共有されている **DriveItem** が共有フォルダー内のファイルとともに返されます。</span><span class="sxs-lookup"><span data-stu-id="7bc6f-170">By requesting the **driveItem** relationship and expanding the **children** collection, the **DriveItem** that was shared will be returned along with the files within the shared folder.</span></span>

<!-- { "blockType": "request", "name": "get-shared-driveitem-expand-children" } -->

```http
GET /shares/{shareIdOrUrl}/driveItem?$expand=children
```

### <a name="response"></a><span data-ttu-id="7bc6f-171">応答</span><span class="sxs-lookup"><span data-stu-id="7bc6f-171">Response</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="7bc6f-172">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="7bc6f-172">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="7bc6f-173">C#</span><span class="sxs-lookup"><span data-stu-id="7bc6f-173">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-shared-driveitem-expand-children-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7bc6f-174">Javascript</span><span class="sxs-lookup"><span data-stu-id="7bc6f-174">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-shared-driveitem-expand-children-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="7bc6f-175">目的-C</span><span class="sxs-lookup"><span data-stu-id="7bc6f-175">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get-shared-driveitem-expand-children-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="error-responses"></a><span data-ttu-id="7bc6f-176">エラー応答</span><span class="sxs-lookup"><span data-stu-id="7bc6f-176">Error Responses</span></span>

<span data-ttu-id="7bc6f-177">エラーがどのような形で返されるかについては、「[エラー応答][error-response]」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7bc6f-177">Read the [Error Responses][error-response] topic for more information about how errors are returned.</span></span>

## <a name="remarks"></a><span data-ttu-id="7bc6f-178">備考</span><span class="sxs-lookup"><span data-stu-id="7bc6f-178">Remarks</span></span>

* <span data-ttu-id="7bc6f-179">OneDrive for Business と SharePoint の場合、Shares API には常に認証が必要です。また、ユーザー コンテキストを使用せずに、匿名で共有コンテンツにアクセスするためには使用できません。</span><span class="sxs-lookup"><span data-stu-id="7bc6f-179">For OneDrive for Business and SharePoint, the Shares API always requires authentication and cannot be used to access anonymously shared content without a user context.</span></span>

[error-response]: /graph/errors

<!-- {
  "type": "#page.annotation",
  "description": "Access the contents of a sharing link with the OneDrive API.",
  "keywords": "shares,shared,sharing,share link, sharing link, share id, share token",
  "section": "documentation",
  "tocPath": "Sharing/Use a link",
  "suppressions": [
    "Error: /api-reference/v1.0/api/shares-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/shares-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/shares-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/v1.0/api/shares-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/shares-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/v1.0/api/shares-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/shares-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
} -->
