---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: 共有アイテムへのアクセス
localization_priority: Normal
ms.openlocfilehash: 0d0c244c1707714bd651be0dd8e0d22752a0a628
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35453671"
---
# <a name="accessing-shared-driveitems"></a><span data-ttu-id="eb8ff-102">共有 DriveItems へのアクセス</span><span class="sxs-lookup"><span data-stu-id="eb8ff-102">Accessing shared DriveItems</span></span>

<span data-ttu-id="eb8ff-103">**shareId** または共有の URL を使用して、共有 [DriveItem](../resources/driveitem.md) または共有アイテムのコレクションにアクセスします。</span><span class="sxs-lookup"><span data-stu-id="eb8ff-103">Access a shared [DriveItem](../resources/driveitem.md) or a collection of shared items by using a **shareId** or sharing URL.</span></span>

<span data-ttu-id="eb8ff-104">この API で共有の URL を使用するには、アプリで [URL を共有のトークンに変換する](#encoding-sharing-urls)必要があります。</span><span class="sxs-lookup"><span data-stu-id="eb8ff-104">To use a sharing URL with this API, your app needs to [transform the URL into a sharing token](#encoding-sharing-urls).</span></span>

## <a name="permissions"></a><span data-ttu-id="eb8ff-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="eb8ff-105">Permissions</span></span>

<span data-ttu-id="eb8ff-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="eb8ff-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eb8ff-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="eb8ff-108">Permission type</span></span>      | <span data-ttu-id="eb8ff-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="eb8ff-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="eb8ff-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="eb8ff-110">Delegated (work or school account)</span></span> | <span data-ttu-id="eb8ff-111">Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eb8ff-111">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="eb8ff-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="eb8ff-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eb8ff-113">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eb8ff-113">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="eb8ff-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="eb8ff-114">Application</span></span> | <span data-ttu-id="eb8ff-115">Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eb8ff-115">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="eb8ff-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="eb8ff-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /shares/{shareIdOrEncodedSharingUrl}
```

### <a name="path-parameters"></a><span data-ttu-id="eb8ff-117">パス パラメーター</span><span class="sxs-lookup"><span data-stu-id="eb8ff-117">Path parameters</span></span>

| <span data-ttu-id="eb8ff-118">パラメーター名</span><span class="sxs-lookup"><span data-stu-id="eb8ff-118">Parameter Name</span></span>                 | <span data-ttu-id="eb8ff-119">値</span><span class="sxs-lookup"><span data-stu-id="eb8ff-119">Value</span></span>    | <span data-ttu-id="eb8ff-120">説明</span><span class="sxs-lookup"><span data-stu-id="eb8ff-120">Description</span></span>                                                                         |
|:-------------------------------|:---------|:------------------------------------------------------------------------------------|
| <span data-ttu-id="eb8ff-121">**Sharingidorencodedsharingurl**</span><span class="sxs-lookup"><span data-stu-id="eb8ff-121">**shareIdOrEncodedSharingUrl**</span></span> | `string` | <span data-ttu-id="eb8ff-122">必須。</span><span class="sxs-lookup"><span data-stu-id="eb8ff-122">Required.</span></span> <span data-ttu-id="eb8ff-123">API によって返される共有トークン、または適切にエンコードされた共有 URL。</span><span class="sxs-lookup"><span data-stu-id="eb8ff-123">A sharing token as returned by the API or a properly encoded sharing URL.</span></span> |

### <a name="encoding-sharing-urls"></a><span data-ttu-id="eb8ff-124">共有 URL をエンコードする</span><span class="sxs-lookup"><span data-stu-id="eb8ff-124">Encoding sharing URLs</span></span>

<span data-ttu-id="eb8ff-125">共有 URL をエンコードするには、次のロジックを使用します。</span><span class="sxs-lookup"><span data-stu-id="eb8ff-125">To encode a sharing URL, use the following logic:</span></span>

1. <span data-ttu-id="eb8ff-126">まず、base64 を使用して URL をエンコードします。</span><span class="sxs-lookup"><span data-stu-id="eb8ff-126">First, use base64 encode the URL.</span></span>
2. <span data-ttu-id="eb8ff-127">base64 でエンコードされた結果を [unpadded base64url 形式](https://en.wikipedia.org/wiki/Base64)に変換します (値の末尾から `=` 文字を削除し、`/` を `_`、`+` を `-` に置き換える)。</span><span class="sxs-lookup"><span data-stu-id="eb8ff-127">Convert the base64 encoded result to [unpadded base64url format](https://en.wikipedia.org/wiki/Base64) by removing `=` characters from the end of the value, replacing `/` with `_` and `+` with `-`.)</span></span>
3. <span data-ttu-id="eb8ff-128">文字列の先頭に `u!` を追加します。</span><span class="sxs-lookup"><span data-stu-id="eb8ff-128">Append `u!` to be beginning of the string.</span></span>

<span data-ttu-id="eb8ff-129">URL を C# でエンコードする例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="eb8ff-129">As an example, to encode a URL in C#:</span></span>

```csharp
string sharingUrl = "https://onedrive.live.com/redir?resid=1231244193912!12&authKey=1201919!12921!1";
string base64Value = System.Convert.ToBase64String(System.Text.Encoding.UTF8.GetBytes(sharingUrl));
string encodedUrl = "u!" + base64Value.TrimEnd('=').Replace('/','_').Replace('+','-');
```

## <a name="optional-request-headers"></a><span data-ttu-id="eb8ff-130">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="eb8ff-130">Optional request headers</span></span>

| <span data-ttu-id="eb8ff-131">名前</span><span class="sxs-lookup"><span data-stu-id="eb8ff-131">Name</span></span>       | <span data-ttu-id="eb8ff-132">型</span><span class="sxs-lookup"><span data-stu-id="eb8ff-132">Type</span></span>   | <span data-ttu-id="eb8ff-133">説明</span><span class="sxs-lookup"><span data-stu-id="eb8ff-133">Description</span></span>                                                    |
|:-----------|:-------|:---------------------------------------------------------------|
| <span data-ttu-id="eb8ff-134">**Prefer**</span><span class="sxs-lookup"><span data-stu-id="eb8ff-134">**Prefer**</span></span> | <span data-ttu-id="eb8ff-135">string</span><span class="sxs-lookup"><span data-stu-id="eb8ff-135">string</span></span> | <span data-ttu-id="eb8ff-136">省略可能。</span><span class="sxs-lookup"><span data-stu-id="eb8ff-136">Optional.</span></span> <span data-ttu-id="eb8ff-137">以下に記載され`prefer`ている値の1つに設定します。</span><span class="sxs-lookup"><span data-stu-id="eb8ff-137">Set to one of the `prefer` values documented below.</span></span>  |

### <a name="prefer-header-values"></a><span data-ttu-id="eb8ff-138">ヘッダー値を優先する</span><span class="sxs-lookup"><span data-stu-id="eb8ff-138">Prefer header values</span></span>

| <span data-ttu-id="eb8ff-139">名前</span><span class="sxs-lookup"><span data-stu-id="eb8ff-139">Name</span></span>                          | <span data-ttu-id="eb8ff-140">説明</span><span class="sxs-lookup"><span data-stu-id="eb8ff-140">Description</span></span>                                                                                             |
|:------------------------------|:--------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="eb8ff-141">redeemSharingLink</span><span class="sxs-lookup"><span data-stu-id="eb8ff-141">redeemSharingLink</span></span>             | <span data-ttu-id="eb8ff-142">共有リンク\*\*\*\* の場合は、発信者に、アイテムへの永続的なアクセス権を付与します。</span><span class="sxs-lookup"><span data-stu-id="eb8ff-142">If the **shareIdOrEncodedSharingUrl** is a sharing link, grant the caller durable access to the item</span></span>    |
| <span data-ttu-id="eb8ff-143">redeemSharingLinkIfNecessary</span><span class="sxs-lookup"><span data-stu-id="eb8ff-143">redeemSharingLinkIfNecessary</span></span>  | <span data-ttu-id="eb8ff-144">RedeemSharingLink と同じですが、この要求の期間だけアクセスが許可されることが保証されます。</span><span class="sxs-lookup"><span data-stu-id="eb8ff-144">Same as redeemSharingLink, but access is only guaranteed to be granted for the duration of this request</span></span> |

<span data-ttu-id="eb8ff-145">redeemSharingLink は、発信者と同等であると考えて、共有リンクに移動します (共有ジェスチャに同意します)。 redeemSharingLinkIfNecessary は、リンクの場所を単にピークすることを目的としたシナリオに対して使用されます。metadata.</span><span class="sxs-lookup"><span data-stu-id="eb8ff-145">redeemSharingLink should be considered equivalent to the caller navigating to the sharing link the browser (accepting the sharing gesture), whereas redeemSharingLinkIfNecessary is intended for scenarios where the intention is simply to peek at the link's metadata.</span></span>

## <a name="response"></a><span data-ttu-id="eb8ff-146">応答</span><span class="sxs-lookup"><span data-stu-id="eb8ff-146">Response</span></span>

<span data-ttu-id="eb8ff-147">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [sharedDriveItem](../resources/shareddriveitem.md) リソースを返します。</span><span class="sxs-lookup"><span data-stu-id="eb8ff-147">If successful, this method returns a `200 OK` response code and a [sharedDriveItem](../resources/shareddriveitem.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eb8ff-148">例</span><span class="sxs-lookup"><span data-stu-id="eb8ff-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="eb8ff-149">要求</span><span class="sxs-lookup"><span data-stu-id="eb8ff-149">Request</span></span>

<span data-ttu-id="eb8ff-150">以下は、共有アイテムを取得する要求の例です。</span><span class="sxs-lookup"><span data-stu-id="eb8ff-150">Here is an example of the request to retrieve a shared item:</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="eb8ff-151">プロトコル</span><span class="sxs-lookup"><span data-stu-id="eb8ff-151">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-shared-root" } -->

```http
GET /shares/{shareIdOrEncodedSharingUrl}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="eb8ff-152">C#</span><span class="sxs-lookup"><span data-stu-id="eb8ff-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-shared-root-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="eb8ff-153">Javascript</span><span class="sxs-lookup"><span data-stu-id="eb8ff-153">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-shared-root-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="eb8ff-154">目的-C</span><span class="sxs-lookup"><span data-stu-id="eb8ff-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-shared-root-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="eb8ff-155">応答</span><span class="sxs-lookup"><span data-stu-id="eb8ff-155">Response</span></span>

<span data-ttu-id="eb8ff-156">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="eb8ff-156">Here is an example of the response.</span></span>

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

## <a name="access-the-shared-item-directly"></a><span data-ttu-id="eb8ff-157">共有アイテムに直接アクセスする</span><span class="sxs-lookup"><span data-stu-id="eb8ff-157">Access the shared item directly</span></span>

<span data-ttu-id="eb8ff-p104">[**SharedDriveItem**](../resources/shareddriveitem.md) には、いくつかの有用な情報が含まれていますが、ほとんどのアプリは、共有の [DriveItem](../resources/driveitem.md)に直接アクセスする必要があります。**SharedDriveItem** リソースには、共有アイテムのスコープ内でコンテンツにアクセスできる、**root** と **items** のリレーションシップが含まれています。</span><span class="sxs-lookup"><span data-stu-id="eb8ff-p104">While the [**SharedDriveItem**](../resources/shareddriveitem.md) contains some useful information, most apps will want to directly access the shared [DriveItem](../resources/driveitem.md). The **SharedDriveItem** resource includes a **root** and **items** relationships which can access content within the scope of the shared item.</span></span>

## <a name="example-single-file"></a><span data-ttu-id="eb8ff-160">例 (単一ファイル)</span><span class="sxs-lookup"><span data-stu-id="eb8ff-160">Example (single file)</span></span>

### <a name="request"></a><span data-ttu-id="eb8ff-161">要求</span><span class="sxs-lookup"><span data-stu-id="eb8ff-161">Request</span></span>

<span data-ttu-id="eb8ff-162">**driveItem** リレーションシップを要求することで、共有された **DriveItem** が返されます。</span><span class="sxs-lookup"><span data-stu-id="eb8ff-162">By requesting the **driveItem** relationship, the **DriveItem** that was shared will be returned.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="eb8ff-163">プロトコル</span><span class="sxs-lookup"><span data-stu-id="eb8ff-163">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-shared-driveitem" } -->

```http
GET /shares/{shareIdOrUrl}/driveItem
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="eb8ff-164">C#</span><span class="sxs-lookup"><span data-stu-id="eb8ff-164">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-shared-driveitem-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="eb8ff-165">Javascript</span><span class="sxs-lookup"><span data-stu-id="eb8ff-165">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-shared-driveitem-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="eb8ff-166">目的-C</span><span class="sxs-lookup"><span data-stu-id="eb8ff-166">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-shared-driveitem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="eb8ff-167">応答</span><span class="sxs-lookup"><span data-stu-id="eb8ff-167">Response</span></span>

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

## <a name="example-shared-folder"></a><span data-ttu-id="eb8ff-168">例 (共有フォルダー)</span><span class="sxs-lookup"><span data-stu-id="eb8ff-168">Example (shared folder)</span></span>

### <a name="request"></a><span data-ttu-id="eb8ff-169">要求</span><span class="sxs-lookup"><span data-stu-id="eb8ff-169">Request</span></span>

<span data-ttu-id="eb8ff-170">**driveItem** リレーションシップを要求して、**children** コレクションを展開することで、共有されている **DriveItem** が共有フォルダー内のファイルとともに返されます。</span><span class="sxs-lookup"><span data-stu-id="eb8ff-170">By requesting the **driveItem** relationship and expanding the **children** collection, the **DriveItem** that was shared will be returned along with the files within the shared folder.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="eb8ff-171">プロトコル</span><span class="sxs-lookup"><span data-stu-id="eb8ff-171">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-shared-driveitem-expand-children" } -->

```http
GET /shares/{shareIdOrUrl}/driveItem?$expand=children
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="eb8ff-172">C#</span><span class="sxs-lookup"><span data-stu-id="eb8ff-172">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-shared-driveitem-expand-children-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="eb8ff-173">Javascript</span><span class="sxs-lookup"><span data-stu-id="eb8ff-173">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-shared-driveitem-expand-children-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="eb8ff-174">目的-C</span><span class="sxs-lookup"><span data-stu-id="eb8ff-174">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-shared-driveitem-expand-children-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="eb8ff-175">応答</span><span class="sxs-lookup"><span data-stu-id="eb8ff-175">Response</span></span>

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

## <a name="error-responses"></a><span data-ttu-id="eb8ff-176">エラー応答</span><span class="sxs-lookup"><span data-stu-id="eb8ff-176">Error Responses</span></span>

<span data-ttu-id="eb8ff-177">エラーがどのような形で返されるかについては、「[エラー応答][error-response]」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="eb8ff-177">Read the [Error Responses][error-response] topic for more information about how errors are returned.</span></span>

## <a name="remarks"></a><span data-ttu-id="eb8ff-178">備考</span><span class="sxs-lookup"><span data-stu-id="eb8ff-178">Remarks</span></span>

* <span data-ttu-id="eb8ff-179">OneDrive for Business と SharePoint の場合、Shares API には常に認証が必要です。また、ユーザー コンテキストを使用せずに、匿名で共有コンテンツにアクセスするためには使用できません。</span><span class="sxs-lookup"><span data-stu-id="eb8ff-179">For OneDrive for Business and SharePoint, the Shares API always requires authentication and cannot be used to access anonymously shared content without a user context.</span></span>

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
