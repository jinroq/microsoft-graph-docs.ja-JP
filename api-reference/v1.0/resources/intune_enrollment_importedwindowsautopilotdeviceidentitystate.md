# <a name="importedwindowsautopilotdeviceidentitystate-resource-type"></a><span data-ttu-id="52a47-101">importedWindowsAutopilotDeviceIdentityState リソースの種類</span><span class="sxs-lookup"><span data-stu-id="52a47-101">importedWindowsAutopilotDeviceIdentityState resource type</span></span>

> <span data-ttu-id="52a47-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="52a47-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="52a47-103">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="52a47-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="52a47-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="52a47-104">Properties</span></span>
|<span data-ttu-id="52a47-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="52a47-105">Property</span></span>|<span data-ttu-id="52a47-106">型</span><span class="sxs-lookup"><span data-stu-id="52a47-106">Type</span></span>|<span data-ttu-id="52a47-107">説明</span><span class="sxs-lookup"><span data-stu-id="52a47-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="52a47-108">deviceImportStatus</span><span class="sxs-lookup"><span data-stu-id="52a47-108">deviceImportStatus</span></span>|<span data-ttu-id="52a47-109">String</span><span class="sxs-lookup"><span data-stu-id="52a47-109">String</span></span>|<span data-ttu-id="52a47-110">Device Directory Service (DDS) から報告されたデバイスの状態です。</span><span class="sxs-lookup"><span data-stu-id="52a47-110">Device status reported by Device Directory Service(DDS).</span></span> <span data-ttu-id="52a47-111">可能な値は、`unknown`、`pending`、`partial`、`complete`、`error` です。</span><span class="sxs-lookup"><span data-stu-id="52a47-111">Possible values are: `unknown`, `pending`, `partial`, `complete`, `error`.</span></span>|
|<span data-ttu-id="52a47-112">deviceRegistrationId</span><span class="sxs-lookup"><span data-stu-id="52a47-112">deviceRegistrationId</span></span>|<span data-ttu-id="52a47-113">String</span><span class="sxs-lookup"><span data-stu-id="52a47-113">String</span></span>|<span data-ttu-id="52a47-114">正常に追加されたと Devce Directory Service (DDS) から報告されたデバイスの Devce Registration ID です。</span><span class="sxs-lookup"><span data-stu-id="52a47-114">Device Registration ID for successfully added device reported by Device Directory Service(DDS).</span></span>|
|<span data-ttu-id="52a47-115">deviceErrorCode</span><span class="sxs-lookup"><span data-stu-id="52a47-115">deviceErrorCode</span></span>|<span data-ttu-id="52a47-116">Int32</span><span class="sxs-lookup"><span data-stu-id="52a47-116">Int32</span></span>|<span data-ttu-id="52a47-117">Device Directory Service (DDS) から報告されたデバイス エラー コードです。</span><span class="sxs-lookup"><span data-stu-id="52a47-117">Device error code reported by Device Directory Service(DDS).</span></span>|
|<span data-ttu-id="52a47-118">deviceErrorName</span><span class="sxs-lookup"><span data-stu-id="52a47-118">deviceErrorName</span></span>|<span data-ttu-id="52a47-119">String</span><span class="sxs-lookup"><span data-stu-id="52a47-119">String</span></span>|<span data-ttu-id="52a47-120">Device Directory Service (DDS) から報告されたデバイス エラー名です。</span><span class="sxs-lookup"><span data-stu-id="52a47-120">Device error name reported by Device Directory Service(DDS).</span></span>|

## <a name="relationships"></a><span data-ttu-id="52a47-121">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="52a47-121">Relationships</span></span>
<span data-ttu-id="52a47-122">なし</span><span class="sxs-lookup"><span data-stu-id="52a47-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="52a47-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="52a47-123">JSON Representation</span></span>
<span data-ttu-id="52a47-124">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="52a47-124">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.importedWindowsAutopilotDeviceIdentityState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.importedWindowsAutopilotDeviceIdentityState",
  "deviceImportStatus": "String",
  "deviceRegistrationId": "String",
  "deviceErrorCode": 1024,
  "deviceErrorName": "String"
}
```



