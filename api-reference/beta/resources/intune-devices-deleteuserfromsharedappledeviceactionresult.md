---
title: deleteUserFromSharedAppleDeviceActionResult リソースの種類
description: 共有の Apple デバイスのアクションの結果からユーザーを削除する
ms.openlocfilehash: 5ed6d7b8c07c28dce5ee8cc830a9e86bcdcafa1b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27069113"
---
# <a name="deleteuserfromsharedappledeviceactionresult-resource-type"></a><span data-ttu-id="f7255-103">deleteUserFromSharedAppleDeviceActionResult リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f7255-103">deleteUserFromSharedAppleDeviceActionResult resource type</span></span>

> <span data-ttu-id="f7255-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="f7255-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f7255-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f7255-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f7255-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="f7255-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f7255-107">共有の Apple デバイスのアクションの結果からユーザーを削除する</span><span class="sxs-lookup"><span data-stu-id="f7255-107">Delete user from shared apple device action result</span></span>

<span data-ttu-id="f7255-108">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f7255-108">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="f7255-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f7255-109">Properties</span></span>
|<span data-ttu-id="f7255-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f7255-110">Property</span></span>|<span data-ttu-id="f7255-111">型</span><span class="sxs-lookup"><span data-stu-id="f7255-111">Type</span></span>|<span data-ttu-id="f7255-112">説明</span><span class="sxs-lookup"><span data-stu-id="f7255-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f7255-113">actionName</span><span class="sxs-lookup"><span data-stu-id="f7255-113">actionName</span></span>|<span data-ttu-id="f7255-114">String</span><span class="sxs-lookup"><span data-stu-id="f7255-114">String</span></span>|<span data-ttu-id="f7255-115">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) から継承されるアクション名</span><span class="sxs-lookup"><span data-stu-id="f7255-115">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="f7255-116">actionState</span><span class="sxs-lookup"><span data-stu-id="f7255-116">actionState</span></span>|[<span data-ttu-id="f7255-117">actionState</span><span class="sxs-lookup"><span data-stu-id="f7255-117">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="f7255-118">[DeviceActionResult](../resources/intune-devices-deviceactionresult.md)から継承される、アクションの状態です。</span><span class="sxs-lookup"><span data-stu-id="f7255-118">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="f7255-119">可能な値は、`none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported` です。</span><span class="sxs-lookup"><span data-stu-id="f7255-119">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="f7255-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="f7255-120">startDateTime</span></span>|<span data-ttu-id="f7255-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f7255-121">DateTimeOffset</span></span>|<span data-ttu-id="f7255-122">アクションが開始された時刻 ([deviceActionResult](../resources/intune-devices-deviceactionresult.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="f7255-122">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="f7255-123">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="f7255-123">lastUpdatedDateTime</span></span>|<span data-ttu-id="f7255-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f7255-124">DateTimeOffset</span></span>|<span data-ttu-id="f7255-125">アクション状態の最終更新時刻 ([deviceActionResult](../resources/intune-devices-deviceactionresult.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="f7255-125">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="f7255-126">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="f7255-126">userPrincipalName</span></span>|<span data-ttu-id="f7255-127">String</span><span class="sxs-lookup"><span data-stu-id="f7255-127">String</span></span>|<span data-ttu-id="f7255-128">削除するユーザーのユーザー プリンシパル名</span><span class="sxs-lookup"><span data-stu-id="f7255-128">User principal name of the user to be deleted</span></span>|

## <a name="relationships"></a><span data-ttu-id="f7255-129">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="f7255-129">Relationships</span></span>
<span data-ttu-id="f7255-130">なし</span><span class="sxs-lookup"><span data-stu-id="f7255-130">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="f7255-131">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f7255-131">JSON Representation</span></span>
<span data-ttu-id="f7255-132">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="f7255-132">Here is a JSON representation of the resource.</span></span>
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





