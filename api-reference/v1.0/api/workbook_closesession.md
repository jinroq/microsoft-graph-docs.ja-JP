# <a name="close-session"></a><span data-ttu-id="4dd8e-101">セッションを閉じる</span><span class="sxs-lookup"><span data-stu-id="4dd8e-101">Close Session</span></span>

<span data-ttu-id="4dd8e-102">この API を使用して、既存のブック セッションを閉じます。</span><span class="sxs-lookup"><span data-stu-id="4dd8e-102">Use this API to close an existing workbook session.</span></span> 

## <a name="permissions"></a><span data-ttu-id="4dd8e-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="4dd8e-103">Permissions</span></span>
<span data-ttu-id="4dd8e-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4dd8e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="4dd8e-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4dd8e-106">Permission type</span></span>      | <span data-ttu-id="4dd8e-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="4dd8e-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4dd8e-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="4dd8e-108">Delegated (work or school account)</span></span> | <span data-ttu-id="4dd8e-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4dd8e-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="4dd8e-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4dd8e-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4dd8e-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4dd8e-111">Not supported.</span></span>    |
|<span data-ttu-id="4dd8e-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4dd8e-112">Application</span></span> | <span data-ttu-id="4dd8e-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4dd8e-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4dd8e-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4dd8e-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/closeSession
workbook-session-id: {session-id}
```
## <a name="request-headers"></a><span data-ttu-id="4dd8e-115">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4dd8e-115">Request headers</span></span>
| <span data-ttu-id="4dd8e-116">名前</span><span class="sxs-lookup"><span data-stu-id="4dd8e-116">Name</span></span>       | <span data-ttu-id="4dd8e-117">説明</span><span class="sxs-lookup"><span data-stu-id="4dd8e-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="4dd8e-118">承認</span><span class="sxs-lookup"><span data-stu-id="4dd8e-118">Authorization</span></span>  | <span data-ttu-id="4dd8e-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="4dd8e-p102">Bearer {token}. Required.</span></span> | | <span data-ttu-id="4dd8e-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="4dd8e-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="4dd8e-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="4dd8e-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|
| <span data-ttu-id="4dd8e-124">workbook-session-id</span><span class="sxs-lookup"><span data-stu-id="4dd8e-124">workbook-session-id</span></span> | <span data-ttu-id="4dd8e-125">閉じるブック セッションの ID</span><span class="sxs-lookup"><span data-stu-id="4dd8e-125">Workbook session Id to be closed</span></span> |

## <a name="request-body"></a><span data-ttu-id="4dd8e-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="4dd8e-126">Request body</span></span>
<span data-ttu-id="4dd8e-127">この API は、要求本文を必要としません。</span><span class="sxs-lookup"><span data-stu-id="4dd8e-127">This API does not require any request body.</span></span>

## <a name="response"></a><span data-ttu-id="4dd8e-128">応答</span><span class="sxs-lookup"><span data-stu-id="4dd8e-128">Response</span></span>

<span data-ttu-id="4dd8e-129">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="4dd8e-129">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="4dd8e-130">例</span><span class="sxs-lookup"><span data-stu-id="4dd8e-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4dd8e-131">要求</span><span class="sxs-lookup"><span data-stu-id="4dd8e-131">Request</span></span>
<span data-ttu-id="4dd8e-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="4dd8e-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "close_excel_session"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/closeSession
Content-type: application/json
workbook-session-id: {session-id}
Content-length: 0

{

}
```

<span data-ttu-id="4dd8e-133">workbook-session-id ヘッダーが必要となることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="4dd8e-133">Note that workbook-session-id header is required.</span></span> 


##### <a name="response"></a><span data-ttu-id="4dd8e-134">応答</span><span class="sxs-lookup"><span data-stu-id="4dd8e-134">Response</span></span>
<span data-ttu-id="4dd8e-135">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="4dd8e-135">Here is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- {
  "type": "#page.annotation",
  "suppressions": [
    "Warning: close_excel_session//api-reference/v1.0/api/workbook_closesession.md:
      Request includes a non-standard header: workbook-session-id"
  ]
}-->