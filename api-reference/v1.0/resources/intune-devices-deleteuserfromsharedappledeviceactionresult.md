---
title: deleteUserFromSharedAppleDeviceActionResult リソースの種類
description: 共有の Apple デバイスのアクションの結果からユーザーを削除する
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 997b9d9339abe44f8bc7427d9533b43066eac3b8
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27975457"
---
# <a name="deleteuserfromsharedappledeviceactionresult-resource-type"></a><span data-ttu-id="b310b-103">deleteUserFromSharedAppleDeviceActionResult リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b310b-103">deleteUserFromSharedAppleDeviceActionResult resource type</span></span>

> <span data-ttu-id="b310b-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="b310b-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b310b-105">共有の Apple デバイスのアクションの結果からユーザーを削除する</span><span class="sxs-lookup"><span data-stu-id="b310b-105">Delete user from shared apple device action result</span></span>

<span data-ttu-id="b310b-106">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b310b-106">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="b310b-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b310b-107">Properties</span></span>
|<span data-ttu-id="b310b-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b310b-108">Property</span></span>|<span data-ttu-id="b310b-109">種類</span><span class="sxs-lookup"><span data-stu-id="b310b-109">Type</span></span>|<span data-ttu-id="b310b-110">説明</span><span class="sxs-lookup"><span data-stu-id="b310b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b310b-111">actionName</span><span class="sxs-lookup"><span data-stu-id="b310b-111">actionName</span></span>|<span data-ttu-id="b310b-112">String</span><span class="sxs-lookup"><span data-stu-id="b310b-112">String</span></span>|<span data-ttu-id="b310b-113">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) から継承されるアクション名</span><span class="sxs-lookup"><span data-stu-id="b310b-113">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="b310b-114">actionState</span><span class="sxs-lookup"><span data-stu-id="b310b-114">actionState</span></span>|[<span data-ttu-id="b310b-115">actionState</span><span class="sxs-lookup"><span data-stu-id="b310b-115">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="b310b-116">[DeviceActionResult](../resources/intune-devices-deviceactionresult.md)から継承される、アクションの状態です。</span><span class="sxs-lookup"><span data-stu-id="b310b-116">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="b310b-117">可能な値は、`none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported` です。</span><span class="sxs-lookup"><span data-stu-id="b310b-117">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="b310b-118">startDateTime</span><span class="sxs-lookup"><span data-stu-id="b310b-118">startDateTime</span></span>|<span data-ttu-id="b310b-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b310b-119">DateTimeOffset</span></span>|<span data-ttu-id="b310b-120">アクションが開始された時刻 ([deviceActionResult](../resources/intune-devices-deviceactionresult.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="b310b-120">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="b310b-121">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="b310b-121">lastUpdatedDateTime</span></span>|<span data-ttu-id="b310b-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b310b-122">DateTimeOffset</span></span>|<span data-ttu-id="b310b-123">アクション状態の最終更新時刻 ([deviceActionResult](../resources/intune-devices-deviceactionresult.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="b310b-123">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="b310b-124">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="b310b-124">userPrincipalName</span></span>|<span data-ttu-id="b310b-125">String</span><span class="sxs-lookup"><span data-stu-id="b310b-125">String</span></span>|<span data-ttu-id="b310b-126">削除するユーザーのユーザー プリンシパル名</span><span class="sxs-lookup"><span data-stu-id="b310b-126">User principal name of the user to be deleted</span></span>|

## <a name="relationships"></a><span data-ttu-id="b310b-127">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b310b-127">Relationships</span></span>
<span data-ttu-id="b310b-128">なし</span><span class="sxs-lookup"><span data-stu-id="b310b-128">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b310b-129">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b310b-129">JSON Representation</span></span>
<span data-ttu-id="b310b-130">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="b310b-130">Here is a JSON representation of the resource.</span></span>
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



