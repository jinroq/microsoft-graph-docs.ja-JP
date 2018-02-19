# <a name="deleteuserfromsharedappledeviceactionresult-resource-type"></a><span data-ttu-id="fd8c6-101">deleteUserFromSharedAppleDeviceActionResult リソースの種類</span><span class="sxs-lookup"><span data-stu-id="fd8c6-101">deleteUserFromSharedAppleDeviceActionResult resource type</span></span>

> <span data-ttu-id="fd8c6-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="fd8c6-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fd8c6-103">共有の Apple デバイスのアクションの結果からユーザーを削除する</span><span class="sxs-lookup"><span data-stu-id="fd8c6-103">Delete user from shared apple device action result</span></span>

<span data-ttu-id="fd8c6-104">[deviceActionResult](../resources/intune_devices_deviceactionresult.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="fd8c6-104">Inherits from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="fd8c6-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fd8c6-105">Properties</span></span>
|<span data-ttu-id="fd8c6-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fd8c6-106">Property</span></span>|<span data-ttu-id="fd8c6-107">型</span><span class="sxs-lookup"><span data-stu-id="fd8c6-107">Type</span></span>|<span data-ttu-id="fd8c6-108">説明</span><span class="sxs-lookup"><span data-stu-id="fd8c6-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fd8c6-109">actionName</span><span class="sxs-lookup"><span data-stu-id="fd8c6-109">ActionName</span></span>|<span data-ttu-id="fd8c6-110">String</span><span class="sxs-lookup"><span data-stu-id="fd8c6-110">String</span></span>|<span data-ttu-id="fd8c6-111">[deviceActionResult](../resources/intune_devices_deviceactionresult.md) から継承されるアクション名</span><span class="sxs-lookup"><span data-stu-id="fd8c6-111">Action name Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>|
|<span data-ttu-id="fd8c6-112">actionState</span><span class="sxs-lookup"><span data-stu-id="fd8c6-112">actionState</span></span>|<span data-ttu-id="fd8c6-113">String</span><span class="sxs-lookup"><span data-stu-id="fd8c6-113">String</span></span>|<span data-ttu-id="fd8c6-114">[deviceActionResult](../resources/intune_devices_deviceactionresult.md) から継承されるアクションの状態です。可能な値は、`none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported` です。</span><span class="sxs-lookup"><span data-stu-id="fd8c6-114">State of the action Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md) Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="fd8c6-115">startDateTime</span><span class="sxs-lookup"><span data-stu-id="fd8c6-115">startDateTime</span></span>|<span data-ttu-id="fd8c6-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fd8c6-116">DateTimeOffset</span></span>|<span data-ttu-id="fd8c6-117">アクションが開始された時刻 ([deviceActionResult](../resources/intune_devices_deviceactionresult.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="fd8c6-117">Time the action was initiated Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>|
|<span data-ttu-id="fd8c6-118">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="fd8c6-118">lastUpdatedDateTime</span></span>|<span data-ttu-id="fd8c6-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fd8c6-119">DateTimeOffset</span></span>|<span data-ttu-id="fd8c6-120">アクション状態の最終更新時刻 ([deviceActionResult](../resources/intune_devices_deviceactionresult.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="fd8c6-120">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>|
|<span data-ttu-id="fd8c6-121">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="fd8c6-121">userPrincipalName</span></span>|<span data-ttu-id="fd8c6-122">String</span><span class="sxs-lookup"><span data-stu-id="fd8c6-122">String</span></span>|<span data-ttu-id="fd8c6-123">削除するユーザーのユーザー プリンシパル名</span><span class="sxs-lookup"><span data-stu-id="fd8c6-123">User principal name of the user to be deleted</span></span>|

## <a name="relationships"></a><span data-ttu-id="fd8c6-124">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="fd8c6-124">Relationships</span></span>
<span data-ttu-id="fd8c6-125">なし</span><span class="sxs-lookup"><span data-stu-id="fd8c6-125">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="fd8c6-126">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="fd8c6-126">JSON Representation</span></span>
<span data-ttu-id="fd8c6-127">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="fd8c6-127">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deleteUserFromSharedAppleDeviceActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deleteUserFromSharedAppleDeviceActionResult",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)",
  "userPrincipalName": "String"
}
```



