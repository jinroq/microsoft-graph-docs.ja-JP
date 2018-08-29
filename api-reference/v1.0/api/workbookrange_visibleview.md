# <a name="workbookrange-visibleview"></a><span data-ttu-id="5ed65-101">workbookRange: visibleView</span><span class="sxs-lookup"><span data-stu-id="5ed65-101">workbookRange: visibleView</span></span>


## <a name="permissions"></a><span data-ttu-id="5ed65-102">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="5ed65-102">Permissions</span></span>
<span data-ttu-id="5ed65-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5ed65-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="5ed65-105">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="5ed65-105">Permission type</span></span>      | <span data-ttu-id="5ed65-106">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="5ed65-106">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5ed65-107">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="5ed65-107">Delegated (work or school account)</span></span> | <span data-ttu-id="5ed65-108">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5ed65-108">Files.ReadWrite</span></span>    |
|<span data-ttu-id="5ed65-109">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="5ed65-109">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5ed65-110">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5ed65-110">Not supported.</span></span>    |
|<span data-ttu-id="5ed65-111">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5ed65-111">Application</span></span> | <span data-ttu-id="5ed65-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5ed65-112">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5ed65-113">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5ed65-113">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/root/workbook/worksheets/{id}/range(address={address})/visibleView
```
## <a name="request-headers"></a><span data-ttu-id="5ed65-114">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5ed65-114">Request headers</span></span>
| <span data-ttu-id="5ed65-115">名前</span><span class="sxs-lookup"><span data-stu-id="5ed65-115">Name</span></span>       | <span data-ttu-id="5ed65-116">説明</span><span class="sxs-lookup"><span data-stu-id="5ed65-116">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="5ed65-117">承認</span><span class="sxs-lookup"><span data-stu-id="5ed65-117">Authorization</span></span>  | <span data-ttu-id="5ed65-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="5ed65-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5ed65-120">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="5ed65-120">Workbook-Session-Id</span></span>  | <span data-ttu-id="5ed65-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="5ed65-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5ed65-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="5ed65-123">Request body</span></span>

### <a name="response"></a><span data-ttu-id="5ed65-124">応答</span><span class="sxs-lookup"><span data-stu-id="5ed65-124">Response</span></span>
<span data-ttu-id="5ed65-125">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [workbookRangeView](../resources/workbookrangeview.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="5ed65-125">If successful, this method returns `200 OK` response code and [workbookRangeView](../resources/workbookrangeview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5ed65-126">例</span><span class="sxs-lookup"><span data-stu-id="5ed65-126">Example</span></span>
<span data-ttu-id="5ed65-127">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="5ed65-127">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="5ed65-128">要求</span><span class="sxs-lookup"><span data-stu-id="5ed65-128">Request</span></span>
<span data-ttu-id="5ed65-129">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="5ed65-129">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "workbookrange_visibleview"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/root/workbook/worksheets/{id}/range(address='A1:Z10')/visibleView
```

##### <a name="response"></a><span data-ttu-id="5ed65-130">応答</span><span class="sxs-lookup"><span data-stu-id="5ed65-130">Response</span></span>
<span data-ttu-id="5ed65-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="5ed65-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRangeView"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 194

{
  "cellAddresses": "cellAddresses-value",
  "columnCount": 99,
  "formulas": "formulas-value",
  "formulasLocal": "formulasLocal-value",
  "formulasR1C1": "formulasR1C1-value",
  "index": 99
}
```