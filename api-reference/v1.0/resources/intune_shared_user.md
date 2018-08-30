# <a name="user-resource-type"></a><span data-ttu-id="29a6c-101">user リソースの種類</span><span class="sxs-lookup"><span data-stu-id="29a6c-101">user resource type</span></span>

> <span data-ttu-id="29a6c-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="29a6c-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="29a6c-103">Azure Active Directory ユーザー オブジェクトを表します。</span><span class="sxs-lookup"><span data-stu-id="29a6c-103">Represents an Azure Active Directory user object.</span></span>

## <a name="methods"></a><span data-ttu-id="29a6c-104">メソッド</span><span class="sxs-lookup"><span data-stu-id="29a6c-104">Methods</span></span>
|<span data-ttu-id="29a6c-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="29a6c-105">Method</span></span>|<span data-ttu-id="29a6c-106">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="29a6c-106">Return Type</span></span>|<span data-ttu-id="29a6c-107">説明</span><span class="sxs-lookup"><span data-stu-id="29a6c-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="29a6c-108">[ユーザー](../api/intune_shared_user_list.md) オブジェクト をリストする</span><span class="sxs-lookup"><span data-stu-id="29a6c-108">[List users](../api/intune_shared_user_list.md) objects.</span></span>|
|<span data-ttu-id="29a6c-109">オブジェクトの[ユーザーを取得](../api/intune_shared_user_get.md) する</span><span class="sxs-lookup"><span data-stu-id="29a6c-109">[Get user](../api/intune_shared_user_get.md) object.</span></span>|
|<span data-ttu-id="29a6c-110">[ユーザー](../api/intune_shared_user_create.md) オブジェクトを作成する</span><span class="sxs-lookup"><span data-stu-id="29a6c-110">Create a new [user](../api/intune_shared_user_create.md) object.</span></span>|
|<span data-ttu-id="29a6c-111">[ユーザーを削除する](../api/intune_shared_user_delete.md)</span><span class="sxs-lookup"><span data-stu-id="29a6c-111">Delete user</span></span>|
|<span data-ttu-id="29a6c-112">[ユーザー](../api/intune_shared_user_update.md) オブジェクトを更新する</span><span class="sxs-lookup"><span data-stu-id="29a6c-112">Update user object.</span></span>|
|<span data-ttu-id="29a6c-113">**デバイス管理**</span><span class="sxs-lookup"><span data-stu-id="29a6c-113">**Device management**</span></span>|
|[<span data-ttu-id="29a6c-114">removeAllDevicesFromManagement 操作</span><span class="sxs-lookup"><span data-stu-id="29a6c-114">removeAllDevicesFromManagement action</span></span>](../api/intune_shared_user_removealldevicesfrommanagement.md)|<span data-ttu-id="29a6c-115">なし</span><span class="sxs-lookup"><span data-stu-id="29a6c-115">None</span></span>|<span data-ttu-id="29a6c-116">対象ユーザーの管理からすべてのデバイスを破棄します</span><span class="sxs-lookup"><span data-stu-id="29a6c-116">Retire all devices from management for this user</span></span>|
|<span data-ttu-id="29a6c-117">**モバイル アプリケーション管理 (MAM)**</span><span class="sxs-lookup"><span data-stu-id="29a6c-117">**Mobile app management (MAM)**</span></span>|
|[<span data-ttu-id="29a6c-118">getManagedAppDiagnosticStatuses 関数</span><span class="sxs-lookup"><span data-stu-id="29a6c-118">getManagedAppDiagnosticStatuses function</span></span>](../api/intune_shared_user_getmanagedappdiagnosticstatuses.md)|<span data-ttu-id="29a6c-119">[managedAppDiagnosticStatus](../resources/intune_mam_managedappdiagnosticstatus.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="29a6c-119">[managedAppDiagnosticStatus](../resources/intune_mam_managedappdiagnosticstatus.md) collection</span></span>|<span data-ttu-id="29a6c-120">特定のユーザーの診断検証状態を取得します。</span><span class="sxs-lookup"><span data-stu-id="29a6c-120">Gets diagnostics validation status for a given user.</span></span>|
|[<span data-ttu-id="29a6c-121">getManagedAppPolicies 関数</span><span class="sxs-lookup"><span data-stu-id="29a6c-121">getManagedAppPolicies function</span></span>](../api/intune_shared_user_getmanagedapppolicies.md)|<span data-ttu-id="29a6c-122">[managedAppPolicy](../resources/intune_mam_managedapppolicy.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="29a6c-122">[managedAppPolicy](../resources/intune_mam_managedapppolicy.md) collection</span></span>|<span data-ttu-id="29a6c-123">特定のユーザーのアプリ制限を取得します。</span><span class="sxs-lookup"><span data-stu-id="29a6c-123">Gets app restrictions for a given user.</span></span>|
|[<span data-ttu-id="29a6c-124">wipeManagedAppRegistrationsByDeviceTag アクション</span><span class="sxs-lookup"><span data-stu-id="29a6c-124">wipeManagedAppRegistrationsByDeviceTag action</span></span>](../api/intune_shared_user_wipemanagedappregistrationsbydevicetag.md)|<span data-ttu-id="29a6c-125">なし</span><span class="sxs-lookup"><span data-stu-id="29a6c-125">None</span></span>|<span data-ttu-id="29a6c-126">指定されたデバイス タグが含まれるアプリ登録でワイプ操作を実行します。</span><span class="sxs-lookup"><span data-stu-id="29a6c-126">Issues a wipe operation on an app registration with specified device tag.</span></span>|

## <a name="properties"></a><span data-ttu-id="29a6c-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="29a6c-127">Properties</span></span>
|<span data-ttu-id="29a6c-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="29a6c-128">Property</span></span>|<span data-ttu-id="29a6c-129">タイプ</span><span class="sxs-lookup"><span data-stu-id="29a6c-129">Type</span></span>|<span data-ttu-id="29a6c-130">説明</span><span class="sxs-lookup"><span data-stu-id="29a6c-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="29a6c-131">id</span><span class="sxs-lookup"><span data-stu-id="29a6c-131">id</span></span>|<span data-ttu-id="29a6c-132">文字列</span><span class="sxs-lookup"><span data-stu-id="29a6c-132">String</span></span>|<span data-ttu-id="29a6c-133">ユーザーの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="29a6c-133">Unique identifier of the user.</span></span>|
|<span data-ttu-id="29a6c-134">**採用**</span><span class="sxs-lookup"><span data-stu-id="29a6c-134">**On-boarding**</span></span>|
|<span data-ttu-id="29a6c-135">deviceEnrollmentLimit</span><span class="sxs-lookup"><span data-stu-id="29a6c-135">deviceEnrollmentLimit</span></span>|<span data-ttu-id="29a6c-136">Int32</span><span class="sxs-lookup"><span data-stu-id="29a6c-136">Int32</span></span>|<span data-ttu-id="29a6c-137">ユーザーが登録を許可されているデバイスの最大数。</span><span class="sxs-lookup"><span data-stu-id="29a6c-137">The limit on the maximum number of devices that the user is permitted to enroll.</span></span> <span data-ttu-id="29a6c-138">使用できる値は 5 または 1000 です。</span><span class="sxs-lookup"><span data-stu-id="29a6c-138">Allowed values are 5 or 1000.</span></span>|


## <a name="relationships"></a><span data-ttu-id="29a6c-139">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="29a6c-139">Relationships</span></span>
|<span data-ttu-id="29a6c-140">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="29a6c-140">Relationship</span></span>|<span data-ttu-id="29a6c-141">型</span><span class="sxs-lookup"><span data-stu-id="29a6c-141">Type</span></span>|<span data-ttu-id="29a6c-142">説明</span><span class="sxs-lookup"><span data-stu-id="29a6c-142">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="29a6c-143">**デバイス管理**</span><span class="sxs-lookup"><span data-stu-id="29a6c-143">**Device management**</span></span>|
|<span data-ttu-id="29a6c-144">managedDevices</span><span class="sxs-lookup"><span data-stu-id="29a6c-144">managedDevices</span></span>|<span data-ttu-id="29a6c-145">[managedDevice](../resources/intune_devices_manageddevice.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="29a6c-145">[managedDevice](../resources/intune_devices_manageddevice.md) collection</span></span>|<span data-ttu-id="29a6c-146">対象ユーザーに関連付けられている管理対象デバイス。</span><span class="sxs-lookup"><span data-stu-id="29a6c-146">The managed devices associated with the user.</span></span>|
|<span data-ttu-id="29a6c-147">**モバイル アプリケーション管理 (MAM)**</span><span class="sxs-lookup"><span data-stu-id="29a6c-147">**Mobile app management (MAM)**</span></span>|
|<span data-ttu-id="29a6c-148">managedAppRegistrations</span><span class="sxs-lookup"><span data-stu-id="29a6c-148">managedAppRegistrations</span></span>|<span data-ttu-id="29a6c-149">[managedAppRegistration](../resources/intune_mam_managedappregistration.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="29a6c-149">[managedAppRegistration](../resources/intune_mam_managedappregistration.md) collection</span></span>|<span data-ttu-id="29a6c-150">対象ユーザーに属する 0 個以上の管理対象アプリ登録。</span><span class="sxs-lookup"><span data-stu-id="29a6c-150">Zero or more managed app registrations that belong to the user.</span></span>|
|<span data-ttu-id="29a6c-151">**トラブルシューティング**</span><span class="sxs-lookup"><span data-stu-id="29a6c-151">**Troubleshooting**</span></span>|
|<span data-ttu-id="29a6c-152">deviceManagementTroubleshootingEvents</span><span class="sxs-lookup"><span data-stu-id="29a6c-152">deviceManagementTroubleshootingEvents</span></span>|<span data-ttu-id="29a6c-153">[deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="29a6c-153">[deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md) collection</span></span>|<span data-ttu-id="29a6c-154">対象ユーザーのトラブルシューティング イベントの一覧です。</span><span class="sxs-lookup"><span data-stu-id="29a6c-154">The list of troubleshooting events for this user.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="29a6c-155">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="29a6c-155">JSON Representation</span></span>
<span data-ttu-id="29a6c-156">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="29a6c-156">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.directoryObject",
  "openType": true,
  "@odata.type": "microsoft.graph.user"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.user",
  "id": "String (identifier)",
  "deviceEnrollmentLimit": 5
}
```

<!-- {
  "type": "#page.annotation",
  "suppressions": [
    "Warning: Resource microsoft.graph.user is defined in multiple files: /api-reference/v1.0/resources/intune_shared_user.md, /api-reference/v1.0/resources/user.md",
  ]
}-->
