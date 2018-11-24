# <a name="driveitem-preview"></a><span data-ttu-id="165d2-101">driveItem: プレビュー</span><span class="sxs-lookup"><span data-stu-id="165d2-101">driveItem: preview</span></span>

<span data-ttu-id="165d2-102">このアクションを使用すると、一時的なプレビューをレンダリングするためにアイテムを短時間の埋め込み可能な Url を取得できます。</span><span class="sxs-lookup"><span data-stu-id="165d2-102">This action allows you to obtain short-lived embeddable URLs for an item in order to render a temporary preview.</span></span>

<span data-ttu-id="165d2-103">有効期間の長い埋め込みリンクを取得する場合は、 [createLink][] API を使用してください。</span><span class="sxs-lookup"><span data-stu-id="165d2-103">If you want to obtain long-lived embeddable links, use the [createLink][] API instead.</span></span>

> <span data-ttu-id="165d2-104">**注:\*\*\*\*プレビュー**の動作は、現在 SharePoint およびビジネスのための OneDrive で使用可能なのみです。</span><span class="sxs-lookup"><span data-stu-id="165d2-104">**Note:** The **preview** action is currently only available on SharePoint and OneDrive for Business.</span></span>

[createLink]: driveItem_createLink.md

## <a name="permissions"></a><span data-ttu-id="165d2-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="165d2-106">Permissions</span></span>

<span data-ttu-id="165d2-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="165d2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="165d2-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="165d2-109">Permission type</span></span>                        | <span data-ttu-id="165d2-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="165d2-110">Permissions (from least to most privileged)</span></span>
|:---------------------------------------|:-------------------------------------------
| <span data-ttu-id="165d2-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="165d2-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="165d2-112">Files.Read、Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="165d2-112">Files.Read, Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>
| <span data-ttu-id="165d2-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="165d2-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="165d2-114">Files.Read、Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="165d2-114">Files.Read, Files.ReadWrite, Files.ReadWrite.All</span></span>
| <span data-ttu-id="165d2-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="165d2-115">Application</span></span>                            | <span data-ttu-id="165d2-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="165d2-116">Not supported.</span></span>

## <a name="http-request"></a><span data-ttu-id="165d2-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="165d2-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/preview
POST /groups/{groupId}/drive/items/{itemId}/preview
POST /me/drive/items/{itemId}/preview
POST /sites/{siteId}/drive/items/{itemId}/preview
POST /users/{userId}/drive/items/{itemId}/preview
POST /shares/{shareId}/driveItem/preview
```

## <a name="request-body"></a><span data-ttu-id="165d2-118">要求本文</span><span class="sxs-lookup"><span data-stu-id="165d2-118">Request body</span></span>

<span data-ttu-id="165d2-119">要求の本文では、アプリケーションが要求する埋め込み可能な URL のプロパティを定義します。</span><span class="sxs-lookup"><span data-stu-id="165d2-119">The body of the request defines properties of the embeddable URL your application is requesting.</span></span>
<span data-ttu-id="165d2-120">要求は、次のプロパティを含む JSON オブジェクトである必要があります。</span><span class="sxs-lookup"><span data-stu-id="165d2-120">The request should be a JSON object with the following properties.</span></span>

|   <span data-ttu-id="165d2-121">名前</span><span class="sxs-lookup"><span data-stu-id="165d2-121">Name</span></span>      |  <span data-ttu-id="165d2-122">型</span><span class="sxs-lookup"><span data-stu-id="165d2-122">Type</span></span>         | <span data-ttu-id="165d2-123">説明</span><span class="sxs-lookup"><span data-stu-id="165d2-123">Description</span></span>
|:------------|:--------------|:-----------------------------------------------
| <span data-ttu-id="165d2-124">page</span><span class="sxs-lookup"><span data-stu-id="165d2-124">page</span></span>        | <span data-ttu-id="165d2-125">文字列と番号</span><span class="sxs-lookup"><span data-stu-id="165d2-125">string/number</span></span> | <span data-ttu-id="165d2-126">省略可能。</span><span class="sxs-lookup"><span data-stu-id="165d2-126">Optional.</span></span> <span data-ttu-id="165d2-127">該当する場合に、開始するドキュメントのページ数です。</span><span class="sxs-lookup"><span data-stu-id="165d2-127">Page number of document to start at, if applicable.</span></span> <span data-ttu-id="165d2-128">将来使用する場合は、ZIP などのファイルの種類を文字列として指定します。</span><span class="sxs-lookup"><span data-stu-id="165d2-128">Specified as string for future use cases around file types such as ZIP.</span></span>
| <span data-ttu-id="165d2-129">ズーム</span><span class="sxs-lookup"><span data-stu-id="165d2-129">zoom</span></span>        | <span data-ttu-id="165d2-130">数値</span><span class="sxs-lookup"><span data-stu-id="165d2-130">number</span></span>        | <span data-ttu-id="165d2-131">省略可能。</span><span class="sxs-lookup"><span data-stu-id="165d2-131">Optional.</span></span> <span data-ttu-id="165d2-132">該当する場合に、開始するレベルを拡大します。</span><span class="sxs-lookup"><span data-stu-id="165d2-132">Zoom level to start at, if applicable.</span></span>

## <a name="response"></a><span data-ttu-id="165d2-133">応答</span><span class="sxs-lookup"><span data-stu-id="165d2-133">Response</span></span>

```json
{
    "getUrl": "https://www.onedrive.com/embed?foo=bar&bar=baz",
    "postParameters": "param1=value&param2=another%20value",
    "postUrl": "https://www.onedrive.com/embed_by_post"
}
```

<span data-ttu-id="165d2-134">応答は、次のプロパティを含む JSON オブジェクトになります。</span><span class="sxs-lookup"><span data-stu-id="165d2-134">The response will be a JSON object containing the following properties:</span></span>

| <span data-ttu-id="165d2-135">名前</span><span class="sxs-lookup"><span data-stu-id="165d2-135">Name</span></span>           | <span data-ttu-id="165d2-136">型</span><span class="sxs-lookup"><span data-stu-id="165d2-136">Type</span></span>   | <span data-ttu-id="165d2-137">説明</span><span class="sxs-lookup"><span data-stu-id="165d2-137">Description</span></span>
|:---------------|:-------|:---------------------------------------------------
| <span data-ttu-id="165d2-138">getUrl</span><span class="sxs-lookup"><span data-stu-id="165d2-138">getUrl</span></span>         | <span data-ttu-id="165d2-139">文字列</span><span class="sxs-lookup"><span data-stu-id="165d2-139">string</span></span> | <span data-ttu-id="165d2-140">HTTP の GET (iframe など) を使用して埋め込みの適切な URL</span><span class="sxs-lookup"><span data-stu-id="165d2-140">URL suitable for embedding using HTTP GET (iframes, etc.)</span></span>
| <span data-ttu-id="165d2-141">postUrl</span><span class="sxs-lookup"><span data-stu-id="165d2-141">postUrl</span></span>        | <span data-ttu-id="165d2-142">文字列</span><span class="sxs-lookup"><span data-stu-id="165d2-142">string</span></span> | <span data-ttu-id="165d2-143">HTTP POST を使用して埋め込みの適切な URL (フォーム ポスト、JS など)。</span><span class="sxs-lookup"><span data-stu-id="165d2-143">URL suitable for embedding using HTTP POST (form post, JS, etc.)</span></span>
| <span data-ttu-id="165d2-144">postParameters</span><span class="sxs-lookup"><span data-stu-id="165d2-144">postParameters</span></span> | <span data-ttu-id="165d2-145">文字列</span><span class="sxs-lookup"><span data-stu-id="165d2-145">string</span></span> | <span data-ttu-id="165d2-146">PostUrl を使用する場合は、POST のパラメーター</span><span class="sxs-lookup"><span data-stu-id="165d2-146">POST parameters to include if using postUrl</span></span>

<span data-ttu-id="165d2-147">GetUrl、postUrl、またはその両方は、指定したオプションの埋め込みのサポートの現在の状態によって返される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="165d2-147">Either getUrl, postUrl, or both might be returned depending on the current state of embed support for the specified options.</span></span>

<span data-ttu-id="165d2-148">として書式設定された文字列は、postParameters`application/x-www-form-urlencoded`と postUrl のコンテンツの種類へのポストを実行し、それに応じて設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="165d2-148">postParameters is a string formatted as `application/x-www-form-urlencoded`, and if performing a POST to the postUrl the content-type should be set accordingly.</span></span> <span data-ttu-id="165d2-149">例:</span><span class="sxs-lookup"><span data-stu-id="165d2-149">For example:</span></span>
```
POST https://www.onedrive.com/embed_by_post
Content-Type: application/x-www-form-urlencoded

param1=value&param2=another%20value
```

### <a name="pagezoom"></a><span data-ttu-id="165d2-150">ページ/ズーム</span><span class="sxs-lookup"><span data-stu-id="165d2-150">Page/zoom</span></span>

<span data-ttu-id="165d2-151">'ページ' と '拡大' オプションは、すべてのプレビュー アプリケーションを使用できない場合がありますが、プレビュー アプリケーションでサポートされている場合に適用されます。</span><span class="sxs-lookup"><span data-stu-id="165d2-151">The 'page' and 'zoom' options may not be available for all preview apps, but will be applied if the preview app supports it.</span></span>
