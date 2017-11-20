# <a name="update-a-group-setting"></a><span data-ttu-id="b8c1e-101">グループ設定を更新する</span><span class="sxs-lookup"><span data-stu-id="b8c1e-101">Update a group setting</span></span>

<span data-ttu-id="b8c1e-102">特定のグループ設定オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="b8c1e-102">Update the properties of a specific group setting object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b8c1e-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="b8c1e-103">Permissions</span></span>

<span data-ttu-id="b8c1e-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b8c1e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="b8c1e-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b8c1e-106">Permission type</span></span>      | <span data-ttu-id="b8c1e-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="b8c1e-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b8c1e-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b8c1e-108">Delegated (work or school account)</span></span> | <span data-ttu-id="b8c1e-109">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b8c1e-109">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="b8c1e-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b8c1e-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b8c1e-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b8c1e-111">Not supported.</span></span>    |
|<span data-ttu-id="b8c1e-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b8c1e-112">Application</span></span> | <span data-ttu-id="b8c1e-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b8c1e-113">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b8c1e-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b8c1e-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

<span data-ttu-id="b8c1e-115">テナント全体またはグループ固有の設定を更新します。</span><span class="sxs-lookup"><span data-stu-id="b8c1e-115">Update a tenant-wide or group specific setting.</span></span>

```http
PATCH /groupSettings/{id}
PATCH /groups/{id}/settings/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="b8c1e-116">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b8c1e-116">Optional request headers</span></span>
| <span data-ttu-id="b8c1e-117">名前</span><span class="sxs-lookup"><span data-stu-id="b8c1e-117">Name</span></span> | <span data-ttu-id="b8c1e-118">説明</span><span class="sxs-lookup"><span data-stu-id="b8c1e-118">Description</span></span> |
|:-----------|:-----------|
| <span data-ttu-id="b8c1e-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="b8c1e-119">Authorization</span></span>  | <span data-ttu-id="b8c1e-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="b8c1e-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b8c1e-122">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b8c1e-122">Content-Type</span></span>  | <span data-ttu-id="b8c1e-123">application/json</span><span class="sxs-lookup"><span data-stu-id="b8c1e-123">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b8c1e-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="b8c1e-124">Request body</span></span>
<span data-ttu-id="b8c1e-125">要求本文で、更新する関連フィールドの値を指定します。</span><span class="sxs-lookup"><span data-stu-id="b8c1e-125">In the request body, supply the values for relevant fields that should be updated.</span></span> 

| <span data-ttu-id="b8c1e-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b8c1e-126">Property</span></span> | <span data-ttu-id="b8c1e-127">型</span><span class="sxs-lookup"><span data-stu-id="b8c1e-127">Type</span></span> | <span data-ttu-id="b8c1e-128">説明</span><span class="sxs-lookup"><span data-stu-id="b8c1e-128">Description</span></span> |
|:---------------|:--------|:----------|
| <span data-ttu-id="b8c1e-129">values</span><span class="sxs-lookup"><span data-stu-id="b8c1e-129">values</span></span> | <span data-ttu-id="b8c1e-130">settingValue</span><span class="sxs-lookup"><span data-stu-id="b8c1e-130">settingValue</span></span> | <span data-ttu-id="b8c1e-p103">更新された値のセットです。注:コレクション セット全体を指定する必要があります。単一の値のセットを更新することはできません。</span><span class="sxs-lookup"><span data-stu-id="b8c1e-p103">The updated set of values.  NOTE: You must supply the entire collection set. You cannot update a single set of values.</span></span> |

## <a name="response"></a><span data-ttu-id="b8c1e-134">応答</span><span class="sxs-lookup"><span data-stu-id="b8c1e-134">Response</span></span>

<span data-ttu-id="b8c1e-135">成功した場合、このメソッドは `204 OK` 応答コードと、応答本文で、更新された [groupSetting](../resources/groupsetting.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="b8c1e-135">If successful, this method returns a `204 OK` response code and updated [groupSetting](../resources/groupsetting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b8c1e-136">例</span><span class="sxs-lookup"><span data-stu-id="b8c1e-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b8c1e-137">要求</span><span class="sxs-lookup"><span data-stu-id="b8c1e-137">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "update_groupsetting"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/groupSettings/{id}
Content-type: application/json
Content-length: 173

{
  "displayName": "displayName-value",
  "templateId": "templateId-value",
  "values": [
    {
      "name": "CustomBlockedWordsList",
      "value": ""
    },
    {
      "name": "EnableMSStandardBlockedWords",
      "value": "False"
    },
    {
      "name": "ClassificationDescriptions",
      "value": ""
    },
    {
      "name": "DefaultClassification",
      "value": ""
    },
    {
      "name": "PrefixSuffixNamingRequirement",
      "value": ""
    },
    {
      "name": "AllowGuestsToBeGroupOwner",
      "value": "False"
    },
    {
      "name": "AllowGuestsToAccessGroups",
      "value": "True"
    },
    {
      "name": "GuestUsageGuidelinesUrl",
      "value": ""
    },
    {
      "name": "GroupCreationAllowedGroupId",
      "value": "62e90394-69f5-4237-9190-012177145e10"
    },
    {
      "name": "AllowToAddGuests",
      "value": "True"
    },
    {
      "name": "UsageGuidelinesUrl",
      "value": ""
    },
    {
      "name": "ClassificationList",
      "value": ""
    },
    {
      "name": "EnableGroupCreation",
      "value": "True"
    }
  ]
}
```
##### <a name="response"></a><span data-ttu-id="b8c1e-138">応答</span><span class="sxs-lookup"><span data-stu-id="b8c1e-138">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupSetting"
} -->
```http
HTTP/1.1 204 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update groupSetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
