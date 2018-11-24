# <a name="managedappstatus-resource-type"></a><span data-ttu-id="309ed-101">managedAppStatus リソースの種類</span><span class="sxs-lookup"><span data-stu-id="309ed-101">managedAppStatus resource type</span></span>

> <span data-ttu-id="309ed-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="309ed-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="309ed-103">組織のアプリ保護と構成の状態を表します。</span><span class="sxs-lookup"><span data-stu-id="309ed-103">Represents app protection and configuration status for the organization.</span></span>
## <a name="methods"></a><span data-ttu-id="309ed-104">メソッド</span><span class="sxs-lookup"><span data-stu-id="309ed-104">Methods</span></span>
|<span data-ttu-id="309ed-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="309ed-105">Method</span></span>|<span data-ttu-id="309ed-106">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="309ed-106">Return Type</span></span>|<span data-ttu-id="309ed-107">説明</span><span class="sxs-lookup"><span data-stu-id="309ed-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="309ed-108">List managedAppStatuses</span><span class="sxs-lookup"><span data-stu-id="309ed-108">List managedAppStatuses</span></span>](../api/intune_mam_managedappstatus_list.md)|<span data-ttu-id="309ed-109">[managedAppStatus](../resources/intune_mam_managedappstatus.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="309ed-109">[managedAppStatus](../resources/intune_mam_managedappstatus.md) collection</span></span>|<span data-ttu-id="309ed-110">[managedAppStatus](../resources/intune_mam_managedappstatus.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="309ed-110">List properties and relationships of the [managedAppStatus](../resources/intune_mam_managedappstatus.md) objects.</span></span>|
|[<span data-ttu-id="309ed-111">Get managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="309ed-111">Get managedAppStatus</span></span>](../api/intune_mam_managedappstatus_get.md)|[<span data-ttu-id="309ed-112">managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="309ed-112">managedAppStatus</span></span>](../resources/intune_mam_managedappstatus.md)|<span data-ttu-id="309ed-113">[managedAppStatus](../resources/intune_mam_managedappstatus.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="309ed-113">Read properties and relationships of the [managedAppStatus](../resources/intune_mam_managedappstatus.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="309ed-114">プロパティ</span><span class="sxs-lookup"><span data-stu-id="309ed-114">Properties</span></span>
|<span data-ttu-id="309ed-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="309ed-115">Property</span></span>|<span data-ttu-id="309ed-116">型</span><span class="sxs-lookup"><span data-stu-id="309ed-116">Type</span></span>|<span data-ttu-id="309ed-117">説明</span><span class="sxs-lookup"><span data-stu-id="309ed-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="309ed-118">displayName</span><span class="sxs-lookup"><span data-stu-id="309ed-118">displayName</span></span>|<span data-ttu-id="309ed-119">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="309ed-119">String</span></span>|<span data-ttu-id="309ed-120">進捗レポートのフレンドリ名。</span><span class="sxs-lookup"><span data-stu-id="309ed-120">Friendly name of the status report.</span></span>|
|<span data-ttu-id="309ed-121">id</span><span class="sxs-lookup"><span data-stu-id="309ed-121">id</span></span>|<span data-ttu-id="309ed-122">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="309ed-122">String</span></span>|<span data-ttu-id="309ed-123">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="309ed-123">Key of the entity.</span></span>|
|<span data-ttu-id="309ed-124">version</span><span class="sxs-lookup"><span data-stu-id="309ed-124">version</span></span>|<span data-ttu-id="309ed-125">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="309ed-125">String</span></span>|<span data-ttu-id="309ed-126">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="309ed-126">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="309ed-127">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="309ed-127">Relationships</span></span>
<span data-ttu-id="309ed-128">なし</span><span class="sxs-lookup"><span data-stu-id="309ed-128">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="309ed-129">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="309ed-129">JSON Representation</span></span>
<span data-ttu-id="309ed-130">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="309ed-130">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAppStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppStatus",
  "displayName": "String",
  "id": "String (identifier)",
  "version": "String"
}
```



