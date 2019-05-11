---
title: deleteUserFromSharedAppleDeviceActionResult リソースの種類
description: 共有の Apple デバイスのアクションの結果からユーザーを削除する
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4a86128b3bb8f863c21225567c91dc0a9938bc7b
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33942179"
---
# <a name="deleteuserfromsharedappledeviceactionresult-resource-type"></a><span data-ttu-id="8bddb-103">deleteUserFromSharedAppleDeviceActionResult リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8bddb-103">deleteUserFromSharedAppleDeviceActionResult resource type</span></span>

> <span data-ttu-id="8bddb-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8bddb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8bddb-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="8bddb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8bddb-106">共有の Apple デバイスのアクションの結果からユーザーを削除する</span><span class="sxs-lookup"><span data-stu-id="8bddb-106">Delete user from shared apple device action result</span></span>


<span data-ttu-id="8bddb-107">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8bddb-107">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="8bddb-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8bddb-108">Properties</span></span>
|<span data-ttu-id="8bddb-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8bddb-109">Property</span></span>|<span data-ttu-id="8bddb-110">型</span><span class="sxs-lookup"><span data-stu-id="8bddb-110">Type</span></span>|<span data-ttu-id="8bddb-111">説明</span><span class="sxs-lookup"><span data-stu-id="8bddb-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8bddb-112">actionName</span><span class="sxs-lookup"><span data-stu-id="8bddb-112">actionName</span></span>|<span data-ttu-id="8bddb-113">String</span><span class="sxs-lookup"><span data-stu-id="8bddb-113">String</span></span>|<span data-ttu-id="8bddb-114">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) から継承されるアクション名</span><span class="sxs-lookup"><span data-stu-id="8bddb-114">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="8bddb-115">actionState</span><span class="sxs-lookup"><span data-stu-id="8bddb-115">actionState</span></span>|[<span data-ttu-id="8bddb-116">actionState</span><span class="sxs-lookup"><span data-stu-id="8bddb-116">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="8bddb-117">[Deviceactionresult](../resources/intune-devices-deviceactionresult.md)から継承されるアクションの状態。</span><span class="sxs-lookup"><span data-stu-id="8bddb-117">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="8bddb-118">可能な値は、`none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported` です。</span><span class="sxs-lookup"><span data-stu-id="8bddb-118">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="8bddb-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="8bddb-119">startDateTime</span></span>|<span data-ttu-id="8bddb-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8bddb-120">DateTimeOffset</span></span>|<span data-ttu-id="8bddb-121">アクションが開始された時刻。[deviceActionResult](../resources/intune-devices-deviceactionresult.md) から継承。</span><span class="sxs-lookup"><span data-stu-id="8bddb-121">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="8bddb-122">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="8bddb-122">lastUpdatedDateTime</span></span>|<span data-ttu-id="8bddb-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8bddb-123">DateTimeOffset</span></span>|<span data-ttu-id="8bddb-124">アクション状態の最終更新時刻 ([deviceActionResult](../resources/intune-devices-deviceactionresult.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="8bddb-124">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="8bddb-125">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="8bddb-125">userPrincipalName</span></span>|<span data-ttu-id="8bddb-126">String</span><span class="sxs-lookup"><span data-stu-id="8bddb-126">String</span></span>|<span data-ttu-id="8bddb-127">削除するユーザーのユーザー プリンシパル名</span><span class="sxs-lookup"><span data-stu-id="8bddb-127">User principal name of the user to be deleted</span></span>|

## <a name="relationships"></a><span data-ttu-id="8bddb-128">関係</span><span class="sxs-lookup"><span data-stu-id="8bddb-128">Relationships</span></span>
<span data-ttu-id="8bddb-129">なし</span><span class="sxs-lookup"><span data-stu-id="8bddb-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8bddb-130">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8bddb-130">JSON Representation</span></span>
<span data-ttu-id="8bddb-131">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="8bddb-131">Here is a JSON representation of the resource.</span></span>
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




