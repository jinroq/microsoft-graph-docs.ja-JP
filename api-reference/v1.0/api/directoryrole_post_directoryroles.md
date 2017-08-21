# <a name="activate-directoryrole"></a><span data-ttu-id="bb16b-101">directoryRole をアクティブにする</span><span class="sxs-lookup"><span data-stu-id="bb16b-101">Activate directoryRole</span></span>

<span data-ttu-id="bb16b-p101">ディレクトリ ロールをアクティブ化します。ディレクトリ ロールを読み取る場合や、そのメンバーを更新する場合は、まず、そのディレクトリ ロールをテナントでアクティブにする必要があります。既定では、会社の管理者 (Company Administrators) とユーザー (Users) のディレクトリ ロールのみがアクティブ化されています。アクセスしてメンバーを別のディレクトリ ロールに割り当てるには、まずそのディレクトリ ロールを対応するディレクトリ ロール テンプレート ([directoryRoleTemplate](../resources/directoryroletemplate.md)) でアクティブにする必要があります。</span><span class="sxs-lookup"><span data-stu-id="bb16b-p101">Activate a directory role. To read a directory role or update its members, it must first be activated in the tenant. Only the Company Administrators and the implicit Users directory roles are activated by default. To access and assign members to another directory role, you must first activate it with its corresponding directory role template ([directoryRoleTemplate](../resources/directoryroletemplate.md)).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bb16b-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="bb16b-106">Prerequisites</span></span>
<span data-ttu-id="bb16b-107">この API を実行するには、以下のいずれかの**スコープ**が必要です。*Directory.ReadWrite.All* または *Directory.AccessAsUser.All*</span><span class="sxs-lookup"><span data-stu-id="bb16b-107">One of the following **scopes** is required to execute this API: *Directory.ReadWrite.All* or *Directory.AccessAsUser.All*</span></span>
## <a name="http-request"></a><span data-ttu-id="bb16b-108">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="bb16b-108">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /directoryRoles

```
## <a name="request-headers"></a><span data-ttu-id="bb16b-109">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="bb16b-109">Request headers</span></span>
| <span data-ttu-id="bb16b-110">名前</span><span class="sxs-lookup"><span data-stu-id="bb16b-110">Name</span></span>       | <span data-ttu-id="bb16b-111">型</span><span class="sxs-lookup"><span data-stu-id="bb16b-111">Type</span></span> | <span data-ttu-id="bb16b-112">説明</span><span class="sxs-lookup"><span data-stu-id="bb16b-112">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="bb16b-113">Authorization</span><span class="sxs-lookup"><span data-stu-id="bb16b-113">Authorization</span></span>  | <span data-ttu-id="bb16b-114">string</span><span class="sxs-lookup"><span data-stu-id="bb16b-114">string</span></span>  | <span data-ttu-id="bb16b-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="bb16b-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="bb16b-117">Content-Type</span><span class="sxs-lookup"><span data-stu-id="bb16b-117">Content-Type</span></span>  | <span data-ttu-id="bb16b-118">application/json</span><span class="sxs-lookup"><span data-stu-id="bb16b-118">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="bb16b-119">要求本文</span><span class="sxs-lookup"><span data-stu-id="bb16b-119">Request body</span></span>
<span data-ttu-id="bb16b-120">要求本文で、[directoryRole](../resources/directoryrole.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="bb16b-120">In the request body, supply a JSON representation of [directoryRole](../resources/directoryrole.md) object.</span></span>

<span data-ttu-id="bb16b-121">次の表に、ディレクトリ ロールをアクティブにする際に必要になるプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="bb16b-121">The following table shows the properties that are required when you activate a directory role.</span></span>

|<span data-ttu-id="bb16b-122">必須のパラメーター</span><span class="sxs-lookup"><span data-stu-id="bb16b-122">Required parameter</span></span> | <span data-ttu-id="bb16b-123">種類</span><span class="sxs-lookup"><span data-stu-id="bb16b-123">Type</span></span> | <span data-ttu-id="bb16b-124">説明</span><span class="sxs-lookup"><span data-stu-id="bb16b-124">Description</span></span>|
|:---------|:---------|:---------|
|<span data-ttu-id="bb16b-125">roleTemplateId</span><span class="sxs-lookup"><span data-stu-id="bb16b-125">roleTemplateId</span></span> | <span data-ttu-id="bb16b-126">string</span><span class="sxs-lookup"><span data-stu-id="bb16b-126">string</span></span> | <span data-ttu-id="bb16b-p103">このロールが基づいている [directoryRoleTemplate](../resources/directoryroletemplate.md) の ID。これは要求で指定できる唯一のプロパティです。</span><span class="sxs-lookup"><span data-stu-id="bb16b-p103">The ID of the [directoryRoleTemplate](../resources/directoryroletemplate.md) that the role is based on. This is the only property that may be specified in the request.</span></span>|

## <a name="response"></a><span data-ttu-id="bb16b-129">応答</span><span class="sxs-lookup"><span data-stu-id="bb16b-129">Response</span></span>

<span data-ttu-id="bb16b-130">成功した場合、このメソッドは `201, Created` 応答コードと、応答本文で [directoryRole](../resources/directoryrole.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="bb16b-130">If successful, this method returns `201, Created` response code and [directoryRole](../resources/directoryrole.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bb16b-131">例</span><span class="sxs-lookup"><span data-stu-id="bb16b-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bb16b-132">要求</span><span class="sxs-lookup"><span data-stu-id="bb16b-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create_directoryrole_from_directoryroles"
}-->
```http
POST https://graph.microsoft.com/v1.0/directoryRoles
Content-type: application/json

{
  "roleTemplateId": "roleTemplateId-value"
}
```
<span data-ttu-id="bb16b-133">要求本文で、[directoryRole](../resources/directoryrole.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="bb16b-133">In the request body, supply a JSON representation of [directoryRole](../resources/directoryrole.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="bb16b-134">応答</span><span class="sxs-lookup"><span data-stu-id="bb16b-134">Response</span></span>
<span data-ttu-id="bb16b-p104">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="bb16b-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryRole"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "description": "description-value",
  "displayName": "displayName-value",
  "roleTemplateId": "roleTemplateId-value",
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create directoryRole",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
