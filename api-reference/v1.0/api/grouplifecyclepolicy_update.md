# <a name="update-grouplifecyclepolicy"></a><span data-ttu-id="a6c1f-101">Update groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="a6c1f-101">Update groupLifecyclePolicy</span></span>

<span data-ttu-id="a6c1f-102">groupLifecyclePolicy[groupLifecyclePolicy リソース タイプ](../resources/grouplifecyclepolicy.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="a6c1f-102">Update the properties of a groupLifecyclePolicy[groupLifecyclePolicy resource type](../resources/grouplifecyclepolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a6c1f-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="a6c1f-103">Permissions</span></span>

<span data-ttu-id="a6c1f-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a6c1f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>
 
|<span data-ttu-id="a6c1f-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a6c1f-106">Permission type</span></span>      | <span data-ttu-id="a6c1f-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="a6c1f-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a6c1f-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a6c1f-108">Delegated (work or school account)</span></span> | <span data-ttu-id="a6c1f-109">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a6c1f-109">Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="a6c1f-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a6c1f-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a6c1f-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a6c1f-111">Not supported.</span></span>    |
|<span data-ttu-id="a6c1f-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a6c1f-112">Application</span></span> | <span data-ttu-id="a6c1f-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a6c1f-113">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a6c1f-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a6c1f-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /groupLifecyclePolicies/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="a6c1f-115">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a6c1f-115">Optional request headers</span></span>
| <span data-ttu-id="a6c1f-116">名前</span><span class="sxs-lookup"><span data-stu-id="a6c1f-116">Name</span></span> | <span data-ttu-id="a6c1f-117">説明</span><span class="sxs-lookup"><span data-stu-id="a6c1f-117">Description</span></span> |
|:-----------|:-----------|
| <span data-ttu-id="a6c1f-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="a6c1f-118">Authorization</span></span> | <span data-ttu-id="a6c1f-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="a6c1f-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a6c1f-121">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a6c1f-121">Content-Type</span></span>  | <span data-ttu-id="a6c1f-122">application/json</span><span class="sxs-lookup"><span data-stu-id="a6c1f-122">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a6c1f-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="a6c1f-123">Request body</span></span>

<span data-ttu-id="a6c1f-124">要求本文で、更新する関連フィールドの値を指定します。</span><span class="sxs-lookup"><span data-stu-id="a6c1f-124">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="a6c1f-125">要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変更に基づいて再計算されます。</span><span class="sxs-lookup"><span data-stu-id="a6c1f-125">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="a6c1f-126">最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="a6c1f-126">For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="a6c1f-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a6c1f-127">Property</span></span> | <span data-ttu-id="a6c1f-128">型</span><span class="sxs-lookup"><span data-stu-id="a6c1f-128">Type</span></span> | <span data-ttu-id="a6c1f-129">説明</span><span class="sxs-lookup"><span data-stu-id="a6c1f-129">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="a6c1f-130">alternateNotificationEmails</span><span class="sxs-lookup"><span data-stu-id="a6c1f-130">alternateNotificationEmails</span></span>|<span data-ttu-id="a6c1f-131">String</span><span class="sxs-lookup"><span data-stu-id="a6c1f-131">String</span></span>| <span data-ttu-id="a6c1f-132">所有者のいないグループに対して通知を送信する電子メール アドレスのリスト</span><span class="sxs-lookup"><span data-stu-id="a6c1f-132">List of email address to send notifications for groups without owners.</span></span> <span data-ttu-id="a6c1f-133">電子メール アドレスをセミコロンで区切って、複数の電子メール アドレスを定義することができます。</span><span class="sxs-lookup"><span data-stu-id="a6c1f-133">Multiple email address can be defined by separating email address with a semicolon.</span></span> |
|<span data-ttu-id="a6c1f-134">groupLifetimeInDays</span><span class="sxs-lookup"><span data-stu-id="a6c1f-134">groupLifetimeInDays</span></span>|<span data-ttu-id="a6c1f-135">Int32</span><span class="sxs-lookup"><span data-stu-id="a6c1f-135">Int32</span></span>| <span data-ttu-id="a6c1f-136">グループの有効期限が切れ、更新が必要になるまでの日数。</span><span class="sxs-lookup"><span data-stu-id="a6c1f-136">Number of days before a group expires and needs to be renewed.</span></span> <span data-ttu-id="a6c1f-137">更新されると、グループの有効期限は定義された日数、延長されます。</span><span class="sxs-lookup"><span data-stu-id="a6c1f-137">Once renewed, the group expiration is extended by the number of days defined.</span></span> |
|<span data-ttu-id="a6c1f-138">managedGroupTypes</span><span class="sxs-lookup"><span data-stu-id="a6c1f-138">managedGroupTypes</span></span>|<span data-ttu-id="a6c1f-139">String</span><span class="sxs-lookup"><span data-stu-id="a6c1f-139">String</span></span>| <span data-ttu-id="a6c1f-140">有効期限ポリシーを適用するグループの種類。</span><span class="sxs-lookup"><span data-stu-id="a6c1f-140">The group type for which the expiration policy applies.</span></span> <span data-ttu-id="a6c1f-141">可能な値は、**All**、**Selected**、または **None** です。</span><span class="sxs-lookup"><span data-stu-id="a6c1f-141">Possible values are **All**, **Selected** or **None**.</span></span> |

## <a name="response"></a><span data-ttu-id="a6c1f-142">応答</span><span class="sxs-lookup"><span data-stu-id="a6c1f-142">Response</span></span>

<span data-ttu-id="a6c1f-143">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="a6c1f-143">If successful, this method returns a `200 OK` response code and updated [Chart](../resources/grouplifecyclepolicy.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a6c1f-144">例</span><span class="sxs-lookup"><span data-stu-id="a6c1f-144">Example</span></span>

##### <a name="request"></a><span data-ttu-id="a6c1f-145">要求</span><span class="sxs-lookup"><span data-stu-id="a6c1f-145">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "update_grouplifecyclepolicy"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/groupLifecyclePolicies/{id}
Content-type: application/json
Content-length: 125

{
  "groupLifetimeInDays": 180,
  "managedGroupTypes": "Selected",
  "alternateNotificationEmails": "admin@contoso.com"
}
```
##### <a name="response"></a><span data-ttu-id="a6c1f-146">応答</span><span class="sxs-lookup"><span data-stu-id="a6c1f-146">Response</span></span>
<span data-ttu-id="a6c1f-147">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="a6c1f-147">Note: The response object shown here may be truncated for brevity.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupLifecyclePolicy"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 146

{
  "id": "id-value",
  "groupLifetimeInDays": 180,
  "managedGroupTypes": "Selected",
  "alternateNotificationEmails": "admin@contoso.com"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update groupLifecyclePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->