# <a name="remoteassistancepartner-resource-type"></a><span data-ttu-id="05ddb-101">remoteAssistancePartner リソースの種類</span><span class="sxs-lookup"><span data-stu-id="05ddb-101">remoteAssistancePartner resource type</span></span>

> <span data-ttu-id="05ddb-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="05ddb-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="05ddb-103">remoteAssistPartner リソースは、特定のリモート アシスタンス パートナー サービスのメタデータおよび状態を表します。</span><span class="sxs-lookup"><span data-stu-id="05ddb-103">remoteAssistPartner resources represent the metadata and status of a given Remote Assistance partner service.</span></span>
## <a name="methods"></a><span data-ttu-id="05ddb-104">メソッド</span><span class="sxs-lookup"><span data-stu-id="05ddb-104">Methods</span></span>
|<span data-ttu-id="05ddb-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="05ddb-105">Method</span></span>|<span data-ttu-id="05ddb-106">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="05ddb-106">Return Type</span></span>|<span data-ttu-id="05ddb-107">説明</span><span class="sxs-lookup"><span data-stu-id="05ddb-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="05ddb-108">remoteAssistancePartners をリストします</span><span class="sxs-lookup"><span data-stu-id="05ddb-108">List remoteAssistancePartners</span></span>](../api/intune_remoteassistance_remoteassistancepartner_list.md)|<span data-ttu-id="05ddb-109">[remoteAssistancePartner](../resources/intune_remoteassistance_remoteassistancepartner.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="05ddb-109">[remoteAssistancePartner](../resources/intune_remoteassistance_remoteassistancepartner.md) collection</span></span>|<span data-ttu-id="05ddb-110">[remoteAssistancePartner](../resources/intune_remoteassistance_remoteassistancepartner.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="05ddb-110">List properties and relationships of the [remoteAssistancePartner](../resources/intune_remoteassistance_remoteassistancepartner.md) objects.</span></span>|
|[<span data-ttu-id="05ddb-111">remoteAssistancePartner を取得します</span><span class="sxs-lookup"><span data-stu-id="05ddb-111">Get remoteAssistancePartner</span></span>](../api/intune_remoteassistance_remoteassistancepartner_get.md)|[<span data-ttu-id="05ddb-112">remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="05ddb-112">remoteAssistancePartner</span></span>](../resources/intune_remoteassistance_remoteassistancepartner.md)|<span data-ttu-id="05ddb-113">[remoteAssistancePartner](../resources/intune_remoteassistance_remoteassistancepartner.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="05ddb-113">Read properties and relationships of the [remoteAssistancePartner](../resources/intune_remoteassistance_remoteassistancepartner.md) object.</span></span>|
|[<span data-ttu-id="05ddb-114">remoteAssistancePartner を作成します</span><span class="sxs-lookup"><span data-stu-id="05ddb-114">Create remoteAssistancePartner</span></span>](../api/intune_remoteassistance_remoteassistancepartner_create.md)|[<span data-ttu-id="05ddb-115">remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="05ddb-115">remoteAssistancePartner</span></span>](../resources/intune_remoteassistance_remoteassistancepartner.md)|<span data-ttu-id="05ddb-116">新しい [remoteAssistancePartner](../resources/intune_remoteassistance_remoteassistancepartner.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="05ddb-116">Create a new [remoteAssistancePartner](../resources/intune_remoteassistance_remoteassistancepartner.md) object.</span></span>|
|[<span data-ttu-id="05ddb-117">remoteAssistancePartner を削除します</span><span class="sxs-lookup"><span data-stu-id="05ddb-117">Delete remoteAssistancePartner</span></span>](../api/intune_remoteassistance_remoteassistancepartner_delete.md)|<span data-ttu-id="05ddb-118">なし</span><span class="sxs-lookup"><span data-stu-id="05ddb-118">None</span></span>|<span data-ttu-id="05ddb-119">[remoteAssistancePartner](../resources/intune_remoteassistance_remoteassistancepartner.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="05ddb-119">Deletes a [remoteAssistancePartner](../resources/intune_remoteassistance_remoteassistancepartner.md).</span></span>|
|[<span data-ttu-id="05ddb-120">remoteAssistancePartner を更新します</span><span class="sxs-lookup"><span data-stu-id="05ddb-120">Update remoteAssistancePartner</span></span>](../api/intune_remoteassistance_remoteassistancepartner_update.md)|[<span data-ttu-id="05ddb-121">remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="05ddb-121">remoteAssistancePartner</span></span>](../resources/intune_remoteassistance_remoteassistancepartner.md)|<span data-ttu-id="05ddb-122">[remoteAssistancePartner](../resources/intune_remoteassistance_remoteassistancepartner.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="05ddb-122">Update the properties of a [remoteAssistancePartner](../resources/intune_remoteassistance_remoteassistancepartner.md) object.</span></span>|
|[<span data-ttu-id="05ddb-123">beginOnboarding アクション</span><span class="sxs-lookup"><span data-stu-id="05ddb-123">beginOnboarding action</span></span>](../api/intune_remoteassistance_remoteassistancepartner_beginonboarding.md)|<span data-ttu-id="05ddb-124">なし</span><span class="sxs-lookup"><span data-stu-id="05ddb-124">None</span></span>|<span data-ttu-id="05ddb-125">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="05ddb-125">Not yet documented</span></span>|
|[<span data-ttu-id="05ddb-126">disconnect アクション</span><span class="sxs-lookup"><span data-stu-id="05ddb-126">disconnect action</span></span>](../api/intune_remoteassistance_remoteassistancepartner_disconnect.md)|<span data-ttu-id="05ddb-127">なし</span><span class="sxs-lookup"><span data-stu-id="05ddb-127">None</span></span>|<span data-ttu-id="05ddb-128">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="05ddb-128">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="05ddb-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="05ddb-129">Properties</span></span>
|<span data-ttu-id="05ddb-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="05ddb-130">Property</span></span>|<span data-ttu-id="05ddb-131">タイプ</span><span class="sxs-lookup"><span data-stu-id="05ddb-131">Type</span></span>|<span data-ttu-id="05ddb-132">説明</span><span class="sxs-lookup"><span data-stu-id="05ddb-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="05ddb-133">ID</span><span class="sxs-lookup"><span data-stu-id="05ddb-133">id</span></span>|<span data-ttu-id="05ddb-134">文字列</span><span class="sxs-lookup"><span data-stu-id="05ddb-134">String</span></span>|<span data-ttu-id="05ddb-135">パートナーの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="05ddb-135">Unique identifier of the partner.</span></span>|
|<span data-ttu-id="05ddb-136">displayName</span><span class="sxs-lookup"><span data-stu-id="05ddb-136">displayName</span></span>|<span data-ttu-id="05ddb-137">文字列</span><span class="sxs-lookup"><span data-stu-id="05ddb-137">String</span></span>|<span data-ttu-id="05ddb-138">パートナーの表示名。</span><span class="sxs-lookup"><span data-stu-id="05ddb-138">Display name of the partner.</span></span>|
|<span data-ttu-id="05ddb-139">onboardingUrl</span><span class="sxs-lookup"><span data-stu-id="05ddb-139">onboardingUrl</span></span>|<span data-ttu-id="05ddb-140">文字列</span><span class="sxs-lookup"><span data-stu-id="05ddb-140">String</span></span>|<span data-ttu-id="05ddb-141">パートナーのオンボーディング ポータルの URL。このポータルでは、管理者がパートナーのリモート アシスタンス サービスを構成できます。</span><span class="sxs-lookup"><span data-stu-id="05ddb-141">URL of the partner's onboarding portal, where an administrator can configure their Remote Assistance service.</span></span>|
|<span data-ttu-id="05ddb-142">onboardingStatus</span><span class="sxs-lookup"><span data-stu-id="05ddb-142">onboardingStatus</span></span>|[<span data-ttu-id="05ddb-143">remoteAssistanceOnboardingStatus</span><span class="sxs-lookup"><span data-stu-id="05ddb-143">remoteAssistanceOnboardingStatus</span></span>](../resources/intune_remoteassistance_remoteassistanceonboardingstatus.md)|<span data-ttu-id="05ddb-p101">TBD。使用可能な値は`notOnboarded`、`onboarding`、`onboarded` です。</span><span class="sxs-lookup"><span data-stu-id="05ddb-p101">TBD Possible values are: `notOnboarded`, `onboarding`, `onboarded`.</span></span>|
|<span data-ttu-id="05ddb-146">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="05ddb-146">lastConnectionDateTime</span></span>|<span data-ttu-id="05ddb-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="05ddb-147">DateTimeOffset</span></span>|<span data-ttu-id="05ddb-148">TEM パートナーによって Intune に対して最後に送信された要求のタイムスタンプ。</span><span class="sxs-lookup"><span data-stu-id="05ddb-148">Timestamp of the last request sent to Intune by the TEM partner.</span></span>|

## <a name="relationships"></a><span data-ttu-id="05ddb-149">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="05ddb-149">Relationships</span></span>
<span data-ttu-id="05ddb-150">なし</span><span class="sxs-lookup"><span data-stu-id="05ddb-150">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="05ddb-151">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="05ddb-151">JSON Representation</span></span>
<span data-ttu-id="05ddb-152">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="05ddb-152">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.remoteAssistancePartner"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.remoteAssistancePartner",
  "id": "String (identifier)",
  "displayName": "String",
  "onboardingUrl": "String",
  "onboardingStatus": "String",
  "lastConnectionDateTime": "String (timestamp)"
}
```








