# <a name="managedappregistration-resource-type"></a><span data-ttu-id="42ad4-101">managedAppRegistration リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="42ad4-101">managedAppRegistration resource type</span></span>

> <span data-ttu-id="42ad4-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="42ad4-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="42ad4-103">ManagedAppEntity は、アプリ管理ワークフロー下にある他のすべてのエンティティ タイプの基本型です。</span><span class="sxs-lookup"><span data-stu-id="42ad4-103">The ManagedAppEntity is the base entity type for all other entity types under app management workflow.</span></span>
<span data-ttu-id="42ad4-104">ManagedAppRegistration リソースは、組織のメンバーに使用されるアプリの詳細を管理機能と共に示します。</span><span class="sxs-lookup"><span data-stu-id="42ad4-104">The ManagedAppRegistration resource represents the details of an app, with management capability, used by a member of the organization.</span></span>
## <a name="methods"></a><span data-ttu-id="42ad4-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="42ad4-105">Methods</span></span>
|<span data-ttu-id="42ad4-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="42ad4-106">Method</span></span>|<span data-ttu-id="42ad4-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="42ad4-107">Return Type</span></span>|<span data-ttu-id="42ad4-108">説明</span><span class="sxs-lookup"><span data-stu-id="42ad4-108">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="42ad4-109">List managedAppRegistrations</span><span class="sxs-lookup"><span data-stu-id="42ad4-109">List managedAppRegistrations</span></span>](../api/intune_mam_managedappregistration_list.md)|<span data-ttu-id="42ad4-110">[managedAppRegistration](../resources/intune_mam_managedappregistration.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="42ad4-110">[managedAppRegistration](../resources/intune_mam_managedappregistration.md) collection</span></span>|<span data-ttu-id="42ad4-111">[managedAppRegistration](../resources/intune_mam_managedappregistration.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="42ad4-111">List properties and relationships of the [managedAppRegistration](../resources/intune_mam_managedappregistration.md) objects.</span></span>|
|[<span data-ttu-id="42ad4-112">Get managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="42ad4-112">Get managedAppRegistration</span></span>](../api/intune_mam_managedappregistration_get.md)|[<span data-ttu-id="42ad4-113">managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="42ad4-113">managedAppRegistration</span></span>](../resources/intune_mam_managedappregistration.md)|<span data-ttu-id="42ad4-114">[managedAppRegistration](../resources/intune_mam_managedappregistration.md) オブジェクトのプロパティとリレーションを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="42ad4-114">Read properties and relationships of [plannerTaskDetails](../resources/intune_mam_managedappregistration.md) object.</span></span>|
|[<span data-ttu-id="42ad4-115">getUserIdsWithFlaggedAppRegistration function</span><span class="sxs-lookup"><span data-stu-id="42ad4-115">getUserIdsWithFlaggedAppRegistration function</span></span>](../api/intune_mam_managedappregistration_getuseridswithflaggedappregistration.md)|<span data-ttu-id="42ad4-116">String コレクション</span><span class="sxs-lookup"><span data-stu-id="42ad4-116">String collection</span></span>|<span data-ttu-id="42ad4-117">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="42ad4-117">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="42ad4-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="42ad4-118">Properties</span></span>
|<span data-ttu-id="42ad4-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="42ad4-119">Property</span></span>|<span data-ttu-id="42ad4-120">型</span><span class="sxs-lookup"><span data-stu-id="42ad4-120">Type</span></span>|<span data-ttu-id="42ad4-121">説明</span><span class="sxs-lookup"><span data-stu-id="42ad4-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="42ad4-122">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="42ad4-122">createdDateTime</span></span>|<span data-ttu-id="42ad4-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="42ad4-123">DateTimeOffset</span></span>|<span data-ttu-id="42ad4-124">作成日時</span><span class="sxs-lookup"><span data-stu-id="42ad4-124">Date and time of cube creation.</span></span>|
|<span data-ttu-id="42ad4-125">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="42ad4-125">lastSyncDateTime</span></span>|<span data-ttu-id="42ad4-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="42ad4-126">DateTimeOffset</span></span>|<span data-ttu-id="42ad4-127">アプリが管理サービスと最後に同期した日付と時刻。</span><span class="sxs-lookup"><span data-stu-id="42ad4-127">Date and time of last the app synced with management service.</span></span>|
|<span data-ttu-id="42ad4-128">applicationVersion</span><span class="sxs-lookup"><span data-stu-id="42ad4-128">applicationVersion</span></span>|<span data-ttu-id="42ad4-129">String</span><span class="sxs-lookup"><span data-stu-id="42ad4-129">String</span></span>|<span data-ttu-id="42ad4-130">アプリのバージョン</span><span class="sxs-lookup"><span data-stu-id="42ad4-130">App version</span></span>|
|<span data-ttu-id="42ad4-131">managementSdkVersion</span><span class="sxs-lookup"><span data-stu-id="42ad4-131">managementSdkVersion</span></span>|<span data-ttu-id="42ad4-132">String</span><span class="sxs-lookup"><span data-stu-id="42ad4-132">String</span></span>|<span data-ttu-id="42ad4-133">アプリ管理の SDK バージョン</span><span class="sxs-lookup"><span data-stu-id="42ad4-133">App management SDK version</span></span>|
|<span data-ttu-id="42ad4-134">platformVersion</span><span class="sxs-lookup"><span data-stu-id="42ad4-134">platformVersion</span></span>|<span data-ttu-id="42ad4-135">String</span><span class="sxs-lookup"><span data-stu-id="42ad4-135">String</span></span>|<span data-ttu-id="42ad4-136">オペレーティング システムのバージョン</span><span class="sxs-lookup"><span data-stu-id="42ad4-136">Operating System version</span></span>|
|<span data-ttu-id="42ad4-137">deviceType</span><span class="sxs-lookup"><span data-stu-id="42ad4-137">DeviceType</span></span>|<span data-ttu-id="42ad4-138">String</span><span class="sxs-lookup"><span data-stu-id="42ad4-138">String</span></span>|<span data-ttu-id="42ad4-139">ホスト デバイスの種類</span><span class="sxs-lookup"><span data-stu-id="42ad4-139">Host device type</span></span>|
|<span data-ttu-id="42ad4-140">deviceTag</span><span class="sxs-lookup"><span data-stu-id="42ad4-140">deviceTag</span></span>|<span data-ttu-id="42ad4-141">String</span><span class="sxs-lookup"><span data-stu-id="42ad4-141">String</span></span>|<span data-ttu-id="42ad4-142">アプリ管理 SDK が生成したタグ。同じデバイス上にホストされているアプリを関連付けるのに役立ちます。</span><span class="sxs-lookup"><span data-stu-id="42ad4-142">App management SDK generated tag, which helps relate apps hosted on the same device.</span></span> <span data-ttu-id="42ad4-143">あらゆる状況でのアプリの関連付けを保証するものではありません。</span><span class="sxs-lookup"><span data-stu-id="42ad4-143">Not guaranteed to relate apps in all conditions.</span></span>|
|<span data-ttu-id="42ad4-144">deviceName</span><span class="sxs-lookup"><span data-stu-id="42ad4-144">DeviceName</span></span>|<span data-ttu-id="42ad4-145">String</span><span class="sxs-lookup"><span data-stu-id="42ad4-145">String</span></span>|<span data-ttu-id="42ad4-146">ホスト デバイスの名前</span><span class="sxs-lookup"><span data-stu-id="42ad4-146">Host device name</span></span>|
|<span data-ttu-id="42ad4-147">flaggedReasons</span><span class="sxs-lookup"><span data-stu-id="42ad4-147">flaggedReasons</span></span>|<span data-ttu-id="42ad4-148">String コレクション</span><span class="sxs-lookup"><span data-stu-id="42ad4-148">String collection</span></span>|<span data-ttu-id="42ad4-149">アプリ登録にフラグが付けられた、0 個以上の理由。</span><span class="sxs-lookup"><span data-stu-id="42ad4-149">Zero or more reasons an app registration is flagged.</span></span> <span data-ttu-id="42ad4-150">例:</span><span class="sxs-lookup"><span data-stu-id="42ad4-150">E.g.</span></span> <span data-ttu-id="42ad4-151">ルートのデバイスで実行されているアプリ</span><span class="sxs-lookup"><span data-stu-id="42ad4-151">app running on rooted device</span></span>|
|<span data-ttu-id="42ad4-152">userId</span><span class="sxs-lookup"><span data-stu-id="42ad4-152">userId</span></span>|<span data-ttu-id="42ad4-153">String</span><span class="sxs-lookup"><span data-stu-id="42ad4-153">String</span></span>|<span data-ttu-id="42ad4-154">このアプリの登録が属するユーザー ID。</span><span class="sxs-lookup"><span data-stu-id="42ad4-154">The user Id to who this app registration belongs.</span></span>|
|<span data-ttu-id="42ad4-155">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="42ad4-155">appIdentifier</span></span>|[<span data-ttu-id="42ad4-156">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="42ad4-156">mobileAppIdentifier</span></span>](../resources/intune_mam_mobileappidentifier.md)|<span data-ttu-id="42ad4-157">アプリ パッケージの識別子</span><span class="sxs-lookup"><span data-stu-id="42ad4-157">The app package Identifier</span></span>|
|<span data-ttu-id="42ad4-158">id</span><span class="sxs-lookup"><span data-stu-id="42ad4-158">id</span></span>|<span data-ttu-id="42ad4-159">String</span><span class="sxs-lookup"><span data-stu-id="42ad4-159">String</span></span>|<span data-ttu-id="42ad4-160">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="42ad4-160">Name of the entity.</span></span>|
|<span data-ttu-id="42ad4-161">version</span><span class="sxs-lookup"><span data-stu-id="42ad4-161">version</span></span>|<span data-ttu-id="42ad4-162">String</span><span class="sxs-lookup"><span data-stu-id="42ad4-162">String</span></span>|<span data-ttu-id="42ad4-163">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="42ad4-163">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="42ad4-164">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="42ad4-164">Relationships</span></span>
|<span data-ttu-id="42ad4-165">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="42ad4-165">Relationship</span></span>|<span data-ttu-id="42ad4-166">型</span><span class="sxs-lookup"><span data-stu-id="42ad4-166">Type</span></span>|<span data-ttu-id="42ad4-167">説明</span><span class="sxs-lookup"><span data-stu-id="42ad4-167">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="42ad4-168">appliedPolicies</span><span class="sxs-lookup"><span data-stu-id="42ad4-168">appliedPolicies</span></span>|<span data-ttu-id="42ad4-169">[managedAppPolicy](../resources/intune_mam_managedapppolicy.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="42ad4-169">[managedAppPolicy](../resources/intune_mam_managedapppolicy.md) collection</span></span>|<span data-ttu-id="42ad4-170">登録済みのアプリが管理サービスと最後に同期したときに、既に適用されていた 0 個以上のポリシーです。</span><span class="sxs-lookup"><span data-stu-id="42ad4-170">Zero or more policys already applied on the registered app when it last synchronized with managment service.</span></span>|
|<span data-ttu-id="42ad4-171">intendedPolicies</span><span class="sxs-lookup"><span data-stu-id="42ad4-171">intendedPolicies</span></span>|<span data-ttu-id="42ad4-172">[managedAppPolicy](../resources/intune_mam_managedapppolicy.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="42ad4-172">[managedAppPolicy](../resources/intune_mam_managedapppolicy.md) collection</span></span>|<span data-ttu-id="42ad4-173">現時点で、管理者がアプリに対して意図した 0 個以上のポリシーです。</span><span class="sxs-lookup"><span data-stu-id="42ad4-173">Zero or more policies admin intended for the app as of now.</span></span>|
|<span data-ttu-id="42ad4-174">operations</span><span class="sxs-lookup"><span data-stu-id="42ad4-174">operations</span></span>|<span data-ttu-id="42ad4-175">[managedAppOperation](../resources/intune_mam_managedappoperation.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="42ad4-175">[managedAppOperation](../resources/intune_mam_managedappoperation.md) collection</span></span>|<span data-ttu-id="42ad4-176">アプリ登録でトリガーされた、0 個以上の長時間実行の操作です。</span><span class="sxs-lookup"><span data-stu-id="42ad4-176">Zero or more long running operations triggered on the app registration.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="42ad4-177">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="42ad4-177">JSON Representation</span></span>
<span data-ttu-id="42ad4-178">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="42ad4-178">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAppRegistration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppRegistration",
  "createdDateTime": "String (timestamp)",
  "lastSyncDateTime": "String (timestamp)",
  "applicationVersion": "String",
  "managementSdkVersion": "String",
  "platformVersion": "String",
  "deviceType": "String",
  "deviceTag": "String",
  "deviceName": "String",
  "flaggedReasons": [
    "String"
  ],
  "userId": "String",
  "appIdentifier": {
    "@odata.type": "microsoft.graph.mobileAppIdentifier"
  },
  "id": "String (identifier)",
  "version": "String"
}
```



