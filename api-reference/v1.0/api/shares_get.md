# <a name="accessing-shared-driveitems"></a><span data-ttu-id="8e583-101">共有 DriveItems へのアクセス</span><span class="sxs-lookup"><span data-stu-id="8e583-101">Accessing shared DriveItems</span></span>

<span data-ttu-id="8e583-102">**shareId** または共有の URL を使用して、共有 [DriveItem](../resources/driveitem.md) または共有アイテムのコレクションにアクセスします。</span><span class="sxs-lookup"><span data-stu-id="8e583-102">Access a shared [DriveItem](../resources/driveitem.md) or a collection of shared items by using a **shareId** or sharing URL.</span></span>

<span data-ttu-id="8e583-103">この API で共有の URL を使用するには、アプリで [URL を共有のトークンに変換する](#transform-a-sharing-url)必要があります。</span><span class="sxs-lookup"><span data-stu-id="8e583-103">To use a sharing URL with this API, your app needs to [transform the URL into a sharing token](#transform-a-sharing-url).</span></span>

## <a name="permissions"></a><span data-ttu-id="8e583-104">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="8e583-104">Permissions</span></span>

<span data-ttu-id="8e583-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8e583-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="8e583-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8e583-107">Permission type</span></span>      | <span data-ttu-id="8e583-108">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="8e583-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8e583-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8e583-109">Delegated (work or school account)</span></span> | <span data-ttu-id="8e583-110">Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8e583-110">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="8e583-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8e583-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8e583-112">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8e583-112">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="8e583-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8e583-113">Application</span></span> | <span data-ttu-id="8e583-114">Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8e583-114">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8e583-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8e583-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /shares/{sharingIdOrUrl}
```

## <a name="request-body"></a><span data-ttu-id="8e583-116">要求本文</span><span class="sxs-lookup"><span data-stu-id="8e583-116">Request body</span></span>
<span data-ttu-id="8e583-117">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="8e583-117">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8e583-118">応答</span><span class="sxs-lookup"><span data-stu-id="8e583-118">Response</span></span>

<span data-ttu-id="8e583-119">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [sharedDriveItem](../resources/shareddriveitem.md) リソースを返します。</span><span class="sxs-lookup"><span data-stu-id="8e583-119">If successful, this method returns a `200 OK` response code and a [sharedDriveItem](../resources/shareddriveitem.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8e583-120">例</span><span class="sxs-lookup"><span data-stu-id="8e583-120">Example</span></span>

##### <a name="request"></a><span data-ttu-id="8e583-121">要求</span><span class="sxs-lookup"><span data-stu-id="8e583-121">Request</span></span>

<span data-ttu-id="8e583-122">以下は、共有アイテムを取得する要求の例です。</span><span class="sxs-lookup"><span data-stu-id="8e583-122">Here is an example of the request to retrieve a shared item:</span></span>

<!-- {
  "blockType": "request",
  "name": "get_shares_by_url"
}-->
```http
GET https://graph.microsoft.com/v1.0/shares/{shareIdOrUrl}
```
##### <a name="response"></a><span data-ttu-id="8e583-123">応答</span><span class="sxs-lookup"><span data-stu-id="8e583-123">Response</span></span>

<span data-ttu-id="8e583-124">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="8e583-124">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.sharedDriveItem"
} -->
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

## <a name="access-the-shared-item-directly"></a><span data-ttu-id="8e583-125">共有アイテムに直接アクセスする</span><span class="sxs-lookup"><span data-stu-id="8e583-125">Access the shared item directly</span></span>

<span data-ttu-id="8e583-p102">[**SharedDriveItem**](../resources/shareddriveitem.md) には、いくつかの有用な情報が含まれていますが、ほとんどのアプリは、共有の [DriveItem](../resources/driveitem.md)に直接アクセスする必要があります。**SharedDriveItem** リソースには、共有アイテムのスコープ内でコンテンツにアクセスできる、**root** と **items** のリレーションシップが含まれています。</span><span class="sxs-lookup"><span data-stu-id="8e583-p102">While the [**SharedDriveItem**](../resources/shareddriveitem.md) contains some useful information, most apps will want to directly access the shared [DriveItem](../resources/driveitem.md). The **SharedDriveItem** resource includes a **root** and **items** relationships which can access content within the scope of the shared item.</span></span>

## <a name="example-single-file"></a><span data-ttu-id="8e583-128">例 (単一ファイル)</span><span class="sxs-lookup"><span data-stu-id="8e583-128">Example (single file)</span></span>

##### <a name="request"></a><span data-ttu-id="8e583-129">要求</span><span class="sxs-lookup"><span data-stu-id="8e583-129">Request</span></span>

<span data-ttu-id="8e583-130">**root** リレーションシップを要求することで、共有された **DriveItem** が返されます。</span><span class="sxs-lookup"><span data-stu-id="8e583-130">By requesting the **root** relationship, the **DriveItem** that was shared will be returned.</span></span>

```http
GET https://graph.microsoft.com/v1.0/shares/{shareIdOrUrl}/root
```

##### <a name="response"></a><span data-ttu-id="8e583-131">応答</span><span class="sxs-lookup"><span data-stu-id="8e583-131">Response</span></span>

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

## <a name="example-shared-folder"></a><span data-ttu-id="8e583-132">例 (共有フォルダー)</span><span class="sxs-lookup"><span data-stu-id="8e583-132">Example (shared folder)</span></span>

##### <a name="request"></a><span data-ttu-id="8e583-133">要求</span><span class="sxs-lookup"><span data-stu-id="8e583-133">Request</span></span>

<span data-ttu-id="8e583-134">**root** リレーションシップを要求して、**children** コレクションを展開することで、共有されている **DriveItem** が共有フォルダー内のファイルとともに返されます。</span><span class="sxs-lookup"><span data-stu-id="8e583-134">By requesting the **root** relationship and expanding the **children** collection, the **DriveItem** that was shared will be returned along with the files within the shared folder.</span></span>

```http
GET https://graph.microsoft.com/v1.0/shares/{shareIdOrUrl}/root?$expand=children
```

##### <a name="response"></a><span data-ttu-id="8e583-135">応答</span><span class="sxs-lookup"><span data-stu-id="8e583-135">Response</span></span>

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "id": "9FFFDB3C-5B87-4062-9606-1B008CA88E44",
  "name": "Contoso Project",
  "eTag": "2246BD2D-7811-4660-BD0F-1CF36133677B,1",
  "folder": {}
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

## <a name="transform-a-sharing-url"></a><span data-ttu-id="8e583-136">共有の URL を変換する</span><span class="sxs-lookup"><span data-stu-id="8e583-136">Transform a sharing URL</span></span>

<span data-ttu-id="8e583-137">**shares** API を使用して共有の URL にアクセスするには、URL を共有のトークンに変換する必要があります。</span><span class="sxs-lookup"><span data-stu-id="8e583-137">To access a sharing URL using the **shares** API, the URL needs to be transformed into a sharing token.</span></span>

<span data-ttu-id="8e583-138">URL を共有のトークンに変化するには:</span><span class="sxs-lookup"><span data-stu-id="8e583-138">To transform a URL into a sharing token:</span></span>

1. <span data-ttu-id="8e583-139">共有の URL を Base64 エンコードします。</span><span class="sxs-lookup"><span data-stu-id="8e583-139">Base64 encode the sharing URL.</span></span>
2. <span data-ttu-id="8e583-140">次に示すように、base64 でエンコードしたデータを[パディングされていない base64url 形式](https://en.wikipedia.org/wiki/Base64)に変換します。</span><span class="sxs-lookup"><span data-stu-id="8e583-140">Convert the base64 encoded data to [unpadded base64url format](https://en.wikipedia.org/wiki/Base64) by:</span></span>
  1. <span data-ttu-id="8e583-141">文字列から、末尾の `=` 文字をトリミングします。</span><span class="sxs-lookup"><span data-stu-id="8e583-141">Trim trailing `=` characters from the string</span></span>
  2. <span data-ttu-id="8e583-142">安全でない URL 文字を同等の文字に置き換えます (`/` を `_` に、`+` を `-` に置換します)。</span><span class="sxs-lookup"><span data-stu-id="8e583-142">Replace unsafe URL characters with an equivalent character; replace `/` with `_` and `+` with `-`.</span></span>
3. <span data-ttu-id="8e583-143">文字列の先頭に `u!` を追加します。</span><span class="sxs-lookup"><span data-stu-id="8e583-143">Append `u!` to the beginning of the string.</span></span>

<span data-ttu-id="8e583-144">たとえば、次に示す C# メソッドにより、入力文字列を共有のトークンに変換します。</span><span class="sxs-lookup"><span data-stu-id="8e583-144">For example, the following C# method transforms an input string into a sharing token:</span></span>

```csharp
string UrlToSharingToken(string inputUrl) {
  var base64Value = System.Convert.ToBase64String(System.Text.Encoding.UTF8.GetBytes(inputUrl));
  return "u!" + base64Value.TrimEnd('=').Replace('/','_').Replace('+','-');
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update permission",
  "keywords": "",
  "section": "documentation",
  "tocPath": "OneDrive/Item/Update permission"
}-->
