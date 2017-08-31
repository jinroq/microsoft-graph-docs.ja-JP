# <a name="get-a-special-folder-by-name"></a><span data-ttu-id="7d7d0-101">名前で特殊フォルダーを取得する</span><span class="sxs-lookup"><span data-stu-id="7d7d0-101">Get a special folder by name</span></span>

<span data-ttu-id="7d7d0-102">特殊なコレクションを使用して、名前で特殊フォルダーにアクセスします。</span><span class="sxs-lookup"><span data-stu-id="7d7d0-102">Use the special collection to access a special folder by name.</span></span>

<span data-ttu-id="7d7d0-p101">特殊フォルダーは、フォルダーを (ローカライズが必要となる) パスで探したり、ID を持つフォルダーを参照したりせずに、OneDrive の既知のフォルダーにアクセスするための、単純なエイリアスを提供します。特殊フォルダーの名前が変更されたりドライブ内の別の場所に移動されたりした場合でも、この構文はそのフォルダーを返し続けます。</span><span class="sxs-lookup"><span data-stu-id="7d7d0-p101">Special folders provide simple aliases to access well-known folders in OneDrive without the need to look up the folder by path (which would require localization), or reference the folder with an ID. If a special folder is renamed or moved to another location within the drive, this syntax will continue to find that folder.</span></span>

<span data-ttu-id="7d7d0-p102">特殊なフォルダーは、まだ存在していない場合、アプリケーションが最初に書き込みを試行したときに自動的に作成されます。ユーザーが削除した場合は、もう一度書き込まれたときに再作成されます。</span><span class="sxs-lookup"><span data-stu-id="7d7d0-p102">Special folders are automatically created the first time an application attempts to write to one, if it doesn't already exist. If a user deletes one, it is recreated when written to again.</span></span>

><span data-ttu-id="7d7d0-107">**注:**読み取り専用のアクセス許可が付与されているときに、存在していない特殊フォルダーを要求すると、`403 Forbidden` エラーが返されます。</span><span class="sxs-lookup"><span data-stu-id="7d7d0-107">**Note:**  If you have read-only permissions and request a special folder that doesn't exist, you'll receive a `403 Forbidden` error.</span></span>

## <a name="permissions"></a><span data-ttu-id="7d7d0-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="7d7d0-108">Permissions</span></span>

<span data-ttu-id="7d7d0-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7d7d0-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="7d7d0-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7d7d0-111">Permission type</span></span>                        | <span data-ttu-id="7d7d0-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="7d7d0-112">Permissions (from least to most privileged)</span></span>                                                           |
|:--------------------------------------|:------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="7d7d0-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7d7d0-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="7d7d0-114">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7d7d0-114">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |
|<span data-ttu-id="7d7d0-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7d7d0-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7d7d0-116">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Files.ReadWrite.AppFolder</span><span class="sxs-lookup"><span data-stu-id="7d7d0-116">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Files.ReadWrite.AppFolder</span></span>           |
|<span data-ttu-id="7d7d0-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7d7d0-117">Application</span></span>                            | <span data-ttu-id="7d7d0-118">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7d7d0-118">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>                              |

## <a name="http-request"></a><span data-ttu-id="7d7d0-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7d7d0-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/special/{name}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="7d7d0-120">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="7d7d0-120">Optional query parameters</span></span>

<span data-ttu-id="7d7d0-121">このメソッドは、応答をカスタマイズするための `$expand` および `$select` [OData クエリ パラメーター](../../../concepts/query_parameters.md)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="7d7d0-121">This method supports the `$expand` and `$select` [OData Query Parameters](../../../concepts/query_parameters.md) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7d7d0-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7d7d0-122">Request headers</span></span>

| <span data-ttu-id="7d7d0-123">名前</span><span class="sxs-lookup"><span data-stu-id="7d7d0-123">Name</span></span>          | <span data-ttu-id="7d7d0-124">型</span><span class="sxs-lookup"><span data-stu-id="7d7d0-124">Type</span></span>   | <span data-ttu-id="7d7d0-125">説明</span><span class="sxs-lookup"><span data-stu-id="7d7d0-125">Description</span></span>               |
|:--------------|:-------|:--------------------------|
| <span data-ttu-id="7d7d0-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="7d7d0-126">Authorization</span></span> | <span data-ttu-id="7d7d0-127">string</span><span class="sxs-lookup"><span data-stu-id="7d7d0-127">string</span></span> | <span data-ttu-id="7d7d0-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="7d7d0-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7d7d0-130">要求本文</span><span class="sxs-lookup"><span data-stu-id="7d7d0-130">Request body</span></span>

<span data-ttu-id="7d7d0-131">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="7d7d0-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7d7d0-132">応答</span><span class="sxs-lookup"><span data-stu-id="7d7d0-132">Response</span></span>

<span data-ttu-id="7d7d0-133">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [driveItem](../resources/driveitem.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="7d7d0-133">If successful, this method returns a `200 OK` response code and a [driveItem](../resources/driveitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7d7d0-134">例</span><span class="sxs-lookup"><span data-stu-id="7d7d0-134">Example</span></span>

##### <a name="request"></a><span data-ttu-id="7d7d0-135">要求</span><span class="sxs-lookup"><span data-stu-id="7d7d0-135">Request</span></span>

<span data-ttu-id="7d7d0-136">以下はユーザーのドライブの要求例です。</span><span class="sxs-lookup"><span data-stu-id="7d7d0-136">Here is an example of the request for the user's drives.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_drive_special"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/special/{name}
```

##### <a name="response"></a><span data-ttu-id="7d7d0-137">応答</span><span class="sxs-lookup"><span data-stu-id="7d7d0-137">Response</span></span>
<span data-ttu-id="7d7d0-138">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="7d7d0-138">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.driveItem"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "folder": { },
  "id": "s!lkjqwlkj124912049an",
  "name": "Photos",
  "specialFolder": { "name": "photos" },
  "webUrl": "https://contoso-my.sharepoint.com/personal/rgregg_contoso_com/Documents/Photos",
}
```

## <a name="remarks"></a><span data-ttu-id="7d7d0-139">注釈</span><span class="sxs-lookup"><span data-stu-id="7d7d0-139">Remarks</span></span>

<span data-ttu-id="7d7d0-140">特殊フォルダーの子を要求する場合は、`children` コレクションを要求するか、子コレクションを展開する [$expand](../../../concepts/query_parameters.md) オプションを使用します。</span><span class="sxs-lookup"><span data-stu-id="7d7d0-140">To request the children of a special folder, you can request the `children` collection or use the [expand](../../../concepts/query_parameters.md) option to expand the children collection.</span></span>


<!-- {
  "type": "#page.annotation",
  "description": "List drives",
  "keywords": "",
  "section": "documentation",
  "tocPath": "OneDrive/Drive/Get special folder"
}-->
