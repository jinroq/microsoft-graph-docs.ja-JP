# <a name="get-group"></a><span data-ttu-id="ce561-101">グループを取得する</span><span class="sxs-lookup"><span data-stu-id="ce561-101">Get group</span></span>

<span data-ttu-id="ce561-102">この **educationClass** に対応する Office 365 **グループ**を取得します。</span><span class="sxs-lookup"><span data-stu-id="ce561-102">Retrieve the Office 365 **group** that corresponds to this **educationClass**.</span></span>

><span data-ttu-id="ce561-103">**注:** 委任されたトークンを使用した場合、メンバーは自分の学校に関する情報以外を参照できません。</span><span class="sxs-lookup"><span data-stu-id="ce561-103">**Note:** If the delegated token is used, members can only see information about their own schools.</span></span> <span data-ttu-id="ce561-104">この場合は `...beta/education/me/schools` リソースを使用してください。</span><span class="sxs-lookup"><span data-stu-id="ce561-104">Use the `...beta/education/me/schools` resource in this case.</span></span>

## <a name="permissions"></a><span data-ttu-id="ce561-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ce561-105">Permissions</span></span>
<span data-ttu-id="ce561-106">この API を呼び出すには、アクセス許可の組み合わせが必要です。</span><span class="sxs-lookup"><span data-stu-id="ce561-106">A combination of permissions is required to call this API.</span></span> <span data-ttu-id="ce561-107">アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ce561-107">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ce561-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ce561-108">Permission type</span></span>      | <span data-ttu-id="ce561-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="ce561-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ce561-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ce561-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="ce561-111">One from EduRoster.ReadBasic、EduRoster.Read、EduRoster.Write plus Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="ce561-111">One from EduRoster.ReadBasic, EduRoster.Read, EduRoster.Write plus Directory.Read.All</span></span>|
|<span data-ttu-id="ce561-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ce561-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="ce561-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ce561-113">Not supported.</span></span>  |
|<span data-ttu-id="ce561-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ce561-114">Application</span></span> | <span data-ttu-id="ce561-115">EduRoster.Read.All、EduRoster.ReadWrite.All plus Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="ce561-115">EduRoster.Read.All, EduRoster.ReadWrite.All plus Directory.Read.All</span></span>| 

## <a name="http-request"></a><span data-ttu-id="ce561-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ce561-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/group
```
## <a name="request-headers"></a><span data-ttu-id="ce561-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ce561-117">Request headers</span></span>
| <span data-ttu-id="ce561-118">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ce561-118">Header</span></span>       | <span data-ttu-id="ce561-119">値</span><span class="sxs-lookup"><span data-stu-id="ce561-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ce561-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="ce561-120">Authorization</span></span>  | <span data-ttu-id="ce561-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="ce561-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ce561-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="ce561-123">Request body</span></span>
<span data-ttu-id="ce561-124">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="ce561-124">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="ce561-125">応答</span><span class="sxs-lookup"><span data-stu-id="ce561-125">Response</span></span>
<span data-ttu-id="ce561-126">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [group](../resources/group.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="ce561-126">If successful, this method returns a `200 OK` response code and [group](../resources/group.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ce561-127">例</span><span class="sxs-lookup"><span data-stu-id="ce561-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ce561-128">要求</span><span class="sxs-lookup"><span data-stu-id="ce561-128">Request</span></span>
<span data-ttu-id="ce561-129">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="ce561-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_group"
}-->
```http
GET https://graph.microsoft.com/v1.0/education/classes/2961761D-8094-4183-A9F6-8E36E966C7D9/group
```
##### <a name="response"></a><span data-ttu-id="ce561-130">応答</span><span class="sxs-lookup"><span data-stu-id="ce561-130">Response</span></span>
<span data-ttu-id="ce561-131">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="ce561-131">The following is an example of the response.</span></span> 

><span data-ttu-id="ce561-p104">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="ce561-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": false
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: xxx

{
  "id": "id-value",
  "description": "description-value",
  "displayName": "displayName-value",
  "groupTypes": [
    "groupTypes-value"
  ],
  "mail": "mail-value",
  "mailEnabled": true,
  "mailNickname": "mailNickname-value",
  "onPremisesLastSyncDateTime": "onPremisesLastSyncDateTime-value",
  "onPremisesSecurityIdentifier": "onPremisesSecurityIdentifier-value",
  "onPremisesSyncEnabled": true,
  "proxyAddresses": [
    "proxyAddresses-value"
   ],
   "securityEnabled": true,
   "visibility": "visibility-value"
}
```

<!-- uuid: 0087D9B3-1418-4C87-91C9-A18C6D93706B
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get user",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->