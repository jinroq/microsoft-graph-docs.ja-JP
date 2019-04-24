---
title: deleteUserFromSharedAppleDeviceActionResult リソースの種類
description: 共有の Apple デバイスのアクションの結果からユーザーを削除する
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5071c0c9168cfedbbaa527f82241c80b4ad53705
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32467177"
---
# <a name="deleteuserfromsharedappledeviceactionresult-resource-type"></a><span data-ttu-id="1a36b-103">deleteUserFromSharedAppleDeviceActionResult リソースの種類</span><span class="sxs-lookup"><span data-stu-id="1a36b-103">deleteUserFromSharedAppleDeviceActionResult resource type</span></span>

> <span data-ttu-id="1a36b-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="1a36b-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1a36b-105">共有の Apple デバイスのアクションの結果からユーザーを削除する</span><span class="sxs-lookup"><span data-stu-id="1a36b-105">Delete user from shared apple device action result</span></span>


<span data-ttu-id="1a36b-106">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1a36b-106">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="1a36b-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1a36b-107">Properties</span></span>
|<span data-ttu-id="1a36b-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1a36b-108">Property</span></span>|<span data-ttu-id="1a36b-109">型</span><span class="sxs-lookup"><span data-stu-id="1a36b-109">Type</span></span>|<span data-ttu-id="1a36b-110">説明</span><span class="sxs-lookup"><span data-stu-id="1a36b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1a36b-111">actionName</span><span class="sxs-lookup"><span data-stu-id="1a36b-111">actionName</span></span>|<span data-ttu-id="1a36b-112">String</span><span class="sxs-lookup"><span data-stu-id="1a36b-112">String</span></span>|<span data-ttu-id="1a36b-113">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) から継承されるアクション名</span><span class="sxs-lookup"><span data-stu-id="1a36b-113">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="1a36b-114">actionState</span><span class="sxs-lookup"><span data-stu-id="1a36b-114">actionState</span></span>|[<span data-ttu-id="1a36b-115">actionState</span><span class="sxs-lookup"><span data-stu-id="1a36b-115">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="1a36b-116">[deviceactionresult](../resources/intune-devices-deviceactionresult.md)から継承されるアクションの状態。</span><span class="sxs-lookup"><span data-stu-id="1a36b-116">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="1a36b-117">可能な値は、`none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported` です。</span><span class="sxs-lookup"><span data-stu-id="1a36b-117">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="1a36b-118">startDateTime</span><span class="sxs-lookup"><span data-stu-id="1a36b-118">startDateTime</span></span>|<span data-ttu-id="1a36b-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1a36b-119">DateTimeOffset</span></span>|<span data-ttu-id="1a36b-120">アクションが開始された時刻。[deviceActionResult](../resources/intune-devices-deviceactionresult.md) から継承。</span><span class="sxs-lookup"><span data-stu-id="1a36b-120">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="1a36b-121">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="1a36b-121">lastUpdatedDateTime</span></span>|<span data-ttu-id="1a36b-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1a36b-122">DateTimeOffset</span></span>|<span data-ttu-id="1a36b-123">アクション状態の最終更新時刻 ([deviceActionResult](../resources/intune-devices-deviceactionresult.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="1a36b-123">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="1a36b-124">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="1a36b-124">userPrincipalName</span></span>|<span data-ttu-id="1a36b-125">String</span><span class="sxs-lookup"><span data-stu-id="1a36b-125">String</span></span>|<span data-ttu-id="1a36b-126">削除するユーザーのユーザー プリンシパル名</span><span class="sxs-lookup"><span data-stu-id="1a36b-126">User principal name of the user to be deleted</span></span>|

## <a name="relationships"></a><span data-ttu-id="1a36b-127">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="1a36b-127">Relationships</span></span>
<span data-ttu-id="1a36b-128">なし</span><span class="sxs-lookup"><span data-stu-id="1a36b-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1a36b-129">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="1a36b-129">JSON Representation</span></span>
<span data-ttu-id="1a36b-130">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="1a36b-130">Here is a JSON representation of the resource.</span></span>
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



