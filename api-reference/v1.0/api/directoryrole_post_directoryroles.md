# <a name="activate-directoryrole"></a><span data-ttu-id="323d9-101">directoryRole をアクティブにする</span><span class="sxs-lookup"><span data-stu-id="323d9-101">Activate directoryRole</span></span>

<span data-ttu-id="323d9-p101">ディレクトリ ロールをアクティブ化します。ディレクトリ ロールを読み取る場合や、そのメンバーを更新する場合は、まず、そのディレクトリ ロールをテナントでアクティブにする必要があります。既定では、会社の管理者 (Company Administrators) とユーザー (Users) のディレクトリ ロールのみがアクティブ化されています。アクセスしてメンバーを別のディレクトリ ロールに割り当てるには、まずそのディレクトリ ロールを対応するディレクトリ ロール テンプレート ([directoryRoleTemplate](../resources/directoryroletemplate.md)) でアクティブにする必要があります。</span><span class="sxs-lookup"><span data-stu-id="323d9-p101">Activate a directory role. To read a directory role or update its members, it must first be activated in the tenant. Only the Company Administrators and the implicit Users directory roles are activated by default. To access and assign members to another directory role, you must first activate it with its corresponding directory role template ([directoryRoleTemplate](../resources/directoryroletemplate.md)).</span></span>

## <a name="permissions"></a><span data-ttu-id="323d9-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="323d9-106">Permissions</span></span>
<span data-ttu-id="323d9-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="323d9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="323d9-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="323d9-109">Permission type</span></span>      | <span data-ttu-id="323d9-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="323d9-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="323d9-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="323d9-111">Delegated (work or school account)</span></span> | <span data-ttu-id="323d9-112">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="323d9-112">Directory.ReadWrite.All or Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="323d9-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="323d9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="323d9-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="323d9-114">Not supported.</span></span>    |
|<span data-ttu-id="323d9-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="323d9-115">Application</span></span> | <span data-ttu-id="323d9-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="323d9-116">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="323d9-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="323d9-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /directoryRoles

```
## <a name="request-headers"></a><span data-ttu-id="323d9-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="323d9-118">Request headers</span></span>
| <span data-ttu-id="323d9-119">名前</span><span class="sxs-lookup"><span data-stu-id="323d9-119">Name</span></span>       | <span data-ttu-id="323d9-120">型</span><span class="sxs-lookup"><span data-stu-id="323d9-120">Type</span></span> | <span data-ttu-id="323d9-121">説明</span><span class="sxs-lookup"><span data-stu-id="323d9-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="323d9-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="323d9-122">Authorization</span></span>  | <span data-ttu-id="323d9-123">string</span><span class="sxs-lookup"><span data-stu-id="323d9-123">string</span></span>  | <span data-ttu-id="323d9-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="323d9-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="323d9-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="323d9-126">Content-Type</span></span>  | <span data-ttu-id="323d9-127">application/json</span><span class="sxs-lookup"><span data-stu-id="323d9-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="323d9-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="323d9-128">Request body</span></span>
<span data-ttu-id="323d9-129">要求本文で、[directoryRole](../resources/directoryrole.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="323d9-129">In the request body, supply a JSON representation of [directoryRole](../resources/directoryrole.md) object.</span></span>

<span data-ttu-id="323d9-130">次の表に、ディレクトリ ロールをアクティブにする際に必要になるプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="323d9-130">The following table shows the properties that are required when you activate a directory role.</span></span>

|<span data-ttu-id="323d9-131">必須のパラメーター</span><span class="sxs-lookup"><span data-stu-id="323d9-131">Required parameter</span></span> | <span data-ttu-id="323d9-132">種類</span><span class="sxs-lookup"><span data-stu-id="323d9-132">Type</span></span> | <span data-ttu-id="323d9-133">説明</span><span class="sxs-lookup"><span data-stu-id="323d9-133">Description</span></span>|
|:---------|:---------|:---------|
|<span data-ttu-id="323d9-134">roleTemplateId</span><span class="sxs-lookup"><span data-stu-id="323d9-134">roleTemplateId</span></span> | <span data-ttu-id="323d9-135">string</span><span class="sxs-lookup"><span data-stu-id="323d9-135">string</span></span> | <span data-ttu-id="323d9-p104">このロールが基づいている [directoryRoleTemplate](../resources/directoryroletemplate.md) の ID。これは要求で指定できる唯一のプロパティです。</span><span class="sxs-lookup"><span data-stu-id="323d9-p104">The ID of the [directoryRoleTemplate](../resources/directoryroletemplate.md) that the role is based on. This is the only property that may be specified in the request.</span></span>|

## <a name="response"></a><span data-ttu-id="323d9-138">応答</span><span class="sxs-lookup"><span data-stu-id="323d9-138">Response</span></span>

<span data-ttu-id="323d9-139">成功した場合、このメソッドは `201, Created` 応答コードと、応答本文で [directoryRole](../resources/directoryrole.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="323d9-139">If successful, this method returns `201, Created` response code and [directoryRole](../resources/directoryrole.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="323d9-140">例</span><span class="sxs-lookup"><span data-stu-id="323d9-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="323d9-141">要求</span><span class="sxs-lookup"><span data-stu-id="323d9-141">Request</span></span>

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
<span data-ttu-id="323d9-142">要求本文で、[directoryRole](../resources/directoryrole.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="323d9-142">In the request body, supply a JSON representation of [directoryRole](../resources/directoryrole.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="323d9-143">応答</span><span class="sxs-lookup"><span data-stu-id="323d9-143">Response</span></span>
<span data-ttu-id="323d9-p105">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="323d9-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
