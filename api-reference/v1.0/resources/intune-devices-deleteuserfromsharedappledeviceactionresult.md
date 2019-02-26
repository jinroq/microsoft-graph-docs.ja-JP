---
title: deleteUserFromSharedAppleDeviceActionResult リソースの種類
description: 共有の Apple デバイスのアクションの結果からユーザーを削除する
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5071c0c9168cfedbbaa527f82241c80b4ad53705
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30261524"
---
# <a name="deleteuserfromsharedappledeviceactionresult-resource-type"></a><span data-ttu-id="8652d-103">deleteUserFromSharedAppleDeviceActionResult リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8652d-103">deleteUserFromSharedAppleDeviceActionResult resource type</span></span>

> <span data-ttu-id="8652d-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="8652d-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8652d-105">共有の Apple デバイスのアクションの結果からユーザーを削除する</span><span class="sxs-lookup"><span data-stu-id="8652d-105">Delete user from shared apple device action result</span></span>


<span data-ttu-id="8652d-106">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8652d-106">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="8652d-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8652d-107">Properties</span></span>
|<span data-ttu-id="8652d-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8652d-108">Property</span></span>|<span data-ttu-id="8652d-109">型</span><span class="sxs-lookup"><span data-stu-id="8652d-109">Type</span></span>|<span data-ttu-id="8652d-110">説明</span><span class="sxs-lookup"><span data-stu-id="8652d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8652d-111">actionName</span><span class="sxs-lookup"><span data-stu-id="8652d-111">actionName</span></span>|<span data-ttu-id="8652d-112">String</span><span class="sxs-lookup"><span data-stu-id="8652d-112">String</span></span>|<span data-ttu-id="8652d-113">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) から継承されるアクション名</span><span class="sxs-lookup"><span data-stu-id="8652d-113">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="8652d-114">actionState</span><span class="sxs-lookup"><span data-stu-id="8652d-114">actionState</span></span>|[<span data-ttu-id="8652d-115">actionState</span><span class="sxs-lookup"><span data-stu-id="8652d-115">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="8652d-116">[deviceactionresult](../resources/intune-devices-deviceactionresult.md)から継承されるアクションの状態。</span><span class="sxs-lookup"><span data-stu-id="8652d-116">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="8652d-117">可能な値は、`none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported` です。</span><span class="sxs-lookup"><span data-stu-id="8652d-117">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="8652d-118">startDateTime</span><span class="sxs-lookup"><span data-stu-id="8652d-118">startDateTime</span></span>|<span data-ttu-id="8652d-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8652d-119">DateTimeOffset</span></span>|<span data-ttu-id="8652d-120">アクションが開始された時刻 ([deviceActionResult](../resources/intune-devices-deviceactionresult.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="8652d-120">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="8652d-121">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="8652d-121">lastUpdatedDateTime</span></span>|<span data-ttu-id="8652d-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8652d-122">DateTimeOffset</span></span>|<span data-ttu-id="8652d-123">アクション状態の最終更新時刻 ([deviceActionResult](../resources/intune-devices-deviceactionresult.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="8652d-123">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="8652d-124">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="8652d-124">userPrincipalName</span></span>|<span data-ttu-id="8652d-125">String</span><span class="sxs-lookup"><span data-stu-id="8652d-125">String</span></span>|<span data-ttu-id="8652d-126">削除するユーザーのユーザー プリンシパル名</span><span class="sxs-lookup"><span data-stu-id="8652d-126">User principal name of the user to be deleted</span></span>|

## <a name="relationships"></a><span data-ttu-id="8652d-127">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="8652d-127">Relationships</span></span>
<span data-ttu-id="8652d-128">なし</span><span class="sxs-lookup"><span data-stu-id="8652d-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8652d-129">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8652d-129">JSON Representation</span></span>
<span data-ttu-id="8652d-130">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="8652d-130">Here is a JSON representation of the resource.</span></span>
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



