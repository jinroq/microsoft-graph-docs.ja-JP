# <a name="notebook-getrecentnotebooks"></a><span data-ttu-id="9ee71-101">ノートブック: getRecentNotebooks</span><span class="sxs-lookup"><span data-stu-id="9ee71-101">notebook: getRecentNotebooks</span></span>

<span data-ttu-id="9ee71-102">サインインしたユーザーによってアクセスされた [recentNotebook](../resources/recentnotebook.md) インスタンスの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="9ee71-102">Get a list of [recentNotebook](../resources/recentnotebook.md) instances that have been accessed by the signed-in user.</span></span>

## <a name="permissions"></a><span data-ttu-id="9ee71-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="9ee71-103">Permissions</span></span>
<span data-ttu-id="9ee71-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9ee71-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="9ee71-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9ee71-106">Permission type</span></span>      | <span data-ttu-id="9ee71-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="9ee71-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9ee71-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9ee71-108">Delegated (work or school account)</span></span> | <span data-ttu-id="9ee71-109">Notes.Create、Notes.Read、Notes.ReadWrite、Notes.Read.All、Notes.ReadWrite.All、</span><span class="sxs-lookup"><span data-stu-id="9ee71-109">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>|
|<span data-ttu-id="9ee71-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9ee71-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9ee71-111">Notes.Create、Notes.Read、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9ee71-111">Notes.Create, Notes.Read, Notes.ReadWrite</span></span> |
|<span data-ttu-id="9ee71-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9ee71-112">Application</span></span> | <span data-ttu-id="9ee71-113">Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ee71-113">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9ee71-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9ee71-114">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/notebooks/getRecentNotebooks(includePersonalNotebooks=includePersonalNotebooks-value)
GET /users/<id | userPrincipalName>/onenote/notebooks/getRecentNotebooks(includePersonalNotebooks=includePersonalNotebooks-value)
```

<span data-ttu-id="9ee71-115">ユーザーの `<id | userPrincipalName>` は、要求を行うために使用された承認トークンにおいてエンコードされたユーザーと一致しなければなりません。</span><span class="sxs-lookup"><span data-stu-id="9ee71-115">The `<id | userPrincipalName>` for the user must match the user encoded in the authorization token used to make the request.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9ee71-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9ee71-116">Request headers</span></span>
| <span data-ttu-id="9ee71-117">名前</span><span class="sxs-lookup"><span data-stu-id="9ee71-117">Name</span></span>       | <span data-ttu-id="9ee71-118">説明</span><span class="sxs-lookup"><span data-stu-id="9ee71-118">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="9ee71-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="9ee71-119">Authorization</span></span>  | <span data-ttu-id="9ee71-120">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="9ee71-120">Bearer {code}</span></span>|

## <a name="request-parameters"></a><span data-ttu-id="9ee71-121">要求パラメーター</span><span class="sxs-lookup"><span data-stu-id="9ee71-121">Request parameters</span></span>
<span data-ttu-id="9ee71-122">要求 URL に、次のクエリ パラメーターを値で指定します。</span><span class="sxs-lookup"><span data-stu-id="9ee71-122">In the request URL, provide following query parameters with values.</span></span>

| <span data-ttu-id="9ee71-123">パラメーター</span><span class="sxs-lookup"><span data-stu-id="9ee71-123">Parameter</span></span>    | <span data-ttu-id="9ee71-124">型</span><span class="sxs-lookup"><span data-stu-id="9ee71-124">Type</span></span>   |<span data-ttu-id="9ee71-125">説明</span><span class="sxs-lookup"><span data-stu-id="9ee71-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9ee71-126">includePersonalNotebooks</span><span class="sxs-lookup"><span data-stu-id="9ee71-126">includePersonalNotebooks</span></span>|<span data-ttu-id="9ee71-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ee71-127">Boolean</span></span>|<span data-ttu-id="9ee71-128">ユーザーが所有しているノートブックを含みます。</span><span class="sxs-lookup"><span data-stu-id="9ee71-128">Include notebooks owned by the user.</span></span> <span data-ttu-id="9ee71-129">ユーザーが所有しているノートブックを含むには、`true` に設定します。そうでない場合は、`false` に設定します。</span><span class="sxs-lookup"><span data-stu-id="9ee71-129">Set to `true` to include notebooks owned by the user; otherwise, set to `false`.</span></span> <span data-ttu-id="9ee71-130">`includePersonalNotebooks` パラメーターを含めない場合、要求は `400` エラー応答を返します。</span><span class="sxs-lookup"><span data-stu-id="9ee71-130">If you don't include the `includePersonalNotebooks` parameter, your request will return a `400` error response.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9ee71-131">要求本文</span><span class="sxs-lookup"><span data-stu-id="9ee71-131">Request body</span></span>
<span data-ttu-id="9ee71-132">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="9ee71-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9ee71-133">応答</span><span class="sxs-lookup"><span data-stu-id="9ee71-133">Response</span></span>
<span data-ttu-id="9ee71-134">正常な応答は **recentNotebooks** の JSON コレクションを含む `200 OK` を返します。</span><span class="sxs-lookup"><span data-stu-id="9ee71-134">A successful response returns a `200 OK` that contains a JSON collection of **recentNotebooks**.</span></span>

## <a name="example"></a><span data-ttu-id="9ee71-135">例</span><span class="sxs-lookup"><span data-stu-id="9ee71-135">Example</span></span>
<span data-ttu-id="9ee71-136">次の例は、この API を呼び出す方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="9ee71-136">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="9ee71-137">要求</span><span class="sxs-lookup"><span data-stu-id="9ee71-137">Request</span></span>
<span data-ttu-id="9ee71-138">次の例は要求を示しています。</span><span class="sxs-lookup"><span data-stu-id="9ee71-138">The following example shows the request.</span></span>
<!-- { "blockType": "request", "name": "recent_notebooks", "scopes": "notes.read" } -->
```http
GET https://graph.microsoft.com/v1.0/onenote/notebooks/getrecentnotebooks(includePersonalNotebooks=true)
```

#### <a name="response"></a><span data-ttu-id="9ee71-139">応答</span><span class="sxs-lookup"><span data-stu-id="9ee71-139">Response</span></span>
<span data-ttu-id="9ee71-140">次の例は応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="9ee71-140">The following example shows the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.notebook",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-Length: 1110

{
  "value":[
    {
      "name":"Personal Notebook","lastAccessedTime":"timestamp","links":{
        "oneNoteClientUrl":{
          "href":"onenote:href-value"
        },"oneNoteWebUrl":{
          "href":"href-value"
        }
      },"sourceService":"OneDrive"
    },{
      "name":"Team Shared Notebook","lastAccessedTime":"timestamp","links":{
        "oneNoteClientUrl":{
          "href":"onenote:href-value"
        },"oneNoteWebUrl":{
          "href":"href-value"
        }
      },"sourceService":"OneDriveForBusiness"
    }
  ]
}
```
