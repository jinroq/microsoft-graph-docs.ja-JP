---
title: deleteUserFromSharedAppleDeviceActionResult リソースの種類
description: 共有の Apple デバイスのアクションの結果からユーザーを削除する
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c65a1c60a77ba196448dd626b345c69c71f16de6
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29399277"
---
# <a name="deleteuserfromsharedappledeviceactionresult-resource-type"></a><span data-ttu-id="af55b-103">deleteUserFromSharedAppleDeviceActionResult リソースの種類</span><span class="sxs-lookup"><span data-stu-id="af55b-103">deleteUserFromSharedAppleDeviceActionResult resource type</span></span>

> <span data-ttu-id="af55b-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="af55b-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="af55b-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="af55b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="af55b-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="af55b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="af55b-107">共有の Apple デバイスのアクションの結果からユーザーを削除する</span><span class="sxs-lookup"><span data-stu-id="af55b-107">Delete user from shared apple device action result</span></span>


<span data-ttu-id="af55b-108">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="af55b-108">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="af55b-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="af55b-109">Properties</span></span>
|<span data-ttu-id="af55b-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="af55b-110">Property</span></span>|<span data-ttu-id="af55b-111">型</span><span class="sxs-lookup"><span data-stu-id="af55b-111">Type</span></span>|<span data-ttu-id="af55b-112">説明</span><span class="sxs-lookup"><span data-stu-id="af55b-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="af55b-113">actionName</span><span class="sxs-lookup"><span data-stu-id="af55b-113">actionName</span></span>|<span data-ttu-id="af55b-114">String</span><span class="sxs-lookup"><span data-stu-id="af55b-114">String</span></span>|<span data-ttu-id="af55b-115">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) から継承されるアクション名</span><span class="sxs-lookup"><span data-stu-id="af55b-115">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="af55b-116">actionState</span><span class="sxs-lookup"><span data-stu-id="af55b-116">actionState</span></span>|[<span data-ttu-id="af55b-117">actionState</span><span class="sxs-lookup"><span data-stu-id="af55b-117">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="af55b-118">[DeviceActionResult](../resources/intune-devices-deviceactionresult.md)から継承される、アクションの状態です。</span><span class="sxs-lookup"><span data-stu-id="af55b-118">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="af55b-119">可能な値は、`none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported` です。</span><span class="sxs-lookup"><span data-stu-id="af55b-119">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="af55b-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="af55b-120">startDateTime</span></span>|<span data-ttu-id="af55b-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="af55b-121">DateTimeOffset</span></span>|<span data-ttu-id="af55b-122">アクションが開始された時刻 ([deviceActionResult](../resources/intune-devices-deviceactionresult.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="af55b-122">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="af55b-123">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="af55b-123">lastUpdatedDateTime</span></span>|<span data-ttu-id="af55b-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="af55b-124">DateTimeOffset</span></span>|<span data-ttu-id="af55b-125">アクション状態の最終更新時刻 ([deviceActionResult](../resources/intune-devices-deviceactionresult.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="af55b-125">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="af55b-126">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="af55b-126">userPrincipalName</span></span>|<span data-ttu-id="af55b-127">String</span><span class="sxs-lookup"><span data-stu-id="af55b-127">String</span></span>|<span data-ttu-id="af55b-128">削除するユーザーのユーザー プリンシパル名</span><span class="sxs-lookup"><span data-stu-id="af55b-128">User principal name of the user to be deleted</span></span>|

## <a name="relationships"></a><span data-ttu-id="af55b-129">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="af55b-129">Relationships</span></span>
<span data-ttu-id="af55b-130">なし</span><span class="sxs-lookup"><span data-stu-id="af55b-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="af55b-131">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="af55b-131">JSON Representation</span></span>
<span data-ttu-id="af55b-132">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="af55b-132">Here is a JSON representation of the resource.</span></span>
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




