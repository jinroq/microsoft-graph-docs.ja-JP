# <a name="worksheetprotection-protect"></a><span data-ttu-id="2551b-101">WorksheetProtection: protect</span><span class="sxs-lookup"><span data-stu-id="2551b-101">WorksheetProtection: protect</span></span>

<span data-ttu-id="2551b-p101">ワークシートを保護します。ワークシートが保護されている場合はスローします。</span><span class="sxs-lookup"><span data-stu-id="2551b-p101">Protect a worksheet. It throws if the worksheet has been protected.</span></span>
## <a name="permissions"></a><span data-ttu-id="2551b-104">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="2551b-104">Permissions</span></span>
<span data-ttu-id="2551b-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2551b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="2551b-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2551b-107">Permission type</span></span>      | <span data-ttu-id="2551b-108">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="2551b-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2551b-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2551b-109">Delegated (work or school account)</span></span> | <span data-ttu-id="2551b-110">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2551b-110">Files.ReadWrite</span></span>    |
|<span data-ttu-id="2551b-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2551b-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2551b-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2551b-112">Not supported.</span></span>    |
|<span data-ttu-id="2551b-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2551b-113">Application</span></span> | <span data-ttu-id="2551b-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2551b-114">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2551b-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2551b-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/protection/protect

```
## <a name="request-headers"></a><span data-ttu-id="2551b-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2551b-116">Request headers</span></span>
| <span data-ttu-id="2551b-117">名前</span><span class="sxs-lookup"><span data-stu-id="2551b-117">Name</span></span>       | <span data-ttu-id="2551b-118">説明</span><span class="sxs-lookup"><span data-stu-id="2551b-118">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="2551b-119">承認</span><span class="sxs-lookup"><span data-stu-id="2551b-119">Authorization</span></span>  | <span data-ttu-id="2551b-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="2551b-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2551b-122">ブックセッション Id</span><span class="sxs-lookup"><span data-stu-id="2551b-122">Workbook-Session-Id</span></span>  | <span data-ttu-id="2551b-p104">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="2551b-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2551b-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="2551b-125">Request body</span></span>
<span data-ttu-id="2551b-126">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="2551b-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="2551b-127">パラメーター</span><span class="sxs-lookup"><span data-stu-id="2551b-127">Parameter</span></span>    | <span data-ttu-id="2551b-128">型</span><span class="sxs-lookup"><span data-stu-id="2551b-128">Type</span></span>   |<span data-ttu-id="2551b-129">説明</span><span class="sxs-lookup"><span data-stu-id="2551b-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2551b-130">options</span><span class="sxs-lookup"><span data-stu-id="2551b-130">options</span></span>|<span data-ttu-id="2551b-131">WorkbookWorksheetProtectionOptions</span><span class="sxs-lookup"><span data-stu-id="2551b-131">WorkbookWorksheetProtectionOptions</span></span>|<span data-ttu-id="2551b-p105">省略可能。シートの保護のオプション。</span><span class="sxs-lookup"><span data-stu-id="2551b-p105">Optional. sheet protection options.</span></span>|

## <a name="response"></a><span data-ttu-id="2551b-134">応答</span><span class="sxs-lookup"><span data-stu-id="2551b-134">Response</span></span>

<span data-ttu-id="2551b-p106">成功した場合、このメソッドは `200 OK` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="2551b-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2551b-137">例</span><span class="sxs-lookup"><span data-stu-id="2551b-137">Example</span></span>
<span data-ttu-id="2551b-138">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="2551b-138">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="2551b-139">要求</span><span class="sxs-lookup"><span data-stu-id="2551b-139">Request</span></span>
<span data-ttu-id="2551b-140">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="2551b-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "worksheetprotection_protect"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/protection/protect
Content-type: application/json
Content-length: 383

{
  "options": {
    "allowFormatCells": true,
    "allowFormatColumns": true,
    "allowFormatRows": true,
    "allowInsertColumns": true,
    "allowInsertRows": true,
    "allowInsertHyperlinks": true,
    "allowDeleteColumns": true,
    "allowDeleteRows": true,
    "allowSort": true,
    "allowAutoFilter": true,
    "allowPivotTables": true
  }
}
```

##### <a name="response"></a><span data-ttu-id="2551b-141">応答</span><span class="sxs-lookup"><span data-stu-id="2551b-141">Response</span></span>
<span data-ttu-id="2551b-142">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="2551b-142">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "WorksheetProtection: protect",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
