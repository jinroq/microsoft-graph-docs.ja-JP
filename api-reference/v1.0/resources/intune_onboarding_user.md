# <a name="user-resource-type"></a><span data-ttu-id="f6f30-101">user リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f6f30-101">user resource type</span></span>

> <span data-ttu-id="f6f30-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="f6f30-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f6f30-103">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="f6f30-103">Not yet documented</span></span>
## <a name="methods"></a><span data-ttu-id="f6f30-104">メソッド</span><span class="sxs-lookup"><span data-stu-id="f6f30-104">Methods</span></span>
|<span data-ttu-id="f6f30-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="f6f30-105">Method</span></span>|<span data-ttu-id="f6f30-106">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="f6f30-106">Return Type</span></span>|<span data-ttu-id="f6f30-107">説明</span><span class="sxs-lookup"><span data-stu-id="f6f30-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="f6f30-108">List users</span><span class="sxs-lookup"><span data-stu-id="f6f30-108">List users</span></span>](../api/intune_onboarding_user_list.md)|<span data-ttu-id="f6f30-109">[user](../resources/intune_onboarding_user.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="f6f30-109">[user](../resources/intune_onboarding_user.md) collection</span></span>|<span data-ttu-id="f6f30-110">[user](../resources/intune_onboarding_user.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="f6f30-110">List properties and relationships of the [user](../resources/intune_onboarding_user.md) objects.</span></span>|
|[<span data-ttu-id="f6f30-111">Get user</span><span class="sxs-lookup"><span data-stu-id="f6f30-111">Get user</span></span>](../api/intune_onboarding_user_get.md)|[<span data-ttu-id="f6f30-112">user</span><span class="sxs-lookup"><span data-stu-id="f6f30-112">user</span></span>](../resources/intune_onboarding_user.md)|<span data-ttu-id="f6f30-113">[user](../resources/intune_onboarding_user.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="f6f30-113">Read properties and relationships of [plannerTaskDetails](../resources/intune_onboarding_user.md) object.</span></span>|
|[<span data-ttu-id="f6f30-114">Create user</span><span class="sxs-lookup"><span data-stu-id="f6f30-114">Create user</span></span>](../api/intune_onboarding_user_create.md)|[<span data-ttu-id="f6f30-115">user</span><span class="sxs-lookup"><span data-stu-id="f6f30-115">user</span></span>](../resources/intune_onboarding_user.md)|<span data-ttu-id="f6f30-116">新しい [user](../resources/intune_onboarding_user.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="f6f30-116">Create a new user object.</span></span>|
|[<span data-ttu-id="f6f30-117">Delete user</span><span class="sxs-lookup"><span data-stu-id="f6f30-117">Delete user</span></span>](../api/intune_onboarding_user_delete.md)|<span data-ttu-id="f6f30-118">なし</span><span class="sxs-lookup"><span data-stu-id="f6f30-118">None</span></span>|<span data-ttu-id="f6f30-119">[user](../resources/intune_onboarding_user.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="f6f30-119">Deletes a [user](../resources/intune_onboarding_user.md).</span></span>|
|[<span data-ttu-id="f6f30-120">Update user</span><span class="sxs-lookup"><span data-stu-id="f6f30-120">Update user</span></span>](../api/intune_onboarding_user_update.md)|[<span data-ttu-id="f6f30-121">user</span><span class="sxs-lookup"><span data-stu-id="f6f30-121">user</span></span>](../resources/intune_onboarding_user.md)|<span data-ttu-id="f6f30-122">[user](../resources/intune_onboarding_user.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="f6f30-122">Update the properties of a user object.</span></span>|

## <a name="properties"></a><span data-ttu-id="f6f30-123">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f6f30-123">Properties</span></span>
|<span data-ttu-id="f6f30-124">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f6f30-124">Property</span></span>|<span data-ttu-id="f6f30-125">型</span><span class="sxs-lookup"><span data-stu-id="f6f30-125">Type</span></span>|<span data-ttu-id="f6f30-126">説明</span><span class="sxs-lookup"><span data-stu-id="f6f30-126">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f6f30-127">id</span><span class="sxs-lookup"><span data-stu-id="f6f30-127">id</span></span>|<span data-ttu-id="f6f30-128">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="f6f30-128">String</span></span>|<span data-ttu-id="f6f30-129">ユーザーの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="f6f30-129">Unique identifier of the folder.</span></span>|
|<span data-ttu-id="f6f30-130">deviceEnrollmentLimit</span><span class="sxs-lookup"><span data-stu-id="f6f30-130">deviceEnrollmentLimit</span></span>|<span data-ttu-id="f6f30-131">Int32</span><span class="sxs-lookup"><span data-stu-id="f6f30-131">Int32</span></span>|<span data-ttu-id="f6f30-132">ユーザーが登録を許可されているデバイスの最大数。</span><span class="sxs-lookup"><span data-stu-id="f6f30-132">The limit on the maximum number of devices that the user is permitted to enroll.</span></span> <span data-ttu-id="f6f30-133">使用できる値は 5 または 1000 です。</span><span class="sxs-lookup"><span data-stu-id="f6f30-133">Allowed values are 5 or 1000.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f6f30-134">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="f6f30-134">Relationships</span></span>
<span data-ttu-id="f6f30-135">なし</span><span class="sxs-lookup"><span data-stu-id="f6f30-135">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="f6f30-136">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f6f30-136">JSON Representation</span></span>
<span data-ttu-id="f6f30-137">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="f6f30-137">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.user"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.user",
  "id": "String (identifier)",
  "deviceEnrollmentLimit": 1024
}
```



