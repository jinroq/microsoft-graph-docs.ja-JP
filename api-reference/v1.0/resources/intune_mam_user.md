# <a name="user-resource-type"></a><span data-ttu-id="64fe0-101">user リソースの種類</span><span class="sxs-lookup"><span data-stu-id="64fe0-101">user resource type</span></span>

> <span data-ttu-id="64fe0-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="64fe0-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="64fe0-103">Azure Active Directory ユーザー オブジェクトを表します。</span><span class="sxs-lookup"><span data-stu-id="64fe0-103">Represents an Azure Active Directory user object.</span></span>
## <a name="methods"></a><span data-ttu-id="64fe0-104">メソッド</span><span class="sxs-lookup"><span data-stu-id="64fe0-104">Methods</span></span>
|<span data-ttu-id="64fe0-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="64fe0-105">Method</span></span>|<span data-ttu-id="64fe0-106">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="64fe0-106">Return Type</span></span>|<span data-ttu-id="64fe0-107">説明</span><span class="sxs-lookup"><span data-stu-id="64fe0-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="64fe0-108">List users</span><span class="sxs-lookup"><span data-stu-id="64fe0-108">List users</span></span>](../api/intune_mam_user_list.md)|<span data-ttu-id="64fe0-109">[user](../resources/intune_mam_user.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="64fe0-109">[user](../resources/intune_mam_user.md) collection</span></span>|<span data-ttu-id="64fe0-110">[user](../resources/intune_mam_user.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="64fe0-110">List properties and relationships of the [user](../resources/intune_mam_user.md) objects.</span></span>|
|[<span data-ttu-id="64fe0-111">Get user</span><span class="sxs-lookup"><span data-stu-id="64fe0-111">Get user</span></span>](../api/intune_mam_user_get.md)|[<span data-ttu-id="64fe0-112">user</span><span class="sxs-lookup"><span data-stu-id="64fe0-112">user</span></span>](../resources/intune_mam_user.md)|<span data-ttu-id="64fe0-113">[user](../resources/intune_mam_user.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="64fe0-113">Read properties and relationships of [plannerTaskDetails](../resources/intune_mam_user.md) object.</span></span>|
|[<span data-ttu-id="64fe0-114">Create user</span><span class="sxs-lookup"><span data-stu-id="64fe0-114">Create user</span></span>](../api/intune_mam_user_create.md)|[<span data-ttu-id="64fe0-115">user</span><span class="sxs-lookup"><span data-stu-id="64fe0-115">user</span></span>](../resources/intune_mam_user.md)|<span data-ttu-id="64fe0-116">新しい [user](../resources/intune_mam_user.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="64fe0-116">Create a new user object.</span></span>|
|[<span data-ttu-id="64fe0-117">Delete user</span><span class="sxs-lookup"><span data-stu-id="64fe0-117">Delete user</span></span>](../api/intune_mam_user_delete.md)|<span data-ttu-id="64fe0-118">なし</span><span class="sxs-lookup"><span data-stu-id="64fe0-118">None</span></span>|<span data-ttu-id="64fe0-119">[user](../resources/intune_mam_user.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="64fe0-119">Deletes a [user](../resources/intune_mam_user.md).</span></span>|
|[<span data-ttu-id="64fe0-120">Update user</span><span class="sxs-lookup"><span data-stu-id="64fe0-120">Update user</span></span>](../api/intune_mam_user_update.md)|[<span data-ttu-id="64fe0-121">user</span><span class="sxs-lookup"><span data-stu-id="64fe0-121">user</span></span>](../resources/intune_mam_user.md)|<span data-ttu-id="64fe0-122">[user](../resources/intune_mam_user.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="64fe0-122">Update the properties of a user object.</span></span>|
|[<span data-ttu-id="64fe0-123">getManagedAppDiagnosticStatuses 関数</span><span class="sxs-lookup"><span data-stu-id="64fe0-123">getManagedAppDiagnosticStatuses function</span></span>](../api/intune_mam_user_getmanagedappdiagnosticstatuses.md)|<span data-ttu-id="64fe0-124">[managedAppDiagnosticStatus](../resources/intune_mam_managedappdiagnosticstatus.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="64fe0-124">[managedAppDiagnosticStatus](../resources/intune_mam_managedappdiagnosticstatus.md) collection</span></span>|<span data-ttu-id="64fe0-125">特定のユーザーの診断検証状態を取得します。</span><span class="sxs-lookup"><span data-stu-id="64fe0-125">Gets diagnostics validation status for a given user.</span></span>|
|[<span data-ttu-id="64fe0-126">getManagedAppPolicies 関数</span><span class="sxs-lookup"><span data-stu-id="64fe0-126">getManagedAppPolicies function</span></span>](../api/intune_mam_user_getmanagedapppolicies.md)|<span data-ttu-id="64fe0-127">[managedAppPolicy](../resources/intune_mam_managedapppolicy.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="64fe0-127">[managedAppPolicy](../resources/intune_mam_managedapppolicy.md) collection</span></span>|<span data-ttu-id="64fe0-128">特定のユーザーのアプリ制限を取得します。</span><span class="sxs-lookup"><span data-stu-id="64fe0-128">Gets app restrictions for a given user.</span></span>|
|[<span data-ttu-id="64fe0-129">wipeManagedAppRegistrationsByDeviceTag アクション</span><span class="sxs-lookup"><span data-stu-id="64fe0-129">wipeManagedAppRegistrationsByDeviceTag action</span></span>](../api/intune_mam_user_wipemanagedappregistrationsbydevicetag.md)|<span data-ttu-id="64fe0-130">なし</span><span class="sxs-lookup"><span data-stu-id="64fe0-130">None</span></span>|<span data-ttu-id="64fe0-131">指定されたデバイス タグが含まれるアプリ登録でワイプ操作を実行します。</span><span class="sxs-lookup"><span data-stu-id="64fe0-131">Issues a wipe operation on an app registration with specified device tag.</span></span>|

## <a name="properties"></a><span data-ttu-id="64fe0-132">プロパティ</span><span class="sxs-lookup"><span data-stu-id="64fe0-132">Properties</span></span>
|<span data-ttu-id="64fe0-133">プロパティ</span><span class="sxs-lookup"><span data-stu-id="64fe0-133">Property</span></span>|<span data-ttu-id="64fe0-134">型</span><span class="sxs-lookup"><span data-stu-id="64fe0-134">Type</span></span>|<span data-ttu-id="64fe0-135">説明</span><span class="sxs-lookup"><span data-stu-id="64fe0-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="64fe0-136">id</span><span class="sxs-lookup"><span data-stu-id="64fe0-136">id</span></span>|<span data-ttu-id="64fe0-137">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="64fe0-137">String</span></span>|<span data-ttu-id="64fe0-138">ユーザー ID。</span><span class="sxs-lookup"><span data-stu-id="64fe0-138">The user unique identifier.</span></span>|

## <a name="relationships"></a><span data-ttu-id="64fe0-139">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="64fe0-139">Relationships</span></span>
|<span data-ttu-id="64fe0-140">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="64fe0-140">Relationship</span></span>|<span data-ttu-id="64fe0-141">型</span><span class="sxs-lookup"><span data-stu-id="64fe0-141">Type</span></span>|<span data-ttu-id="64fe0-142">説明</span><span class="sxs-lookup"><span data-stu-id="64fe0-142">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="64fe0-143">managedAppRegistrations</span><span class="sxs-lookup"><span data-stu-id="64fe0-143">managedAppRegistrations</span></span>|<span data-ttu-id="64fe0-144">[managedAppRegistration](../resources/intune_mam_managedappregistration.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="64fe0-144">[managedAppRegistration](../resources/intune_mam_managedappregistration.md) collection</span></span>|<span data-ttu-id="64fe0-145">対象ユーザーに属する 0 個以上の管理対象アプリ登録。</span><span class="sxs-lookup"><span data-stu-id="64fe0-145">Zero or more managed app registrations that belong to the user.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="64fe0-146">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="64fe0-146">JSON Representation</span></span>
<span data-ttu-id="64fe0-147">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="64fe0-147">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.user"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.user",
  "id": "String (identifier)"
}
```



