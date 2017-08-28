# <a name="create-a-group-setting"></a><span data-ttu-id="88754-101">グループ設定を作成する</span><span class="sxs-lookup"><span data-stu-id="88754-101">Create a group setting</span></span>

<span data-ttu-id="88754-p101">この API を使用して、[groupSettingTemplates](../resources/groupsettingtemplate.md) で使用可能なテンプレートに基づいて新しい設定を作成します。これらの設定は、テナント レベルまたはグループ レベルで行うことができます。作成要求は、テンプレートに定義されているすべての設定の [settingValues](../resources/settingvalue.md) を提供する必要があります。グループ固有の設定では、グループのメンバーがゲスト ユーザーを招待できるかどうかの管理のみが設定できます。グループにゲスト ユーザーを追加する機能が一般的に利用可能になると、上記の動作は制御されます。</span><span class="sxs-lookup"><span data-stu-id="88754-p101">Use this API to create a new setting, based on the templates available in [groupSettingTemplates](../resources/groupsettingtemplate.md). These settings can be at the tenant-level or at the group level. The creation request must provide [settingValues](../resources/settingvalue.md) for all the settings defined in the template. For group-specific settings, only the setting governing whether members of a group can invite guest users can be set. This will govern this behavior once the ability to add guest users to a group is generally available.</span></span>

## <a name="permissions"></a><span data-ttu-id="88754-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="88754-107">Permissions</span></span>

<span data-ttu-id="88754-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="88754-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="88754-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="88754-110">Permission type</span></span>      | <span data-ttu-id="88754-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="88754-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="88754-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="88754-112">Delegated (work or school account)</span></span> | <span data-ttu-id="88754-113">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="88754-113">Directory.ReadWrite.All or Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="88754-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="88754-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="88754-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="88754-115">Not supported.</span></span>    |
|<span data-ttu-id="88754-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="88754-116">Application</span></span> | <span data-ttu-id="88754-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88754-117">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="88754-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="88754-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groupSettings
POST /groups/{id}/settings
```

## <a name="request-headers"></a><span data-ttu-id="88754-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="88754-119">Request headers</span></span>

| <span data-ttu-id="88754-120">名前</span><span class="sxs-lookup"><span data-stu-id="88754-120">Name</span></span> | <span data-ttu-id="88754-121">説明</span><span class="sxs-lookup"><span data-stu-id="88754-121">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="88754-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="88754-122">Authorization</span></span> | <span data-ttu-id="88754-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="88754-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="88754-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="88754-125">Content-Type</span></span> | <span data-ttu-id="88754-126">application/json</span><span class="sxs-lookup"><span data-stu-id="88754-126">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="88754-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="88754-127">Request body</span></span>
<span data-ttu-id="88754-p104">要求本文で、[groupSetting](../resources/groupsetting.md) オブジェクトの JSON 表記を指定します。ただし、設定の表示名は、参照される設定テンプレート名に基づいて設定されます。</span><span class="sxs-lookup"><span data-stu-id="88754-p104">In the request body, supply a JSON representation of [groupSetting](../resources/groupsetting.md) object. However, the display name for the setting will be set based on the referenced settings template name.</span></span>

## <a name="response"></a><span data-ttu-id="88754-130">応答</span><span class="sxs-lookup"><span data-stu-id="88754-130">Response</span></span>

<span data-ttu-id="88754-131">成功した場合、このメソッドは `201, Created` 応答コードと、応答本文で [groupSetting](../resources/groupsetting.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="88754-131">If successful, this method returns `201, Created` response code and [groupSetting](../resources/groupsetting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="88754-132">例</span><span class="sxs-lookup"><span data-stu-id="88754-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="88754-133">要求</span><span class="sxs-lookup"><span data-stu-id="88754-133">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create_groupsetting_from_groupsettings"
}-->
```http
POST https://graph.microsoft.com/v1.0/groupSettings
Content-type: application/json
Content-length: 215

{
  "groupSetting": {
    "displayName": "displayName-value",
    "templateId": "templateId-value",
    "values": [
      {
        "name": "name-value",
        "value": "value-value"
      }
    ]
  }
}
```
<span data-ttu-id="88754-134">要求本文で、[groupSetting](../resources/groupsetting.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="88754-134">In the request body, supply a JSON representation of [groupSetting](../resources/groupsetting.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="88754-135">応答</span><span class="sxs-lookup"><span data-stu-id="88754-135">Response</span></span>

<span data-ttu-id="88754-p105">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="88754-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupSetting"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 238

{
  "groupSetting": {
    "displayName": "displayName-value",
    "templateId": "templateId-value",
    "values": [
      {
        "name": "name-value",
        "value": "value-value"
      }
    ],
    "id": "id-value"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create groupsetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->