# <a name="telecomexpensemanagementpartner-resource-type"></a><span data-ttu-id="b463d-101">telecomExpenseManagementPartner リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b463d-101">telecomExpenseManagementPartner resource type</span></span>

> <span data-ttu-id="b463d-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="b463d-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b463d-103">telecomExpenseManagementPartner リソースは、特定の TEM サービスのメタデータおよび状態を表します。</span><span class="sxs-lookup"><span data-stu-id="b463d-103">telecomExpenseManagementPartner resources represent the metadata and status of a given TEM service.</span></span> <span data-ttu-id="b463d-104">貴社がパートナーと協力関係を結ぶと、パートナーが TEM 機能をオンまたはオフに切り替える機能を有効または無効にできます。</span><span class="sxs-lookup"><span data-stu-id="b463d-104">Once your organization has onboarded with a partner, the partner can be enabled or disabled to switch TEM functionality on or off.</span></span>
## <a name="methods"></a><span data-ttu-id="b463d-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="b463d-105">Methods</span></span>
|<span data-ttu-id="b463d-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="b463d-106">Method</span></span>|<span data-ttu-id="b463d-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="b463d-107">Return Type</span></span>|<span data-ttu-id="b463d-108">説明</span><span class="sxs-lookup"><span data-stu-id="b463d-108">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="b463d-109">telecomExpenseManagementPartners のリスト</span><span class="sxs-lookup"><span data-stu-id="b463d-109">List telecomExpenseManagementPartners</span></span>](../api/intune_tem_telecomexpensemanagementpartner_list.md)|<span data-ttu-id="b463d-110">[telecomExpenseManagementPartner](../resources/intune_tem_telecomexpensemanagementpartner.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="b463d-110">[telecomExpenseManagementPartner](../resources/intune_tem_telecomexpensemanagementpartner.md) collection</span></span>|<span data-ttu-id="b463d-111">[telecomExpenseManagementPartner](../resources/intune_tem_telecomexpensemanagementpartner.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="b463d-111">List properties and relationships of the [telecomExpenseManagementPartner](../resources/intune_tem_telecomexpensemanagementpartner.md) objects.</span></span>|
|[<span data-ttu-id="b463d-112">telecomExpenseManagementPartner の取得</span><span class="sxs-lookup"><span data-stu-id="b463d-112">Get telecomExpenseManagementPartner</span></span>](../api/intune_tem_telecomexpensemanagementpartner_get.md)|[<span data-ttu-id="b463d-113">telecomExpenseManagementPartner</span><span class="sxs-lookup"><span data-stu-id="b463d-113">telecomExpenseManagementPartner</span></span>](../resources/intune_tem_telecomexpensemanagementpartner.md)|<span data-ttu-id="b463d-114">[telecomExpenseManagementPartner](../resources/intune_tem_telecomexpensemanagementpartner.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="b463d-114">Read properties and relationships of the [telecomExpenseManagementPartner](../resources/intune_tem_telecomexpensemanagementpartner.md) object.</span></span>|
|[<span data-ttu-id="b463d-115">telecomExpenseManagementPartner の作成</span><span class="sxs-lookup"><span data-stu-id="b463d-115">Create telecomExpenseManagementPartner</span></span>](../api/intune_tem_telecomexpensemanagementpartner_create.md)|[<span data-ttu-id="b463d-116">telecomExpenseManagementPartner</span><span class="sxs-lookup"><span data-stu-id="b463d-116">telecomExpenseManagementPartner</span></span>](../resources/intune_tem_telecomexpensemanagementpartner.md)|<span data-ttu-id="b463d-117">新しい [telecomExpenseManagementPartner](../resources/intune_tem_telecomexpensemanagementpartner.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="b463d-117">Create a new [telecomExpenseManagementPartner](../resources/intune_tem_telecomexpensemanagementpartner.md) object.</span></span>|
|[<span data-ttu-id="b463d-118">telecomExpenseManagementPartner の削除</span><span class="sxs-lookup"><span data-stu-id="b463d-118">Delete telecomExpenseManagementPartner</span></span>](../api/intune_tem_telecomexpensemanagementpartner_delete.md)|<span data-ttu-id="b463d-119">なし</span><span class="sxs-lookup"><span data-stu-id="b463d-119">None</span></span>|<span data-ttu-id="b463d-120">[telecomExpenseManagementPartner](../resources/intune_tem_telecomexpensemanagementpartner.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="b463d-120">Deletes a [telecomExpenseManagementPartner](../resources/intune_tem_telecomexpensemanagementpartner.md).</span></span>|
|[<span data-ttu-id="b463d-121">telecomExpenseManagementPartner の更新</span><span class="sxs-lookup"><span data-stu-id="b463d-121">Update telecomExpenseManagementPartner</span></span>](../api/intune_tem_telecomexpensemanagementpartner_update.md)|[<span data-ttu-id="b463d-122">telecomExpenseManagementPartner</span><span class="sxs-lookup"><span data-stu-id="b463d-122">telecomExpenseManagementPartner</span></span>](../resources/intune_tem_telecomexpensemanagementpartner.md)|<span data-ttu-id="b463d-123">[telecomExpenseManagementPartner](../resources/intune_tem_telecomexpensemanagementpartner.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="b463d-123">Update the properties of a [telecomExpenseManagementPartner](../resources/intune_tem_telecomexpensemanagementpartner.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="b463d-124">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b463d-124">Properties</span></span>
|<span data-ttu-id="b463d-125">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b463d-125">Property</span></span>|<span data-ttu-id="b463d-126">タイプ</span><span class="sxs-lookup"><span data-stu-id="b463d-126">Type</span></span>|<span data-ttu-id="b463d-127">説明</span><span class="sxs-lookup"><span data-stu-id="b463d-127">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b463d-128">ID</span><span class="sxs-lookup"><span data-stu-id="b463d-128">id</span></span>|<span data-ttu-id="b463d-129">文字列</span><span class="sxs-lookup"><span data-stu-id="b463d-129">String</span></span>|<span data-ttu-id="b463d-130">TEM パートナーの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="b463d-130">Unique identifier of the TEM partner.</span></span>|
|<span data-ttu-id="b463d-131">displayName</span><span class="sxs-lookup"><span data-stu-id="b463d-131">displayName</span></span>|<span data-ttu-id="b463d-132">文字列</span><span class="sxs-lookup"><span data-stu-id="b463d-132">String</span></span>|<span data-ttu-id="b463d-133">TEM パートナーの表示名。</span><span class="sxs-lookup"><span data-stu-id="b463d-133">Display name of the TEM partner.</span></span>|
|<span data-ttu-id="b463d-134">url</span><span class="sxs-lookup"><span data-stu-id="b463d-134">url</span></span>|<span data-ttu-id="b463d-135">文字列</span><span class="sxs-lookup"><span data-stu-id="b463d-135">String</span></span>|<span data-ttu-id="b463d-136">TEM パートナーの管理用コントロール パネルの URL。管理者はここで TEM サービスを構成できます。</span><span class="sxs-lookup"><span data-stu-id="b463d-136">URL of the TEM partner's administrative control panel, where an administrator can configure their TEM service.</span></span>|
|<span data-ttu-id="b463d-137">appAuthorized</span><span class="sxs-lookup"><span data-stu-id="b463d-137">appAuthorized</span></span>|<span data-ttu-id="b463d-138">ブール値</span><span class="sxs-lookup"><span data-stu-id="b463d-138">Boolean</span></span>|<span data-ttu-id="b463d-139">パートナーの AAD アプリに Intune へのアクセスが承認されているかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="b463d-139">Whether the partner's AAD app has been authorized to access Intune.</span></span>|
|<span data-ttu-id="b463d-140">有効化済み</span><span class="sxs-lookup"><span data-stu-id="b463d-140">enabled</span></span>|<span data-ttu-id="b463d-141">ブール値</span><span class="sxs-lookup"><span data-stu-id="b463d-141">Boolean</span></span>|<span data-ttu-id="b463d-142">TEM サービスへの Intune の接続が現在有効であるか、無効であるかを指定します。</span><span class="sxs-lookup"><span data-stu-id="b463d-142">Whether Intune's connection to the TEM service is currently enabled or disabled.</span></span>|
|<span data-ttu-id="b463d-143">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="b463d-143">lastConnectionDateTime</span></span>|<span data-ttu-id="b463d-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b463d-144">DateTimeOffset</span></span>|<span data-ttu-id="b463d-145">TEM パートナーによって Intune に対して最後に送信された要求のタイムスタンプ。</span><span class="sxs-lookup"><span data-stu-id="b463d-145">Timestamp of the last request sent to Intune by the TEM partner.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b463d-146">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b463d-146">Relationships</span></span>
<span data-ttu-id="b463d-147">なし</span><span class="sxs-lookup"><span data-stu-id="b463d-147">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b463d-148">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b463d-148">JSON Representation</span></span>
<span data-ttu-id="b463d-149">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="b463d-149">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.telecomExpenseManagementPartner"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.telecomExpenseManagementPartner",
  "id": "String (identifier)",
  "displayName": "String",
  "url": "String",
  "appAuthorized": true,
  "enabled": true,
  "lastConnectionDateTime": "String (timestamp)"
}
```








