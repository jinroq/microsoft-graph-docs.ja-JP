---
title: deleteUserFromSharedAppleDeviceActionResult リソースの種類
description: 共有の Apple デバイスのアクションの結果からユーザーを削除する
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: ed004ad8c02d18c19df7be0f819658603fb4fc0d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27861909"
---
# <a name="deleteuserfromsharedappledeviceactionresult-resource-type"></a><span data-ttu-id="68146-103">deleteUserFromSharedAppleDeviceActionResult リソースの種類</span><span class="sxs-lookup"><span data-stu-id="68146-103">deleteUserFromSharedAppleDeviceActionResult resource type</span></span>

> <span data-ttu-id="68146-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="68146-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="68146-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="68146-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="68146-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="68146-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="68146-107">共有の Apple デバイスのアクションの結果からユーザーを削除する</span><span class="sxs-lookup"><span data-stu-id="68146-107">Delete user from shared apple device action result</span></span>

<span data-ttu-id="68146-108">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="68146-108">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="68146-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="68146-109">Properties</span></span>
|<span data-ttu-id="68146-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="68146-110">Property</span></span>|<span data-ttu-id="68146-111">種類</span><span class="sxs-lookup"><span data-stu-id="68146-111">Type</span></span>|<span data-ttu-id="68146-112">説明</span><span class="sxs-lookup"><span data-stu-id="68146-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="68146-113">actionName</span><span class="sxs-lookup"><span data-stu-id="68146-113">actionName</span></span>|<span data-ttu-id="68146-114">String</span><span class="sxs-lookup"><span data-stu-id="68146-114">String</span></span>|<span data-ttu-id="68146-115">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) から継承されるアクション名</span><span class="sxs-lookup"><span data-stu-id="68146-115">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="68146-116">actionState</span><span class="sxs-lookup"><span data-stu-id="68146-116">actionState</span></span>|[<span data-ttu-id="68146-117">actionState</span><span class="sxs-lookup"><span data-stu-id="68146-117">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="68146-118">[DeviceActionResult](../resources/intune-devices-deviceactionresult.md)から継承される、アクションの状態です。</span><span class="sxs-lookup"><span data-stu-id="68146-118">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="68146-119">可能な値は、`none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported` です。</span><span class="sxs-lookup"><span data-stu-id="68146-119">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="68146-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="68146-120">startDateTime</span></span>|<span data-ttu-id="68146-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="68146-121">DateTimeOffset</span></span>|<span data-ttu-id="68146-122">アクションが開始された時刻 ([deviceActionResult](../resources/intune-devices-deviceactionresult.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="68146-122">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="68146-123">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="68146-123">lastUpdatedDateTime</span></span>|<span data-ttu-id="68146-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="68146-124">DateTimeOffset</span></span>|<span data-ttu-id="68146-125">アクション状態の最終更新時刻 ([deviceActionResult](../resources/intune-devices-deviceactionresult.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="68146-125">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="68146-126">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="68146-126">userPrincipalName</span></span>|<span data-ttu-id="68146-127">String</span><span class="sxs-lookup"><span data-stu-id="68146-127">String</span></span>|<span data-ttu-id="68146-128">削除するユーザーのユーザー プリンシパル名</span><span class="sxs-lookup"><span data-stu-id="68146-128">User principal name of the user to be deleted</span></span>|

## <a name="relationships"></a><span data-ttu-id="68146-129">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="68146-129">Relationships</span></span>
<span data-ttu-id="68146-130">なし</span><span class="sxs-lookup"><span data-stu-id="68146-130">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="68146-131">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="68146-131">JSON Representation</span></span>
<span data-ttu-id="68146-132">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="68146-132">Here is a JSON representation of the resource.</span></span>
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





