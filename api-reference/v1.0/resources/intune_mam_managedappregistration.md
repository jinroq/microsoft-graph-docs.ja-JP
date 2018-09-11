# <a name="managedappregistration-resource-type"></a><span data-ttu-id="47944-101">managedAppRegistration リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="47944-101">managedAppRegistration resource type</span></span>

> <span data-ttu-id="47944-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="47944-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="47944-103">ManagedAppEntity は、アプリ管理ワークフロー下にある他のすべてのエンティティ タイプの基本型です。</span><span class="sxs-lookup"><span data-stu-id="47944-103">The ManagedAppEntity is the base entity type for all other entity types under app management workflow.</span></span>
<span data-ttu-id="47944-104">ManagedAppRegistration リソースは、組織のメンバーに使用されるアプリの詳細を管理機能と共に示します。</span><span class="sxs-lookup"><span data-stu-id="47944-104">The ManagedAppRegistration resource represents the details of an app, with management capability, used by a member of the organization.</span></span>
## <a name="methods"></a><span data-ttu-id="47944-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="47944-105">Methods</span></span>
|<span data-ttu-id="47944-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="47944-106">Method</span></span>|<span data-ttu-id="47944-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="47944-107">Return Type</span></span>|<span data-ttu-id="47944-108">説明</span><span class="sxs-lookup"><span data-stu-id="47944-108">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="47944-109">managedAppRegistrations の一覧表示</span><span class="sxs-lookup"><span data-stu-id="47944-109">List managedAppRegistrations</span></span>](../api/intune_mam_managedappregistration_list.md)|<span data-ttu-id="47944-110">[managedAppRegistration](../resources/intune_mam_managedappregistration.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="47944-110">[managedAppRegistration](../resources/intune_mam_managedappregistration.md) collection</span></span>|<span data-ttu-id="47944-111">[managedAppRegistration](../resources/intune_mam_managedappregistration.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="47944-111">List properties and relationships of the [managedAppRegistration](../resources/intune_mam_managedappregistration.md) objects.</span></span>|
|[<span data-ttu-id="47944-112">managedAppRegistration の取得</span><span class="sxs-lookup"><span data-stu-id="47944-112">Get managedAppRegistration</span></span>](../api/intune_mam_managedappregistration_get.md)|[<span data-ttu-id="47944-113">managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="47944-113">managedAppRegistration</span></span>](../resources/intune_mam_managedappregistration.md)|<span data-ttu-id="47944-114">[managedAppRegistration](../resources/intune_mam_managedappregistration.md) オブジェクトのプロパティとリレーションを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="47944-114">Read properties and relationships of the [managedAppRegistration](../resources/intune_mam_managedappregistration.md) object.</span></span>|
|[<span data-ttu-id="47944-115">getUserIdsWithFlaggedAppRegistration 関数</span><span class="sxs-lookup"><span data-stu-id="47944-115">getUserIdsWithFlaggedAppRegistration function</span></span>](../api/intune_mam_managedappregistration_getuseridswithflaggedappregistration.md)|<span data-ttu-id="47944-116">String コレクション</span><span class="sxs-lookup"><span data-stu-id="47944-116">String collection</span></span>|<span data-ttu-id="47944-117">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="47944-117">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="47944-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="47944-118">Properties</span></span>
|<span data-ttu-id="47944-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="47944-119">Property</span></span>|<span data-ttu-id="47944-120">タイプ</span><span class="sxs-lookup"><span data-stu-id="47944-120">Type</span></span>|<span data-ttu-id="47944-121">説明</span><span class="sxs-lookup"><span data-stu-id="47944-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="47944-122">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="47944-122">createdDateTime</span></span>|<span data-ttu-id="47944-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="47944-123">DateTimeOffset</span></span>|<span data-ttu-id="47944-124">作成日時</span><span class="sxs-lookup"><span data-stu-id="47944-124">Date and time of creation</span></span>|
|<span data-ttu-id="47944-125">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="47944-125">lastSyncDateTime</span></span>|<span data-ttu-id="47944-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="47944-126">DateTimeOffset</span></span>|<span data-ttu-id="47944-127">アプリが管理サービスと最後に同期した日付と時刻。</span><span class="sxs-lookup"><span data-stu-id="47944-127">Date and time of last the app synced with management service.</span></span>|
|<span data-ttu-id="47944-128">applicationVersion</span><span class="sxs-lookup"><span data-stu-id="47944-128">applicationVersion</span></span>|<span data-ttu-id="47944-129">文字列</span><span class="sxs-lookup"><span data-stu-id="47944-129">String</span></span>|<span data-ttu-id="47944-130">アプリのバージョン</span><span class="sxs-lookup"><span data-stu-id="47944-130">App version</span></span>|
|<span data-ttu-id="47944-131">managementSdkVersion</span><span class="sxs-lookup"><span data-stu-id="47944-131">managementSdkVersion</span></span>|<span data-ttu-id="47944-132">文字列</span><span class="sxs-lookup"><span data-stu-id="47944-132">String</span></span>|<span data-ttu-id="47944-133">アプリ管理の SDK バージョン</span><span class="sxs-lookup"><span data-stu-id="47944-133">App management SDK version</span></span>|
|<span data-ttu-id="47944-134">platformVersion</span><span class="sxs-lookup"><span data-stu-id="47944-134">platformVersion</span></span>|<span data-ttu-id="47944-135">文字列</span><span class="sxs-lookup"><span data-stu-id="47944-135">String</span></span>|<span data-ttu-id="47944-136">オペレーティング システムのバージョン</span><span class="sxs-lookup"><span data-stu-id="47944-136">Operating System version</span></span>|
|<span data-ttu-id="47944-137">deviceType</span><span class="sxs-lookup"><span data-stu-id="47944-137">deviceType</span></span>|<span data-ttu-id="47944-138">文字列</span><span class="sxs-lookup"><span data-stu-id="47944-138">String</span></span>|<span data-ttu-id="47944-139">ホスト デバイスの種類</span><span class="sxs-lookup"><span data-stu-id="47944-139">Host device type</span></span>|
|<span data-ttu-id="47944-140">deviceTag</span><span class="sxs-lookup"><span data-stu-id="47944-140">deviceTag</span></span>|<span data-ttu-id="47944-141">文字列</span><span class="sxs-lookup"><span data-stu-id="47944-141">String</span></span>|<span data-ttu-id="47944-142">アプリ管理 SDK が生成したタグ。同じデバイスでホストされているアプリの関連付けに役立ちます。</span><span class="sxs-lookup"><span data-stu-id="47944-142">App management SDK generated tag, which helps relate apps hosted on the same device.</span></span> <span data-ttu-id="47944-143">あらゆる状況でのアプリの関連付けを保証するものではありません。</span><span class="sxs-lookup"><span data-stu-id="47944-143">Not guaranteed to relate apps in all conditions.</span></span>|
|<span data-ttu-id="47944-144">deviceName</span><span class="sxs-lookup"><span data-stu-id="47944-144">deviceName</span></span>|<span data-ttu-id="47944-145">文字列</span><span class="sxs-lookup"><span data-stu-id="47944-145">String</span></span>|<span data-ttu-id="47944-146">ホスト デバイスの名前</span><span class="sxs-lookup"><span data-stu-id="47944-146">Host device name</span></span>|
|<span data-ttu-id="47944-147">flaggedReasons</span><span class="sxs-lookup"><span data-stu-id="47944-147">flaggedReasons</span></span>|<span data-ttu-id="47944-148">[managedAppFlaggedReason 列挙型](../resources/intune_mam_managedappflaggedreason.md) のコレクション</span><span class="sxs-lookup"><span data-stu-id="47944-148">[managedAppFlaggedReason enum](../resources/intune_mam_managedappflaggedreason.md) collection</span></span>|<span data-ttu-id="47944-149">アプリ登録にフラグが設定された、0 個以上の理由。</span><span class="sxs-lookup"><span data-stu-id="47944-149">Zero or more reasons an app registration is flagged.</span></span> <span data-ttu-id="47944-150">例:</span><span class="sxs-lookup"><span data-stu-id="47944-150">E.g.</span></span> <span data-ttu-id="47944-151">ルートのデバイスで実行されているアプリ</span><span class="sxs-lookup"><span data-stu-id="47944-151">app running on rooted device</span></span>|
|<span data-ttu-id="47944-152">userId</span><span class="sxs-lookup"><span data-stu-id="47944-152">userId</span></span>|<span data-ttu-id="47944-153">文字列</span><span class="sxs-lookup"><span data-stu-id="47944-153">String</span></span>|<span data-ttu-id="47944-154">このアプリの登録が属するユーザー ID。</span><span class="sxs-lookup"><span data-stu-id="47944-154">The user Id to who this app registration belongs.</span></span>|
|<span data-ttu-id="47944-155">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="47944-155">appIdentifier</span></span>|[<span data-ttu-id="47944-156">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="47944-156">mobileAppIdentifier</span></span>](../resources/intune_mam_mobileappidentifier.md)|<span data-ttu-id="47944-157">アプリ パッケージの識別子</span><span class="sxs-lookup"><span data-stu-id="47944-157">The app package Identifier</span></span>|
|<span data-ttu-id="47944-158">ID</span><span class="sxs-lookup"><span data-stu-id="47944-158">id</span></span>|<span data-ttu-id="47944-159">文字列</span><span class="sxs-lookup"><span data-stu-id="47944-159">String</span></span>|<span data-ttu-id="47944-160">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="47944-160">Key of the entity.</span></span>|
|<span data-ttu-id="47944-161">バージョン</span><span class="sxs-lookup"><span data-stu-id="47944-161">version</span></span>|<span data-ttu-id="47944-162">文字列</span><span class="sxs-lookup"><span data-stu-id="47944-162">String</span></span>|<span data-ttu-id="47944-163">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="47944-163">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="47944-164">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="47944-164">Relationships</span></span>
|<span data-ttu-id="47944-165">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="47944-165">Relationship</span></span>|<span data-ttu-id="47944-166">型</span><span class="sxs-lookup"><span data-stu-id="47944-166">Type</span></span>|<span data-ttu-id="47944-167">説明</span><span class="sxs-lookup"><span data-stu-id="47944-167">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="47944-168">appliedPolicies</span><span class="sxs-lookup"><span data-stu-id="47944-168">appliedPolicies</span></span>|<span data-ttu-id="47944-169">[managedAppPolicy](../resources/intune_mam_managedapppolicy.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="47944-169">[managedAppPolicy](../resources/intune_mam_managedapppolicy.md) collection</span></span>|<span data-ttu-id="47944-170">登録済みのアプリが管理サービスと最後に同期したときに、既に適用されていた 0 個以上のポリシーです。</span><span class="sxs-lookup"><span data-stu-id="47944-170">Zero or more policys already applied on the registered app when it last synchronized with managment service.</span></span>|
|<span data-ttu-id="47944-171">intendedPolicies</span><span class="sxs-lookup"><span data-stu-id="47944-171">intendedPolicies</span></span>|<span data-ttu-id="47944-172">[managedAppPolicy](../resources/intune_mam_managedapppolicy.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="47944-172">[managedAppPolicy](../resources/intune_mam_managedapppolicy.md) collection</span></span>|<span data-ttu-id="47944-173">現時点で、管理者がアプリに対して意図した 0 個以上のポリシーです。</span><span class="sxs-lookup"><span data-stu-id="47944-173">Zero or more policies admin intended for the app as of now.</span></span>|
|<span data-ttu-id="47944-174">operations</span><span class="sxs-lookup"><span data-stu-id="47944-174">operations</span></span>|<span data-ttu-id="47944-175">[managedAppOperation](../resources/intune_mam_managedappoperation.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="47944-175">[managedAppOperation](../resources/intune_mam_managedappoperation.md) collection</span></span>|<span data-ttu-id="47944-176">アプリ登録でトリガーされた、0 個以上の長時間実行の操作です。</span><span class="sxs-lookup"><span data-stu-id="47944-176">Zero or more long running operations triggered on the app registration.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="47944-177">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="47944-177">JSON Representation</span></span>
<span data-ttu-id="47944-178">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="47944-178">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAppRegistration"
}-->
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








