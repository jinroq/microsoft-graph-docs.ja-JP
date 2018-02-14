# <a name="managedappoperation-resource-type"></a><span data-ttu-id="fe985-101">managedAppOperation リソースの種類</span><span class="sxs-lookup"><span data-stu-id="fe985-101">managedAppOperation resource type</span></span>

> <span data-ttu-id="fe985-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="fe985-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fe985-103">アプリ登録に対して適用される操作を表します。</span><span class="sxs-lookup"><span data-stu-id="fe985-103">Represents an operation applied against an app registration.</span></span>
## <a name="methods"></a><span data-ttu-id="fe985-104">メソッド</span><span class="sxs-lookup"><span data-stu-id="fe985-104">Methods</span></span>
|<span data-ttu-id="fe985-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="fe985-105">Method</span></span>|<span data-ttu-id="fe985-106">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="fe985-106">Return Type</span></span>|<span data-ttu-id="fe985-107">説明</span><span class="sxs-lookup"><span data-stu-id="fe985-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="fe985-108">List managedAppOperations</span><span class="sxs-lookup"><span data-stu-id="fe985-108">List managedAppOperations</span></span>](../api/intune_mam_managedappoperation_list.md)|<span data-ttu-id="fe985-109">[managedAppOperation](../resources/intune_mam_managedappoperation.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="fe985-109">[managedAppOperation](../resources/intune_mam_managedappoperation.md) collection</span></span>|<span data-ttu-id="fe985-110">[managedAppOperation](../resources/intune_mam_managedappoperation.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="fe985-110">List properties and relationships of the [managedAppOperation](../resources/intune_mam_managedappoperation.md) objects.</span></span>|
|[<span data-ttu-id="fe985-111">Get managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="fe985-111">Get managedAppOperation</span></span>](../api/intune_mam_managedappoperation_get.md)|[<span data-ttu-id="fe985-112">managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="fe985-112">managedAppOperation</span></span>](../resources/intune_mam_managedappoperation.md)|<span data-ttu-id="fe985-113">[managedAppOperation](../resources/intune_mam_managedappoperation.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="fe985-113">Read properties and relationships of [plannerTaskDetails](../resources/intune_mam_managedappoperation.md) object.</span></span>|
|[<span data-ttu-id="fe985-114">Create managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="fe985-114">Create managedAppOperation</span></span>](../api/intune_mam_managedappoperation_create.md)|[<span data-ttu-id="fe985-115">managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="fe985-115">managedAppOperation</span></span>](../resources/intune_mam_managedappoperation.md)|<span data-ttu-id="fe985-116">新しい [managedAppOperation](../resources/intune_mam_managedappoperation.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="fe985-116">Create a new [plannerBucket](../resources/intune_mam_managedappoperation.md) object.</span></span>|
|[<span data-ttu-id="fe985-117">Delete managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="fe985-117">Delete managedAppOperation</span></span>](../api/intune_mam_managedappoperation_delete.md)|<span data-ttu-id="fe985-118">なし</span><span class="sxs-lookup"><span data-stu-id="fe985-118">None</span></span>|<span data-ttu-id="fe985-119">[managedAppOperation](../resources/intune_mam_managedappoperation.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="fe985-119">Deletes a [managedAppOperation](../resources/intune_mam_managedappoperation.md).</span></span>|
|[<span data-ttu-id="fe985-120">Update managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="fe985-120">Update managedAppOperation</span></span>](../api/intune_mam_managedappoperation_update.md)|[<span data-ttu-id="fe985-121">managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="fe985-121">managedAppOperation</span></span>](../resources/intune_mam_managedappoperation.md)|<span data-ttu-id="fe985-122">[managedAppOperation](../resources/intune_mam_managedappoperation.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="fe985-122">Update the properties of a [calendar](../resources/intune_mam_managedappoperation.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="fe985-123">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fe985-123">Properties</span></span>
|<span data-ttu-id="fe985-124">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fe985-124">Property</span></span>|<span data-ttu-id="fe985-125">型</span><span class="sxs-lookup"><span data-stu-id="fe985-125">Type</span></span>|<span data-ttu-id="fe985-126">説明</span><span class="sxs-lookup"><span data-stu-id="fe985-126">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fe985-127">displayName</span><span class="sxs-lookup"><span data-stu-id="fe985-127">displayName</span></span>|<span data-ttu-id="fe985-128">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="fe985-128">String</span></span>|<span data-ttu-id="fe985-129">操作名。</span><span class="sxs-lookup"><span data-stu-id="fe985-129">The operation name.</span></span>|
|<span data-ttu-id="fe985-130">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fe985-130">lastModifiedDateTime</span></span>|<span data-ttu-id="fe985-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fe985-131">DateTimeOffset</span></span>|<span data-ttu-id="fe985-132">アプリ操作が変更された最終時刻。</span><span class="sxs-lookup"><span data-stu-id="fe985-132">The last time the app operation was modified.</span></span>|
|<span data-ttu-id="fe985-133">state</span><span class="sxs-lookup"><span data-stu-id="fe985-133">state</span></span>|<span data-ttu-id="fe985-134">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="fe985-134">String</span></span>|<span data-ttu-id="fe985-135">操作の現在の状態。</span><span class="sxs-lookup"><span data-stu-id="fe985-135">The current state of the operation</span></span>|
|<span data-ttu-id="fe985-136">id</span><span class="sxs-lookup"><span data-stu-id="fe985-136">id</span></span>|<span data-ttu-id="fe985-137">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="fe985-137">String</span></span>|<span data-ttu-id="fe985-138">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="fe985-138">Name of the entity.</span></span>|
|<span data-ttu-id="fe985-139">version</span><span class="sxs-lookup"><span data-stu-id="fe985-139">version</span></span>|<span data-ttu-id="fe985-140">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="fe985-140">String</span></span>|<span data-ttu-id="fe985-141">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="fe985-141">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fe985-142">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="fe985-142">Relationships</span></span>
<span data-ttu-id="fe985-143">なし</span><span class="sxs-lookup"><span data-stu-id="fe985-143">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="fe985-144">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="fe985-144">JSON Representation</span></span>
<span data-ttu-id="fe985-145">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="fe985-145">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAppOperation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppOperation",
  "displayName": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "state": "String",
  "id": "String (identifier)",
  "version": "String"
}
```



