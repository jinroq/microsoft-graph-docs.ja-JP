# <a name="onpremisesconditionalaccesssettings-resource-type"></a><span data-ttu-id="ac84f-101">onPremisesConditionalAccessSettings リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ac84f-101">onPremisesConditionalAccessSettings resource type</span></span>

> <span data-ttu-id="ac84f-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="ac84f-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ac84f-103">テナントの Exchange OnPremises 条件付きアクセス設定を表す単一エンティティ。</span><span class="sxs-lookup"><span data-stu-id="ac84f-103">Singleton entity which represents the Exchange OnPremises Conditional Access Settings for a tenant.</span></span>
## <a name="methods"></a><span data-ttu-id="ac84f-104">メソッド</span><span class="sxs-lookup"><span data-stu-id="ac84f-104">Methods</span></span>
|<span data-ttu-id="ac84f-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="ac84f-105">Method</span></span>|<span data-ttu-id="ac84f-106">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="ac84f-106">Return Type</span></span>|<span data-ttu-id="ac84f-107">説明</span><span class="sxs-lookup"><span data-stu-id="ac84f-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ac84f-108">Get onPremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="ac84f-108">Get onPremisesConditionalAccessSettings</span></span>](../api/intune_onboarding_onpremisesconditionalaccesssettings_get.md)|[<span data-ttu-id="ac84f-109">onPremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="ac84f-109">onPremisesConditionalAccessSettings</span></span>](../resources/intune_onboarding_onpremisesconditionalaccesssettings.md)|<span data-ttu-id="ac84f-110">[onPremisesConditionalAccessSettings](../resources/intune_onboarding_onpremisesconditionalaccesssettings.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="ac84f-110">Read properties and relationships of the [onPremisesConditionalAccessSettings](../resources/intune_onboarding_onpremisesconditionalaccesssettings.md) object.</span></span>|
|[<span data-ttu-id="ac84f-111">Update onPremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="ac84f-111">Update onPremisesConditionalAccessSettings</span></span>](../api/intune_onboarding_onpremisesconditionalaccesssettings_update.md)|[<span data-ttu-id="ac84f-112">onPremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="ac84f-112">onPremisesConditionalAccessSettings</span></span>](../resources/intune_onboarding_onpremisesconditionalaccesssettings.md)|<span data-ttu-id="ac84f-113">[onPremisesConditionalAccessSettings](../resources/intune_onboarding_onpremisesconditionalaccesssettings.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="ac84f-113">Update the properties of a [onPremisesConditionalAccessSettings](../resources/intune_onboarding_onpremisesconditionalaccesssettings.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="ac84f-114">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ac84f-114">Properties</span></span>
|<span data-ttu-id="ac84f-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ac84f-115">Property</span></span>|<span data-ttu-id="ac84f-116">型</span><span class="sxs-lookup"><span data-stu-id="ac84f-116">Type</span></span>|<span data-ttu-id="ac84f-117">説明</span><span class="sxs-lookup"><span data-stu-id="ac84f-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ac84f-118">id</span><span class="sxs-lookup"><span data-stu-id="ac84f-118">id</span></span>|<span data-ttu-id="ac84f-119">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="ac84f-119">String</span></span>|<span data-ttu-id="ac84f-120">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="ac84f-120">Not yet documented</span></span>|
|<span data-ttu-id="ac84f-121">enabled</span><span class="sxs-lookup"><span data-stu-id="ac84f-121">enabled</span></span>|<span data-ttu-id="ac84f-122">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="ac84f-122">Boolean</span></span>|<span data-ttu-id="ac84f-123">対象組織で、オンプレミスの条件付きアクセスが有効かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ac84f-123">Indicates if on premises conditional access is enabled for this organization</span></span>|
|<span data-ttu-id="ac84f-124">includedGroups</span><span class="sxs-lookup"><span data-stu-id="ac84f-124">includedGroups</span></span>|<span data-ttu-id="ac84f-125">Guid コレクション</span><span class="sxs-lookup"><span data-stu-id="ac84f-125">Guid collection</span></span>|<span data-ttu-id="ac84f-126">オンプレミスの条件付きアクセスで対象となるユーザー グループ。</span><span class="sxs-lookup"><span data-stu-id="ac84f-126">User groups that will be targeted by on premises conditional access.</span></span> <span data-ttu-id="ac84f-127">これらのグループ内のユーザーすべては、管理対象のモバイル デバイスを持っており、メール アクセスに準拠している必要があります。</span><span class="sxs-lookup"><span data-stu-id="ac84f-127">All users in these groups will be required to have mobile device managed and compliant for mail access.</span></span>|
|<span data-ttu-id="ac84f-128">excludedGroups</span><span class="sxs-lookup"><span data-stu-id="ac84f-128">excludedGroups</span></span>|<span data-ttu-id="ac84f-129">Guid コレクション</span><span class="sxs-lookup"><span data-stu-id="ac84f-129">Guid collection</span></span>|<span data-ttu-id="ac84f-130">オンプレミスの条件付きアクセスで除外されるユーザー グループ。</span><span class="sxs-lookup"><span data-stu-id="ac84f-130">User groups that will be exempt by on premises conditional access.</span></span> <span data-ttu-id="ac84f-131">これらのグループ内のすべてのユーザーは、条件付きアクセス ポリシーから除外されます。</span><span class="sxs-lookup"><span data-stu-id="ac84f-131">All users in these groups will be exempt from the conditional access policy.</span></span>|
|<span data-ttu-id="ac84f-132">overrideDefaultRule</span><span class="sxs-lookup"><span data-stu-id="ac84f-132">overrideDefaultRule</span></span>|<span data-ttu-id="ac84f-133">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="ac84f-133">Boolean</span></span>|<span data-ttu-id="ac84f-134">デバイスでアクセスが付与されていることを確認できるようにするとき、既定のアクセス ルールを上書きします。</span><span class="sxs-lookup"><span data-stu-id="ac84f-134">Override the default access rule when allowing a device to ensure access is granted.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ac84f-135">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ac84f-135">Relationships</span></span>
<span data-ttu-id="ac84f-136">なし</span><span class="sxs-lookup"><span data-stu-id="ac84f-136">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="ac84f-137">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ac84f-137">JSON Representation</span></span>
<span data-ttu-id="ac84f-138">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="ac84f-138">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.onPremisesConditionalAccessSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.onPremisesConditionalAccessSettings",
  "id": "String (identifier)",
  "enabled": true,
  "includedGroups": [
    "Guid"
  ],
  "excludedGroups": [
    "Guid"
  ],
  "overrideDefaultRule": true
}
```



