# <a name="activate-directoryrole"></a><span data-ttu-id="f984d-101">directoryRole をアクティブにする</span><span class="sxs-lookup"><span data-stu-id="f984d-101">Activate directoryRole</span></span>

<span data-ttu-id="f984d-p101">ディレクトリ ロールをアクティブ化します。ディレクトリ ロールを読み取る場合や、そのメンバーを更新する場合は、まず、そのディレクトリ ロールをテナントでアクティブにする必要があります。既定では、会社の管理者 (Company Administrators) とユーザー (Users) のディレクトリ ロールのみがアクティブ化されています。アクセスしてメンバーを別のディレクトリ ロールに割り当てるには、まずそのディレクトリ ロールを対応するディレクトリ ロール テンプレート ([directoryRoleTemplate](../resources/directoryroletemplate.md)) でアクティブにする必要があります。</span><span class="sxs-lookup"><span data-stu-id="f984d-p101">Activate a directory role. To read a directory role or update its members, it must first be activated in the tenant. Only the Company Administrators and the implicit Users directory roles are activated by default. To access and assign members to another directory role, you must first activate it with its corresponding directory role template ([directoryRoleTemplate](../resources/directoryroletemplate.md)).</span></span>

## <a name="permissions"></a><span data-ttu-id="f984d-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f984d-106">Permissions</span></span>
<span data-ttu-id="f984d-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f984d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="f984d-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f984d-109">Permission type</span></span>      | <span data-ttu-id="f984d-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="f984d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f984d-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f984d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f984d-112">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f984d-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="f984d-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f984d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f984d-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f984d-114">Not supported.</span></span>    |
|<span data-ttu-id="f984d-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f984d-115">Application</span></span> | <span data-ttu-id="f984d-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f984d-116">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f984d-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f984d-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /directoryRoles

```
## <a name="request-headers"></a><span data-ttu-id="f984d-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f984d-118">Request headers</span></span>
| <span data-ttu-id="f984d-119">名前</span><span class="sxs-lookup"><span data-stu-id="f984d-119">Name</span></span>       | <span data-ttu-id="f984d-120">型</span><span class="sxs-lookup"><span data-stu-id="f984d-120">Type</span></span> | <span data-ttu-id="f984d-121">説明</span><span class="sxs-lookup"><span data-stu-id="f984d-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="f984d-122">承認</span><span class="sxs-lookup"><span data-stu-id="f984d-122">Authorization</span></span>  | <span data-ttu-id="f984d-123">string</span><span class="sxs-lookup"><span data-stu-id="f984d-123">string</span></span>  | <span data-ttu-id="f984d-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="f984d-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f984d-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f984d-126">Content-Type</span></span>  | <span data-ttu-id="f984d-127">string</span><span class="sxs-lookup"><span data-stu-id="f984d-127">string</span></span>  | <span data-ttu-id="f984d-128">application/json</span><span class="sxs-lookup"><span data-stu-id="f984d-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f984d-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="f984d-129">Request body</span></span>
<span data-ttu-id="f984d-130">要求本文で、[directoryRole](../resources/directoryrole.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="f984d-130">In the request body, supply a JSON representation of [directoryRole](../resources/directoryrole.md) object.</span></span>

<span data-ttu-id="f984d-131">次の表に、ディレクトリ ロールをアクティブ化するときに必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="f984d-131">The following table shows the properties that are required when you activate a directory role.</span></span>

|<span data-ttu-id="f984d-132">パラメーター</span><span class="sxs-lookup"><span data-stu-id="f984d-132">Parameter</span></span> | <span data-ttu-id="f984d-133">型</span><span class="sxs-lookup"><span data-stu-id="f984d-133">Type</span></span> | <span data-ttu-id="f984d-134">説明</span><span class="sxs-lookup"><span data-stu-id="f984d-134">Description</span></span>|
|:---------|:---------|:---------|
|<span data-ttu-id="f984d-135">roleTemplateId</span><span class="sxs-lookup"><span data-stu-id="f984d-135">roleTemplateId</span></span> | <span data-ttu-id="f984d-136">string</span><span class="sxs-lookup"><span data-stu-id="f984d-136">string</span></span> | <span data-ttu-id="f984d-137">必須。</span><span class="sxs-lookup"><span data-stu-id="f984d-137">Required.</span></span> <span data-ttu-id="f984d-138">ロールの基になっている [directoryRoleTemplate](../resources/directoryroletemplate.md) の ID です。</span><span class="sxs-lookup"><span data-stu-id="f984d-138">The ID of the [directoryRoleTemplate](../resources/directoryroletemplate.md) that the role is based on. This is the only property that may be specified in the request.</span></span> <span data-ttu-id="f984d-139">これは、要求内で指定できる唯一のプロパティです。</span><span class="sxs-lookup"><span data-stu-id="f984d-139">The ID of the directoryRoleTemplate that the role is based on. This is the only property that may be specified in the request.</span></span>|

## <a name="response"></a><span data-ttu-id="f984d-140">応答</span><span class="sxs-lookup"><span data-stu-id="f984d-140">Response</span></span>

<span data-ttu-id="f984d-141">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [directoryRole](../resources/directoryrole.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="f984d-141">If successful, this method returns `201 Created` response code and [directoryRole](../resources/directoryrole.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f984d-142">例</span><span class="sxs-lookup"><span data-stu-id="f984d-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f984d-143">要求</span><span class="sxs-lookup"><span data-stu-id="f984d-143">Request</span></span>

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
<span data-ttu-id="f984d-144">要求本文で、[directoryRole](../resources/directoryrole.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="f984d-144">In the request body, supply a JSON representation of [directoryRole](../resources/directoryrole.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="f984d-145">応答</span><span class="sxs-lookup"><span data-stu-id="f984d-145">Response</span></span>
<span data-ttu-id="f984d-p105">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f984d-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
