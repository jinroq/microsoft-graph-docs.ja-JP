# <a name="worksheetprotection-unprotect"></a><span data-ttu-id="03848-101">WorksheetProtection: unprotect</span><span class="sxs-lookup"><span data-stu-id="03848-101">WorksheetProtection: unprotect</span></span>

<span data-ttu-id="03848-102">ワークシートの保護を解除します。</span><span class="sxs-lookup"><span data-stu-id="03848-102">Unprotect a worksheet</span></span>
## <a name="permissions"></a><span data-ttu-id="03848-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="03848-103">Permissions</span></span>
<span data-ttu-id="03848-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="03848-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="03848-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="03848-106">Permission type</span></span>      | <span data-ttu-id="03848-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="03848-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="03848-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="03848-108">Delegated (work or school account)</span></span> | <span data-ttu-id="03848-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="03848-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="03848-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="03848-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="03848-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="03848-111">Not supported.</span></span>    |
|<span data-ttu-id="03848-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="03848-112">Application</span></span> | <span data-ttu-id="03848-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="03848-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="03848-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="03848-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/protection/unprotect

```
## <a name="request-headers"></a><span data-ttu-id="03848-115">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="03848-115">Request headers</span></span>
| <span data-ttu-id="03848-116">名前</span><span class="sxs-lookup"><span data-stu-id="03848-116">Name</span></span>       | <span data-ttu-id="03848-117">説明</span><span class="sxs-lookup"><span data-stu-id="03848-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="03848-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="03848-118">Authorization</span></span>  | <span data-ttu-id="03848-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="03848-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="03848-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="03848-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="03848-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="03848-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="03848-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="03848-124">Request body</span></span>
<span data-ttu-id="03848-125">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="03848-125">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="03848-126">パラメーター</span><span class="sxs-lookup"><span data-stu-id="03848-126">Parameter</span></span>    | <span data-ttu-id="03848-127">型</span><span class="sxs-lookup"><span data-stu-id="03848-127">Type</span></span>   |<span data-ttu-id="03848-128">説明</span><span class="sxs-lookup"><span data-stu-id="03848-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="03848-129">password</span><span class="sxs-lookup"><span data-stu-id="03848-129">password</span></span>|<span data-ttu-id="03848-130">string</span><span class="sxs-lookup"><span data-stu-id="03848-130">string</span></span>|<span data-ttu-id="03848-p104">省略可能。シートの保護パスワード。</span><span class="sxs-lookup"><span data-stu-id="03848-p104">Optional. sheet protection password.</span></span>|

## <a name="response"></a><span data-ttu-id="03848-133">応答</span><span class="sxs-lookup"><span data-stu-id="03848-133">Response</span></span>

<span data-ttu-id="03848-p105">成功した場合、このメソッドは `200 OK` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="03848-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="03848-136">例</span><span class="sxs-lookup"><span data-stu-id="03848-136">Example</span></span>
<span data-ttu-id="03848-137">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="03848-137">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="03848-138">要求</span><span class="sxs-lookup"><span data-stu-id="03848-138">Request</span></span>
<span data-ttu-id="03848-139">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="03848-139">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "worksheetprotection_unprotect"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/protection/unprotect
Content-type: application/json
Content-length: 34

{
  "password": "password-value"
}
```

##### <a name="response"></a><span data-ttu-id="03848-140">応答</span><span class="sxs-lookup"><span data-stu-id="03848-140">Response</span></span>
<span data-ttu-id="03848-141">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="03848-141">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "WorksheetProtection: unprotect",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->