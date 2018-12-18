---
title: deleteUserFromSharedAppleDeviceActionResult リソースの種類
description: 共有の Apple デバイスのアクションの結果からユーザーを削除する
author: tfitzmac
ms.openlocfilehash: 2dc6dbdeb8bb72314b25f695f82e4f4dfff0b8fd
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27356036"
---
# <a name="deleteuserfromsharedappledeviceactionresult-resource-type"></a><span data-ttu-id="b8922-103">deleteUserFromSharedAppleDeviceActionResult リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b8922-103">deleteUserFromSharedAppleDeviceActionResult resource type</span></span>

> <span data-ttu-id="b8922-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="b8922-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b8922-105">共有の Apple デバイスのアクションの結果からユーザーを削除する</span><span class="sxs-lookup"><span data-stu-id="b8922-105">Delete user from shared apple device action result</span></span>

<span data-ttu-id="b8922-106">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b8922-106">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="b8922-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b8922-107">Properties</span></span>
|<span data-ttu-id="b8922-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b8922-108">Property</span></span>|<span data-ttu-id="b8922-109">種類</span><span class="sxs-lookup"><span data-stu-id="b8922-109">Type</span></span>|<span data-ttu-id="b8922-110">説明</span><span class="sxs-lookup"><span data-stu-id="b8922-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b8922-111">actionName</span><span class="sxs-lookup"><span data-stu-id="b8922-111">actionName</span></span>|<span data-ttu-id="b8922-112">String</span><span class="sxs-lookup"><span data-stu-id="b8922-112">String</span></span>|<span data-ttu-id="b8922-113">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) から継承されるアクション名</span><span class="sxs-lookup"><span data-stu-id="b8922-113">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="b8922-114">actionState</span><span class="sxs-lookup"><span data-stu-id="b8922-114">actionState</span></span>|[<span data-ttu-id="b8922-115">actionState</span><span class="sxs-lookup"><span data-stu-id="b8922-115">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="b8922-116">[DeviceActionResult](../resources/intune-devices-deviceactionresult.md)から継承される、アクションの状態です。</span><span class="sxs-lookup"><span data-stu-id="b8922-116">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="b8922-117">可能な値は、`none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported` です。</span><span class="sxs-lookup"><span data-stu-id="b8922-117">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="b8922-118">startDateTime</span><span class="sxs-lookup"><span data-stu-id="b8922-118">startDateTime</span></span>|<span data-ttu-id="b8922-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b8922-119">DateTimeOffset</span></span>|<span data-ttu-id="b8922-120">アクションが開始された時刻 ([deviceActionResult](../resources/intune-devices-deviceactionresult.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="b8922-120">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="b8922-121">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="b8922-121">lastUpdatedDateTime</span></span>|<span data-ttu-id="b8922-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b8922-122">DateTimeOffset</span></span>|<span data-ttu-id="b8922-123">アクション状態の最終更新時刻 ([deviceActionResult](../resources/intune-devices-deviceactionresult.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="b8922-123">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="b8922-124">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="b8922-124">userPrincipalName</span></span>|<span data-ttu-id="b8922-125">String</span><span class="sxs-lookup"><span data-stu-id="b8922-125">String</span></span>|<span data-ttu-id="b8922-126">削除するユーザーのユーザー プリンシパル名</span><span class="sxs-lookup"><span data-stu-id="b8922-126">User principal name of the user to be deleted</span></span>|

## <a name="relationships"></a><span data-ttu-id="b8922-127">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b8922-127">Relationships</span></span>
<span data-ttu-id="b8922-128">なし</span><span class="sxs-lookup"><span data-stu-id="b8922-128">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b8922-129">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b8922-129">JSON Representation</span></span>
<span data-ttu-id="b8922-130">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="b8922-130">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
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



