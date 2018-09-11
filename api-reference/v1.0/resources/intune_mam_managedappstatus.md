# <a name="managedappstatus-resource-type"></a><span data-ttu-id="2fb4a-101">managedAppStatus リソースの種類</span><span class="sxs-lookup"><span data-stu-id="2fb4a-101">managedAppStatus resource type</span></span>

> <span data-ttu-id="2fb4a-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="2fb4a-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2fb4a-103">組織のアプリ保護と構成の状態を表します。</span><span class="sxs-lookup"><span data-stu-id="2fb4a-103">Represents app protection and configuration status for the organization.</span></span>
## <a name="methods"></a><span data-ttu-id="2fb4a-104">メソッド</span><span class="sxs-lookup"><span data-stu-id="2fb4a-104">Methods</span></span>
|<span data-ttu-id="2fb4a-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="2fb4a-105">Method</span></span>|<span data-ttu-id="2fb4a-106">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="2fb4a-106">Return Type</span></span>|<span data-ttu-id="2fb4a-107">説明</span><span class="sxs-lookup"><span data-stu-id="2fb4a-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="2fb4a-108">managedAppStatuses のリスト</span><span class="sxs-lookup"><span data-stu-id="2fb4a-108">List managedAppStatuses</span></span>](../api/intune_mam_managedappstatus_list.md)|<span data-ttu-id="2fb4a-109">[managedAppStatus](../resources/intune_mam_managedappstatus.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="2fb4a-109">[managedAppStatus](../resources/intune_mam_managedappstatus.md) collection</span></span>|<span data-ttu-id="2fb4a-110">[managedAppStatus](../resources/intune_mam_managedappstatus.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="2fb4a-110">List properties and relationships of the [managedAppStatus](../resources/intune_mam_managedappstatus.md) objects.</span></span>|
|[<span data-ttu-id="2fb4a-111">managedAppStatus の取得</span><span class="sxs-lookup"><span data-stu-id="2fb4a-111">Get managedAppStatus</span></span>](../api/intune_mam_managedappstatus_get.md)|[<span data-ttu-id="2fb4a-112">managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="2fb4a-112">managedAppStatus</span></span>](../resources/intune_mam_managedappstatus.md)|<span data-ttu-id="2fb4a-113">[managedAppStatus](../resources/intune_mam_managedappstatus.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="2fb4a-113">Read properties and relationships of the [managedAppStatus](../resources/intune_mam_managedappstatus.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="2fb4a-114">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2fb4a-114">Properties</span></span>
|<span data-ttu-id="2fb4a-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2fb4a-115">Property</span></span>|<span data-ttu-id="2fb4a-116">タイプ</span><span class="sxs-lookup"><span data-stu-id="2fb4a-116">Type</span></span>|<span data-ttu-id="2fb4a-117">説明</span><span class="sxs-lookup"><span data-stu-id="2fb4a-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2fb4a-118">displayName</span><span class="sxs-lookup"><span data-stu-id="2fb4a-118">displayName</span></span>|<span data-ttu-id="2fb4a-119">文字列</span><span class="sxs-lookup"><span data-stu-id="2fb4a-119">String</span></span>|<span data-ttu-id="2fb4a-120">進捗レポートのフレンドリ名。</span><span class="sxs-lookup"><span data-stu-id="2fb4a-120">Friendly name of the status report.</span></span>|
|<span data-ttu-id="2fb4a-121">id</span><span class="sxs-lookup"><span data-stu-id="2fb4a-121">id</span></span>|<span data-ttu-id="2fb4a-122">文字列</span><span class="sxs-lookup"><span data-stu-id="2fb4a-122">String</span></span>|<span data-ttu-id="2fb4a-123">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="2fb4a-123">Key of the entity.</span></span>|
|<span data-ttu-id="2fb4a-124">バージョン</span><span class="sxs-lookup"><span data-stu-id="2fb4a-124">version</span></span>|<span data-ttu-id="2fb4a-125">文字列</span><span class="sxs-lookup"><span data-stu-id="2fb4a-125">String</span></span>|<span data-ttu-id="2fb4a-126">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="2fb4a-126">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2fb4a-127">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="2fb4a-127">Relationships</span></span>
<span data-ttu-id="2fb4a-128">なし</span><span class="sxs-lookup"><span data-stu-id="2fb4a-128">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="2fb4a-129">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2fb4a-129">JSON Representation</span></span>
<span data-ttu-id="2fb4a-130">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="2fb4a-130">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAppStatus"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppStatus",
  "displayName": "String",
  "id": "String (identifier)",
  "version": "String"
}
```








