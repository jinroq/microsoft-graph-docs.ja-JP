# <a name="softwareupdatestatussummary-resource-type"></a><span data-ttu-id="e0d6c-101">softwareUpdateStatusSummary リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e0d6c-101">softwareUpdateStatusSummary resource type</span></span>

> <span data-ttu-id="e0d6c-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="e0d6c-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e0d6c-103">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="e0d6c-103">Not yet documented</span></span>
## <a name="methods"></a><span data-ttu-id="e0d6c-104">メソッド</span><span class="sxs-lookup"><span data-stu-id="e0d6c-104">Methods</span></span>
|<span data-ttu-id="e0d6c-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="e0d6c-105">Method</span></span>|<span data-ttu-id="e0d6c-106">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="e0d6c-106">Return Type</span></span>|<span data-ttu-id="e0d6c-107">説明</span><span class="sxs-lookup"><span data-stu-id="e0d6c-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e0d6c-108">Get softwareUpdateStatusSummary</span><span class="sxs-lookup"><span data-stu-id="e0d6c-108">Get softwareUpdateStatusSummary</span></span>](../api/intune_deviceconfig_softwareupdatestatussummary_get.md)|[<span data-ttu-id="e0d6c-109">softwareUpdateStatusSummary</span><span class="sxs-lookup"><span data-stu-id="e0d6c-109">softwareUpdateStatusSummary</span></span>](../resources/intune_deviceconfig_softwareupdatestatussummary.md)|<span data-ttu-id="e0d6c-110">[softwareUpdateStatusSummary](../resources/intune_deviceconfig_softwareupdatestatussummary.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="e0d6c-110">Read properties and relationships of the [softwareUpdateStatusSummary](../resources/intune_deviceconfig_softwareupdatestatussummary.md) object.</span></span>|
|[<span data-ttu-id="e0d6c-111">Update softwareUpdateStatusSummary</span><span class="sxs-lookup"><span data-stu-id="e0d6c-111">Update softwareUpdateStatusSummary</span></span>](../api/intune_deviceconfig_softwareupdatestatussummary_update.md)|[<span data-ttu-id="e0d6c-112">softwareUpdateStatusSummary</span><span class="sxs-lookup"><span data-stu-id="e0d6c-112">softwareUpdateStatusSummary</span></span>](../resources/intune_deviceconfig_softwareupdatestatussummary.md)|<span data-ttu-id="e0d6c-113">[softwareUpdateStatusSummary](../resources/intune_deviceconfig_softwareupdatestatussummary.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="e0d6c-113">Update the properties of a [softwareUpdateStatusSummary](../resources/intune_deviceconfig_softwareupdatestatussummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="e0d6c-114">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e0d6c-114">Properties</span></span>
|<span data-ttu-id="e0d6c-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e0d6c-115">Property</span></span>|<span data-ttu-id="e0d6c-116">型</span><span class="sxs-lookup"><span data-stu-id="e0d6c-116">Type</span></span>|<span data-ttu-id="e0d6c-117">説明</span><span class="sxs-lookup"><span data-stu-id="e0d6c-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e0d6c-118">id</span><span class="sxs-lookup"><span data-stu-id="e0d6c-118">id</span></span>|<span data-ttu-id="e0d6c-119">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="e0d6c-119">String</span></span>|<span data-ttu-id="e0d6c-120">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="e0d6c-120">Key of the entity.</span></span>|
|<span data-ttu-id="e0d6c-121">displayName</span><span class="sxs-lookup"><span data-stu-id="e0d6c-121">displayName</span></span>|<span data-ttu-id="e0d6c-122">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="e0d6c-122">String</span></span>|<span data-ttu-id="e0d6c-123">ポリシーの名前。</span><span class="sxs-lookup"><span data-stu-id="e0d6c-123">The name of the policy.</span></span>|
|<span data-ttu-id="e0d6c-124">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e0d6c-124">compliantDeviceCount</span></span>|<span data-ttu-id="e0d6c-125">Int32</span><span class="sxs-lookup"><span data-stu-id="e0d6c-125">Int32</span></span>|<span data-ttu-id="e0d6c-126">準拠デバイスの数。</span><span class="sxs-lookup"><span data-stu-id="e0d6c-126">Number of compliant devices.</span></span>|
|<span data-ttu-id="e0d6c-127">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e0d6c-127">nonCompliantDeviceCount</span></span>|<span data-ttu-id="e0d6c-128">Int32</span><span class="sxs-lookup"><span data-stu-id="e0d6c-128">Int32</span></span>|<span data-ttu-id="e0d6c-129">準拠していないデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="e0d6c-129">Number of non compliant devices.</span></span>|
|<span data-ttu-id="e0d6c-130">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e0d6c-130">remediatedDeviceCount</span></span>|<span data-ttu-id="e0d6c-131">Int32</span><span class="sxs-lookup"><span data-stu-id="e0d6c-131">Int32</span></span>|<span data-ttu-id="e0d6c-132">修復済みデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="e0d6c-132">Number of remediated devices.</span></span>|
|<span data-ttu-id="e0d6c-133">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e0d6c-133">errorDeviceCount</span></span>|<span data-ttu-id="e0d6c-134">Int32</span><span class="sxs-lookup"><span data-stu-id="e0d6c-134">Int32</span></span>|<span data-ttu-id="e0d6c-135">エラーが発生したデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="e0d6c-135">Number of devices had error.</span></span>|
|<span data-ttu-id="e0d6c-136">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e0d6c-136">unknownDeviceCount</span></span>|<span data-ttu-id="e0d6c-137">Int32</span><span class="sxs-lookup"><span data-stu-id="e0d6c-137">Int32</span></span>|<span data-ttu-id="e0d6c-138">不明なデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="e0d6c-138">Number of unknown devices.</span></span>|
|<span data-ttu-id="e0d6c-139">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e0d6c-139">conflictDeviceCount</span></span>|<span data-ttu-id="e0d6c-140">Int32</span><span class="sxs-lookup"><span data-stu-id="e0d6c-140">Int32</span></span>|<span data-ttu-id="e0d6c-141">競合デバイスの数。</span><span class="sxs-lookup"><span data-stu-id="e0d6c-141">Number of conflict devices.</span></span>|
|<span data-ttu-id="e0d6c-142">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e0d6c-142">notApplicableDeviceCount</span></span>|<span data-ttu-id="e0d6c-143">Int32</span><span class="sxs-lookup"><span data-stu-id="e0d6c-143">Int32</span></span>|<span data-ttu-id="e0d6c-144">該当しないデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="e0d6c-144">Number of not applicable devices.</span></span>|
|<span data-ttu-id="e0d6c-145">compliantUserCount</span><span class="sxs-lookup"><span data-stu-id="e0d6c-145">compliantUserCount</span></span>|<span data-ttu-id="e0d6c-146">Int32</span><span class="sxs-lookup"><span data-stu-id="e0d6c-146">Int32</span></span>|<span data-ttu-id="e0d6c-147">準拠ユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="e0d6c-147">Number of compliant users.</span></span>|
|<span data-ttu-id="e0d6c-148">nonCompliantUserCount</span><span class="sxs-lookup"><span data-stu-id="e0d6c-148">nonCompliantUserCount</span></span>|<span data-ttu-id="e0d6c-149">Int32</span><span class="sxs-lookup"><span data-stu-id="e0d6c-149">Int32</span></span>|<span data-ttu-id="e0d6c-150">準拠していないユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="e0d6c-150">Number of non compliant users.</span></span>|
|<span data-ttu-id="e0d6c-151">remediatedUserCount</span><span class="sxs-lookup"><span data-stu-id="e0d6c-151">remediatedUserCount</span></span>|<span data-ttu-id="e0d6c-152">Int32</span><span class="sxs-lookup"><span data-stu-id="e0d6c-152">Int32</span></span>|<span data-ttu-id="e0d6c-153">修復済みユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="e0d6c-153">Number of remediated users.</span></span>|
|<span data-ttu-id="e0d6c-154">errorUserCount</span><span class="sxs-lookup"><span data-stu-id="e0d6c-154">errorUserCount</span></span>|<span data-ttu-id="e0d6c-155">Int32</span><span class="sxs-lookup"><span data-stu-id="e0d6c-155">Int32</span></span>|<span data-ttu-id="e0d6c-156">エラーが発生したユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="e0d6c-156">Number of users had error.</span></span>|
|<span data-ttu-id="e0d6c-157">unknownUserCount</span><span class="sxs-lookup"><span data-stu-id="e0d6c-157">unknownUserCount</span></span>|<span data-ttu-id="e0d6c-158">Int32</span><span class="sxs-lookup"><span data-stu-id="e0d6c-158">Int32</span></span>|<span data-ttu-id="e0d6c-159">不明なユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="e0d6c-159">Number of unknown users.</span></span>|
|<span data-ttu-id="e0d6c-160">conflictUserCount</span><span class="sxs-lookup"><span data-stu-id="e0d6c-160">conflictUserCount</span></span>|<span data-ttu-id="e0d6c-161">Int32</span><span class="sxs-lookup"><span data-stu-id="e0d6c-161">Int32</span></span>|<span data-ttu-id="e0d6c-162">競合ユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="e0d6c-162">Number of conflict users.</span></span>|
|<span data-ttu-id="e0d6c-163">notApplicableUserCount</span><span class="sxs-lookup"><span data-stu-id="e0d6c-163">notApplicableUserCount</span></span>|<span data-ttu-id="e0d6c-164">Int32</span><span class="sxs-lookup"><span data-stu-id="e0d6c-164">Int32</span></span>|<span data-ttu-id="e0d6c-165">該当しないユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="e0d6c-165">Number of not applicable users.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e0d6c-166">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e0d6c-166">Relationships</span></span>
<span data-ttu-id="e0d6c-167">なし</span><span class="sxs-lookup"><span data-stu-id="e0d6c-167">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="e0d6c-168">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e0d6c-168">JSON Representation</span></span>
<span data-ttu-id="e0d6c-169">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="e0d6c-169">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.softwareUpdateStatusSummary"
}
-->
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



