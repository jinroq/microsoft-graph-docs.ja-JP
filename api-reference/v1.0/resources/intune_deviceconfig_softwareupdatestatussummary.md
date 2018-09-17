# <a name="softwareupdatestatussummary-resource-type"></a><span data-ttu-id="61bc1-101">softwareUpdateStatusSummary リソースの種類</span><span class="sxs-lookup"><span data-stu-id="61bc1-101">softwareUpdateStatusSummary resource type</span></span>

> <span data-ttu-id="61bc1-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="61bc1-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="61bc1-103">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="61bc1-103">Not yet documented</span></span>
## <a name="methods"></a><span data-ttu-id="61bc1-104">メソッド</span><span class="sxs-lookup"><span data-stu-id="61bc1-104">Methods</span></span>
|<span data-ttu-id="61bc1-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="61bc1-105">Method</span></span>|<span data-ttu-id="61bc1-106">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="61bc1-106">Return Type</span></span>|<span data-ttu-id="61bc1-107">説明</span><span class="sxs-lookup"><span data-stu-id="61bc1-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="61bc1-108">softwareUpdateStatusSummary の取得</span><span class="sxs-lookup"><span data-stu-id="61bc1-108">Get softwareUpdateStatusSummary</span></span>](../api/intune_deviceconfig_softwareupdatestatussummary_get.md)|[<span data-ttu-id="61bc1-109">softwareUpdateStatusSummary</span><span class="sxs-lookup"><span data-stu-id="61bc1-109">softwareUpdateStatusSummary</span></span>](../resources/intune_deviceconfig_softwareupdatestatussummary.md)|<span data-ttu-id="61bc1-110">[softwareUpdateStatusSummary](../resources/intune_deviceconfig_softwareupdatestatussummary.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="61bc1-110">Read properties and relationships of the [softwareUpdateStatusSummary](../resources/intune_deviceconfig_softwareupdatestatussummary.md) object.</span></span>|
|[<span data-ttu-id="61bc1-111">softwareUpdateStatusSummary の更新</span><span class="sxs-lookup"><span data-stu-id="61bc1-111">Update softwareUpdateStatusSummary</span></span>](../api/intune_deviceconfig_softwareupdatestatussummary_update.md)|[<span data-ttu-id="61bc1-112">softwareUpdateStatusSummary</span><span class="sxs-lookup"><span data-stu-id="61bc1-112">softwareUpdateStatusSummary</span></span>](../resources/intune_deviceconfig_softwareupdatestatussummary.md)|<span data-ttu-id="61bc1-113">[softwareUpdateStatusSummary](../resources/intune_deviceconfig_softwareupdatestatussummary.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="61bc1-113">Update the properties of a [softwareUpdateStatusSummary](../resources/intune_deviceconfig_softwareupdatestatussummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="61bc1-114">プロパティ</span><span class="sxs-lookup"><span data-stu-id="61bc1-114">Properties</span></span>
|<span data-ttu-id="61bc1-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="61bc1-115">Property</span></span>|<span data-ttu-id="61bc1-116">タイプ</span><span class="sxs-lookup"><span data-stu-id="61bc1-116">Type</span></span>|<span data-ttu-id="61bc1-117">説明</span><span class="sxs-lookup"><span data-stu-id="61bc1-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="61bc1-118">ID</span><span class="sxs-lookup"><span data-stu-id="61bc1-118">id</span></span>|<span data-ttu-id="61bc1-119">文字列</span><span class="sxs-lookup"><span data-stu-id="61bc1-119">String</span></span>|<span data-ttu-id="61bc1-120">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="61bc1-120">Key of the entity.</span></span>|
|<span data-ttu-id="61bc1-121">名前を表示する</span><span class="sxs-lookup"><span data-stu-id="61bc1-121">displayName</span></span>|<span data-ttu-id="61bc1-122">文字列</span><span class="sxs-lookup"><span data-stu-id="61bc1-122">String</span></span>|<span data-ttu-id="61bc1-123">ポリシーの名前。</span><span class="sxs-lookup"><span data-stu-id="61bc1-123">The name of the policy.</span></span>|
|<span data-ttu-id="61bc1-124">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="61bc1-124">compliantDeviceCount</span></span>|<span data-ttu-id="61bc1-125">Int32</span><span class="sxs-lookup"><span data-stu-id="61bc1-125">Int32</span></span>|<span data-ttu-id="61bc1-126">準拠デバイスの数。</span><span class="sxs-lookup"><span data-stu-id="61bc1-126">Number of compliant devices.</span></span>|
|<span data-ttu-id="61bc1-127">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="61bc1-127">nonCompliantDeviceCount</span></span>|<span data-ttu-id="61bc1-128">Int32</span><span class="sxs-lookup"><span data-stu-id="61bc1-128">Int32</span></span>|<span data-ttu-id="61bc1-129">準拠していないデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="61bc1-129">Number of non compliant devices.</span></span>|
|<span data-ttu-id="61bc1-130">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="61bc1-130">remediatedDeviceCount</span></span>|<span data-ttu-id="61bc1-131">Int32</span><span class="sxs-lookup"><span data-stu-id="61bc1-131">Int32</span></span>|<span data-ttu-id="61bc1-132">修復済みデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="61bc1-132">Number of remediated devices.</span></span>|
|<span data-ttu-id="61bc1-133">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="61bc1-133">errorDeviceCount</span></span>|<span data-ttu-id="61bc1-134">Int32</span><span class="sxs-lookup"><span data-stu-id="61bc1-134">Int32</span></span>|<span data-ttu-id="61bc1-135">エラーが発生したデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="61bc1-135">Number of devices had error.</span></span>|
|<span data-ttu-id="61bc1-136">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="61bc1-136">unknownDeviceCount</span></span>|<span data-ttu-id="61bc1-137">Int32</span><span class="sxs-lookup"><span data-stu-id="61bc1-137">Int32</span></span>|<span data-ttu-id="61bc1-138">不明なデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="61bc1-138">Number of unknown devices.</span></span>|
|<span data-ttu-id="61bc1-139">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="61bc1-139">conflictDeviceCount</span></span>|<span data-ttu-id="61bc1-140">Int32</span><span class="sxs-lookup"><span data-stu-id="61bc1-140">Int32</span></span>|<span data-ttu-id="61bc1-141">競合デバイスの数。</span><span class="sxs-lookup"><span data-stu-id="61bc1-141">Number of conflict devices.</span></span>|
|<span data-ttu-id="61bc1-142">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="61bc1-142">notApplicableDeviceCount</span></span>|<span data-ttu-id="61bc1-143">Int32</span><span class="sxs-lookup"><span data-stu-id="61bc1-143">Int32</span></span>|<span data-ttu-id="61bc1-144">該当しないデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="61bc1-144">Number of not applicable devices.</span></span>|
|<span data-ttu-id="61bc1-145">compliantUserCount</span><span class="sxs-lookup"><span data-stu-id="61bc1-145">compliantUserCount</span></span>|<span data-ttu-id="61bc1-146">Int32</span><span class="sxs-lookup"><span data-stu-id="61bc1-146">Int32</span></span>|<span data-ttu-id="61bc1-147">準拠ユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="61bc1-147">Number of compliant users.</span></span>|
|<span data-ttu-id="61bc1-148">nonCompliantUserCount</span><span class="sxs-lookup"><span data-stu-id="61bc1-148">nonCompliantUserCount</span></span>|<span data-ttu-id="61bc1-149">Int32</span><span class="sxs-lookup"><span data-stu-id="61bc1-149">Int32</span></span>|<span data-ttu-id="61bc1-150">準拠していないユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="61bc1-150">Number of non compliant users.</span></span>|
|<span data-ttu-id="61bc1-151">remediatedUserCount</span><span class="sxs-lookup"><span data-stu-id="61bc1-151">remediatedUserCount</span></span>|<span data-ttu-id="61bc1-152">Int32</span><span class="sxs-lookup"><span data-stu-id="61bc1-152">Int32</span></span>|<span data-ttu-id="61bc1-153">修復済みユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="61bc1-153">Number of remediated users.</span></span>|
|<span data-ttu-id="61bc1-154">errorUserCount</span><span class="sxs-lookup"><span data-stu-id="61bc1-154">errorUserCount</span></span>|<span data-ttu-id="61bc1-155">Int32</span><span class="sxs-lookup"><span data-stu-id="61bc1-155">Int32</span></span>|<span data-ttu-id="61bc1-156">エラーが発生したユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="61bc1-156">Number of users had error.</span></span>|
|<span data-ttu-id="61bc1-157">unknownUserCount</span><span class="sxs-lookup"><span data-stu-id="61bc1-157">unknownUserCount</span></span>|<span data-ttu-id="61bc1-158">Int32</span><span class="sxs-lookup"><span data-stu-id="61bc1-158">Int32</span></span>|<span data-ttu-id="61bc1-159">不明なユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="61bc1-159">Number of unknown users.</span></span>|
|<span data-ttu-id="61bc1-160">conflictUserCount</span><span class="sxs-lookup"><span data-stu-id="61bc1-160">conflictUserCount</span></span>|<span data-ttu-id="61bc1-161">Int32</span><span class="sxs-lookup"><span data-stu-id="61bc1-161">Int32</span></span>|<span data-ttu-id="61bc1-162">競合ユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="61bc1-162">Number of conflict users.</span></span>|
|<span data-ttu-id="61bc1-163">notApplicableUserCount</span><span class="sxs-lookup"><span data-stu-id="61bc1-163">notApplicableUserCount</span></span>|<span data-ttu-id="61bc1-164">Int32</span><span class="sxs-lookup"><span data-stu-id="61bc1-164">Int32</span></span>|<span data-ttu-id="61bc1-165">該当しないユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="61bc1-165">Number of not applicable users.</span></span>|

## <a name="relationships"></a><span data-ttu-id="61bc1-166">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="61bc1-166">Relationships</span></span>
<span data-ttu-id="61bc1-167">なし</span><span class="sxs-lookup"><span data-stu-id="61bc1-167">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="61bc1-168">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="61bc1-168">JSON Representation</span></span>
<span data-ttu-id="61bc1-169">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="61bc1-169">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "keyProperty": "id",
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








