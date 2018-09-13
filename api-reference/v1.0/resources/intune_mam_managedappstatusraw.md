# <a name="managedappstatusraw-resource-type"></a><span data-ttu-id="89af2-101">managedAppStatusRaw リソースの種類</span><span class="sxs-lookup"><span data-stu-id="89af2-101">managedAppStatusRaw resource type</span></span>

> <span data-ttu-id="89af2-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="89af2-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="89af2-103">組織アプリの保護と構成についての型指定されていない進捗レポートを表します。</span><span class="sxs-lookup"><span data-stu-id="89af2-103">Represents an un-typed status report about organizations app protection and configuration.</span></span>

<span data-ttu-id="89af2-104">[managedAppStatus](../resources/intune_mam_managedappstatus.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="89af2-104">Inherits from [managedAppStatus](../resources/intune_mam_managedappstatus.md)</span></span>

## <a name="methods"></a><span data-ttu-id="89af2-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="89af2-105">Methods</span></span>
|<span data-ttu-id="89af2-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="89af2-106">Method</span></span>|<span data-ttu-id="89af2-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="89af2-107">Return Type</span></span>|<span data-ttu-id="89af2-108">説明</span><span class="sxs-lookup"><span data-stu-id="89af2-108">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="89af2-109">managedAppStatusRaws のリスト</span><span class="sxs-lookup"><span data-stu-id="89af2-109">List managedAppStatusRaws</span></span>](../api/intune_mam_managedappstatusraw_list.md)|<span data-ttu-id="89af2-110">[managedAppStatusRaw](../resources/intune_mam_managedappstatusraw.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="89af2-110">[managedAppStatusRaw](../resources/intune_mam_managedappstatusraw.md) collection</span></span>|<span data-ttu-id="89af2-111">[managedAppStatusRaw](../resources/intune_mam_managedappstatusraw.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="89af2-111">List properties and relationships of the [managedAppStatusRaw](../resources/intune_mam_managedappstatusraw.md) objects.</span></span>|
|[<span data-ttu-id="89af2-112">managedAppStatusRaw の取得</span><span class="sxs-lookup"><span data-stu-id="89af2-112">Get managedAppStatusRaw</span></span>](../api/intune_mam_managedappstatusraw_get.md)|[<span data-ttu-id="89af2-113">managedAppStatusRaw</span><span class="sxs-lookup"><span data-stu-id="89af2-113">managedAppStatusRaw</span></span>](../resources/intune_mam_managedappstatusraw.md)|<span data-ttu-id="89af2-114">[managedAppStatusRaw](../resources/intune_mam_managedappstatusraw.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="89af2-114">Read properties and relationships of the [managedAppStatusRaw](../resources/intune_mam_managedappstatusraw.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="89af2-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="89af2-115">Properties</span></span>
|<span data-ttu-id="89af2-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="89af2-116">Property</span></span>|<span data-ttu-id="89af2-117">タイプ</span><span class="sxs-lookup"><span data-stu-id="89af2-117">Type</span></span>|<span data-ttu-id="89af2-118">説明</span><span class="sxs-lookup"><span data-stu-id="89af2-118">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="89af2-119">displayName</span><span class="sxs-lookup"><span data-stu-id="89af2-119">displayName</span></span>|<span data-ttu-id="89af2-120">文字列</span><span class="sxs-lookup"><span data-stu-id="89af2-120">String</span></span>|<span data-ttu-id="89af2-121">進捗レポートのフレンドリ名。</span><span class="sxs-lookup"><span data-stu-id="89af2-121">Friendly name of the status report.</span></span> <span data-ttu-id="89af2-122">[managedAppStatus](../resources/intune_mam_managedappstatus.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="89af2-122">Inherited from [managedAppStatus](../resources/intune_mam_managedappstatus.md)</span></span>|
|<span data-ttu-id="89af2-123">ID</span><span class="sxs-lookup"><span data-stu-id="89af2-123">id</span></span>|<span data-ttu-id="89af2-124">文字列</span><span class="sxs-lookup"><span data-stu-id="89af2-124">String</span></span>|<span data-ttu-id="89af2-125">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="89af2-125">Key of the entity.</span></span> <span data-ttu-id="89af2-126">[managedAppStatus](../resources/intune_mam_managedappstatus.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="89af2-126">Inherited from [managedAppStatus](../resources/intune_mam_managedappstatus.md)</span></span>|
|<span data-ttu-id="89af2-127">バージョン</span><span class="sxs-lookup"><span data-stu-id="89af2-127">version</span></span>|<span data-ttu-id="89af2-128">文字列</span><span class="sxs-lookup"><span data-stu-id="89af2-128">String</span></span>|<span data-ttu-id="89af2-129">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="89af2-129">Version of the entity.</span></span> <span data-ttu-id="89af2-130">[managedAppStatus](../resources/intune_mam_managedappstatus.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="89af2-130">Inherited from [managedAppStatus](../resources/intune_mam_managedappstatus.md)</span></span>|
|<span data-ttu-id="89af2-131">コンテンツ</span><span class="sxs-lookup"><span data-stu-id="89af2-131">content</span></span>|[<span data-ttu-id="89af2-132">Json</span><span class="sxs-lookup"><span data-stu-id="89af2-132">Json</span></span>](../resources/json.md)|<span data-ttu-id="89af2-133">進捗レポートの内容。</span><span class="sxs-lookup"><span data-stu-id="89af2-133">Status report content.</span></span>|

## <a name="relationships"></a><span data-ttu-id="89af2-134">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="89af2-134">Relationships</span></span>
<span data-ttu-id="89af2-135">なし</span><span class="sxs-lookup"><span data-stu-id="89af2-135">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="89af2-136">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="89af2-136">JSON Representation</span></span>
<span data-ttu-id="89af2-137">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="89af2-137">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.managedAppStatus",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAppStatusRaw"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppStatusRaw",
  "displayName": "String",
  "id": "String (identifier)",
  "version": "String",
  "content": {
    "@odata.type": "microsoft.graph.Json"
  }
}
```








