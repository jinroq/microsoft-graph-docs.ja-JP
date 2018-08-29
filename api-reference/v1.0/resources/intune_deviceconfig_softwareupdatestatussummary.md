# <a name="softwareupdatestatussummary-resource-type"></a><span data-ttu-id="d3762-101">softwareUpdateStatusSummary リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d3762-101">softwareUpdateStatusSummary resource type</span></span>

> <span data-ttu-id="d3762-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="d3762-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d3762-103">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="d3762-103">Not yet documented</span></span>
## <a name="methods"></a><span data-ttu-id="d3762-104">メソッド</span><span class="sxs-lookup"><span data-stu-id="d3762-104">Methods</span></span>
|<span data-ttu-id="d3762-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="d3762-105">Method</span></span>|<span data-ttu-id="d3762-106">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="d3762-106">Return Type</span></span>|<span data-ttu-id="d3762-107">説明</span><span class="sxs-lookup"><span data-stu-id="d3762-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d3762-108">softwareUpdateStatusSummary の取得</span><span class="sxs-lookup"><span data-stu-id="d3762-108">Get softwareUpdateStatusSummary</span></span>](../api/intune_deviceconfig_softwareupdatestatussummary_get.md)|[<span data-ttu-id="d3762-109">softwareUpdateStatusSummary</span><span class="sxs-lookup"><span data-stu-id="d3762-109">softwareUpdateStatusSummary</span></span>](../resources/intune_deviceconfig_softwareupdatestatussummary.md)|<span data-ttu-id="d3762-110">[softwareUpdateStatusSummary](../resources/intune_deviceconfig_softwareupdatestatussummary.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="d3762-110">Read properties and relationships of the [softwareUpdateStatusSummary](../resources/intune_deviceconfig_softwareupdatestatussummary.md) object.</span></span>|
|[<span data-ttu-id="d3762-111">softwareUpdateStatusSummary の更新</span><span class="sxs-lookup"><span data-stu-id="d3762-111">Update softwareUpdateStatusSummary</span></span>](../api/intune_deviceconfig_softwareupdatestatussummary_update.md)|[<span data-ttu-id="d3762-112">softwareUpdateStatusSummary</span><span class="sxs-lookup"><span data-stu-id="d3762-112">softwareUpdateStatusSummary</span></span>](../resources/intune_deviceconfig_softwareupdatestatussummary.md)|<span data-ttu-id="d3762-113">[softwareUpdateStatusSummary](../resources/intune_deviceconfig_softwareupdatestatussummary.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="d3762-113">Update the properties of a [softwareUpdateStatusSummary](../resources/intune_deviceconfig_softwareupdatestatussummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="d3762-114">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d3762-114">Properties</span></span>
|<span data-ttu-id="d3762-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d3762-115">Property</span></span>|<span data-ttu-id="d3762-116">タイプ</span><span class="sxs-lookup"><span data-stu-id="d3762-116">Type</span></span>|<span data-ttu-id="d3762-117">説明</span><span class="sxs-lookup"><span data-stu-id="d3762-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d3762-118">ID</span><span class="sxs-lookup"><span data-stu-id="d3762-118">id</span></span>|<span data-ttu-id="d3762-119">文字列</span><span class="sxs-lookup"><span data-stu-id="d3762-119">String</span></span>|<span data-ttu-id="d3762-120">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="d3762-120">Key of the entity.</span></span>|
|<span data-ttu-id="d3762-121">displayName</span><span class="sxs-lookup"><span data-stu-id="d3762-121">displayName</span></span>|<span data-ttu-id="d3762-122">文字列</span><span class="sxs-lookup"><span data-stu-id="d3762-122">String</span></span>|<span data-ttu-id="d3762-123">ポリシーの名前。</span><span class="sxs-lookup"><span data-stu-id="d3762-123">The name of the policy.</span></span>|
|<span data-ttu-id="d3762-124">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d3762-124">compliantDeviceCount</span></span>|<span data-ttu-id="d3762-125">Int32</span><span class="sxs-lookup"><span data-stu-id="d3762-125">Int32</span></span>|<span data-ttu-id="d3762-126">準拠デバイスの数。</span><span class="sxs-lookup"><span data-stu-id="d3762-126">Number of compliant devices.</span></span>|
|<span data-ttu-id="d3762-127">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d3762-127">nonCompliantDeviceCount</span></span>|<span data-ttu-id="d3762-128">Int32</span><span class="sxs-lookup"><span data-stu-id="d3762-128">Int32</span></span>|<span data-ttu-id="d3762-129">準拠していないデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="d3762-129">Number of non compliant devices.</span></span>|
|<span data-ttu-id="d3762-130">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d3762-130">remediatedDeviceCount</span></span>|<span data-ttu-id="d3762-131">Int32</span><span class="sxs-lookup"><span data-stu-id="d3762-131">Int32</span></span>|<span data-ttu-id="d3762-132">修復済みデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="d3762-132">Number of remediated devices.</span></span>|
|<span data-ttu-id="d3762-133">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d3762-133">errorDeviceCount</span></span>|<span data-ttu-id="d3762-134">Int32</span><span class="sxs-lookup"><span data-stu-id="d3762-134">Int32</span></span>|<span data-ttu-id="d3762-135">エラーが発生したデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="d3762-135">Number of devices had error.</span></span>|
|<span data-ttu-id="d3762-136">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d3762-136">unknownDeviceCount</span></span>|<span data-ttu-id="d3762-137">Int32</span><span class="sxs-lookup"><span data-stu-id="d3762-137">Int32</span></span>|<span data-ttu-id="d3762-138">不明なデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="d3762-138">Number of unknown devices.</span></span>|
|<span data-ttu-id="d3762-139">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d3762-139">conflictDeviceCount</span></span>|<span data-ttu-id="d3762-140">Int32</span><span class="sxs-lookup"><span data-stu-id="d3762-140">Int32</span></span>|<span data-ttu-id="d3762-141">競合デバイスの数。</span><span class="sxs-lookup"><span data-stu-id="d3762-141">Number of conflict devices.</span></span>|
|<span data-ttu-id="d3762-142">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d3762-142">notApplicableDeviceCount</span></span>|<span data-ttu-id="d3762-143">Int32</span><span class="sxs-lookup"><span data-stu-id="d3762-143">Int32</span></span>|<span data-ttu-id="d3762-144">該当しないデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="d3762-144">Number of not applicable devices.</span></span>|
|<span data-ttu-id="d3762-145">compliantUserCount</span><span class="sxs-lookup"><span data-stu-id="d3762-145">compliantUserCount</span></span>|<span data-ttu-id="d3762-146">Int32</span><span class="sxs-lookup"><span data-stu-id="d3762-146">Int32</span></span>|<span data-ttu-id="d3762-147">準拠ユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="d3762-147">Number of compliant users.</span></span>|
|<span data-ttu-id="d3762-148">nonCompliantUserCount</span><span class="sxs-lookup"><span data-stu-id="d3762-148">nonCompliantUserCount</span></span>|<span data-ttu-id="d3762-149">Int32</span><span class="sxs-lookup"><span data-stu-id="d3762-149">Int32</span></span>|<span data-ttu-id="d3762-150">準拠していないユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="d3762-150">Number of non compliant users.</span></span>|
|<span data-ttu-id="d3762-151">remediatedUserCount</span><span class="sxs-lookup"><span data-stu-id="d3762-151">remediatedUserCount</span></span>|<span data-ttu-id="d3762-152">Int32</span><span class="sxs-lookup"><span data-stu-id="d3762-152">Int32</span></span>|<span data-ttu-id="d3762-153">修復済みユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="d3762-153">Number of remediated users.</span></span>|
|<span data-ttu-id="d3762-154">errorUserCount</span><span class="sxs-lookup"><span data-stu-id="d3762-154">errorUserCount</span></span>|<span data-ttu-id="d3762-155">Int32</span><span class="sxs-lookup"><span data-stu-id="d3762-155">Int32</span></span>|<span data-ttu-id="d3762-156">エラーが発生したユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="d3762-156">Number of users had error.</span></span>|
|<span data-ttu-id="d3762-157">unknownUserCount</span><span class="sxs-lookup"><span data-stu-id="d3762-157">unknownUserCount</span></span>|<span data-ttu-id="d3762-158">Int32</span><span class="sxs-lookup"><span data-stu-id="d3762-158">Int32</span></span>|<span data-ttu-id="d3762-159">不明なユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="d3762-159">Number of unknown users.</span></span>|
|<span data-ttu-id="d3762-160">conflictUserCount</span><span class="sxs-lookup"><span data-stu-id="d3762-160">conflictUserCount</span></span>|<span data-ttu-id="d3762-161">Int32</span><span class="sxs-lookup"><span data-stu-id="d3762-161">Int32</span></span>|<span data-ttu-id="d3762-162">競合ユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="d3762-162">Number of conflict users.</span></span>|
|<span data-ttu-id="d3762-163">notApplicableUserCount</span><span class="sxs-lookup"><span data-stu-id="d3762-163">notApplicableUserCount</span></span>|<span data-ttu-id="d3762-164">Int32</span><span class="sxs-lookup"><span data-stu-id="d3762-164">Int32</span></span>|<span data-ttu-id="d3762-165">該当しないユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="d3762-165">Number of not applicable users.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d3762-166">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="d3762-166">Relationships</span></span>
<span data-ttu-id="d3762-167">なし</span><span class="sxs-lookup"><span data-stu-id="d3762-167">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="d3762-168">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d3762-168">JSON Representation</span></span>
<span data-ttu-id="d3762-169">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="d3762-169">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.softwareUpdateStatusSummary"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.softwareUpdateStatusSummary",
  "id": "String (identifier)",
  "displayName": "String",
  "compliantDeviceCount": 1024,
  "nonCompliantDeviceCount": 1024,
  "remediatedDeviceCount": 1024,
  "errorDeviceCount": 1024,
  "unknownDeviceCount": 1024,
  "conflictDeviceCount": 1024,
  "notApplicableDeviceCount": 1024,
  "compliantUserCount": 1024,
  "nonCompliantUserCount": 1024,
  "remediatedUserCount": 1024,
  "errorUserCount": 1024,
  "unknownUserCount": 1024,
  "conflictUserCount": 1024,
  "notApplicableUserCount": 1024
}
```



