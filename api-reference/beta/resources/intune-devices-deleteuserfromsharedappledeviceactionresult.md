---
title: deleteUserFromSharedAppleDeviceActionResult リソースの種類
description: 共有の Apple デバイスのアクションの結果からユーザーを削除する
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 368a7acc2fd90e79b3ed1361220dd70f722cd217
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30173242"
---
# <a name="deleteuserfromsharedappledeviceactionresult-resource-type"></a><span data-ttu-id="41081-103">deleteUserFromSharedAppleDeviceActionResult リソースの種類</span><span class="sxs-lookup"><span data-stu-id="41081-103">deleteUserFromSharedAppleDeviceActionResult resource type</span></span>

> <span data-ttu-id="41081-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="41081-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="41081-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="41081-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="41081-106">共有の Apple デバイスのアクションの結果からユーザーを削除する</span><span class="sxs-lookup"><span data-stu-id="41081-106">Delete user from shared apple device action result</span></span>


<span data-ttu-id="41081-107">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="41081-107">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="41081-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="41081-108">Properties</span></span>
|<span data-ttu-id="41081-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="41081-109">Property</span></span>|<span data-ttu-id="41081-110">型</span><span class="sxs-lookup"><span data-stu-id="41081-110">Type</span></span>|<span data-ttu-id="41081-111">説明</span><span class="sxs-lookup"><span data-stu-id="41081-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="41081-112">actionName</span><span class="sxs-lookup"><span data-stu-id="41081-112">actionName</span></span>|<span data-ttu-id="41081-113">String</span><span class="sxs-lookup"><span data-stu-id="41081-113">String</span></span>|<span data-ttu-id="41081-114">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) から継承されるアクション名</span><span class="sxs-lookup"><span data-stu-id="41081-114">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="41081-115">actionState</span><span class="sxs-lookup"><span data-stu-id="41081-115">actionState</span></span>|[<span data-ttu-id="41081-116">actionState</span><span class="sxs-lookup"><span data-stu-id="41081-116">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="41081-117">[deviceactionresult](../resources/intune-devices-deviceactionresult.md)から継承されるアクションの状態。</span><span class="sxs-lookup"><span data-stu-id="41081-117">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="41081-118">可能な値は、`none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported` です。</span><span class="sxs-lookup"><span data-stu-id="41081-118">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="41081-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="41081-119">startDateTime</span></span>|<span data-ttu-id="41081-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="41081-120">DateTimeOffset</span></span>|<span data-ttu-id="41081-121">アクションが開始された時刻 ([deviceActionResult](../resources/intune-devices-deviceactionresult.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="41081-121">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="41081-122">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="41081-122">lastUpdatedDateTime</span></span>|<span data-ttu-id="41081-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="41081-123">DateTimeOffset</span></span>|<span data-ttu-id="41081-124">アクション状態の最終更新時刻 ([deviceActionResult](../resources/intune-devices-deviceactionresult.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="41081-124">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="41081-125">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="41081-125">userPrincipalName</span></span>|<span data-ttu-id="41081-126">String</span><span class="sxs-lookup"><span data-stu-id="41081-126">String</span></span>|<span data-ttu-id="41081-127">削除するユーザーのユーザー プリンシパル名</span><span class="sxs-lookup"><span data-stu-id="41081-127">User principal name of the user to be deleted</span></span>|

## <a name="relationships"></a><span data-ttu-id="41081-128">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="41081-128">Relationships</span></span>
<span data-ttu-id="41081-129">なし</span><span class="sxs-lookup"><span data-stu-id="41081-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="41081-130">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="41081-130">JSON Representation</span></span>
<span data-ttu-id="41081-131">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="41081-131">Here is a JSON representation of the resource.</span></span>
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




