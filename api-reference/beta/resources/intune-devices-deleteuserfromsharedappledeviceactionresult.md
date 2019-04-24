---
title: deleteUserFromSharedAppleDeviceActionResult リソースの種類
description: 共有の Apple デバイスのアクションの結果からユーザーを削除する
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 90dec4f79d44d4441d23bdba649ddeb3caa311a7
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32454031"
---
# <a name="deleteuserfromsharedappledeviceactionresult-resource-type"></a><span data-ttu-id="995ec-103">deleteUserFromSharedAppleDeviceActionResult リソースの種類</span><span class="sxs-lookup"><span data-stu-id="995ec-103">deleteUserFromSharedAppleDeviceActionResult resource type</span></span>

> <span data-ttu-id="995ec-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="995ec-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="995ec-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="995ec-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="995ec-106">共有の Apple デバイスのアクションの結果からユーザーを削除する</span><span class="sxs-lookup"><span data-stu-id="995ec-106">Delete user from shared apple device action result</span></span>


<span data-ttu-id="995ec-107">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="995ec-107">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="995ec-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="995ec-108">Properties</span></span>
|<span data-ttu-id="995ec-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="995ec-109">Property</span></span>|<span data-ttu-id="995ec-110">型</span><span class="sxs-lookup"><span data-stu-id="995ec-110">Type</span></span>|<span data-ttu-id="995ec-111">説明</span><span class="sxs-lookup"><span data-stu-id="995ec-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="995ec-112">actionName</span><span class="sxs-lookup"><span data-stu-id="995ec-112">actionName</span></span>|<span data-ttu-id="995ec-113">String</span><span class="sxs-lookup"><span data-stu-id="995ec-113">String</span></span>|<span data-ttu-id="995ec-114">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) から継承されるアクション名</span><span class="sxs-lookup"><span data-stu-id="995ec-114">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="995ec-115">actionState</span><span class="sxs-lookup"><span data-stu-id="995ec-115">actionState</span></span>|[<span data-ttu-id="995ec-116">actionState</span><span class="sxs-lookup"><span data-stu-id="995ec-116">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="995ec-117">[deviceactionresult](../resources/intune-devices-deviceactionresult.md)から継承されるアクションの状態。</span><span class="sxs-lookup"><span data-stu-id="995ec-117">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="995ec-118">可能な値は、`none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported` です。</span><span class="sxs-lookup"><span data-stu-id="995ec-118">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="995ec-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="995ec-119">startDateTime</span></span>|<span data-ttu-id="995ec-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="995ec-120">DateTimeOffset</span></span>|<span data-ttu-id="995ec-121">アクションが開始された時刻。[deviceActionResult](../resources/intune-devices-deviceactionresult.md) から継承。</span><span class="sxs-lookup"><span data-stu-id="995ec-121">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="995ec-122">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="995ec-122">lastUpdatedDateTime</span></span>|<span data-ttu-id="995ec-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="995ec-123">DateTimeOffset</span></span>|<span data-ttu-id="995ec-124">アクション状態の最終更新時刻 ([deviceActionResult](../resources/intune-devices-deviceactionresult.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="995ec-124">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="995ec-125">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="995ec-125">userPrincipalName</span></span>|<span data-ttu-id="995ec-126">String</span><span class="sxs-lookup"><span data-stu-id="995ec-126">String</span></span>|<span data-ttu-id="995ec-127">削除するユーザーのユーザー プリンシパル名</span><span class="sxs-lookup"><span data-stu-id="995ec-127">User principal name of the user to be deleted</span></span>|

## <a name="relationships"></a><span data-ttu-id="995ec-128">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="995ec-128">Relationships</span></span>
<span data-ttu-id="995ec-129">なし</span><span class="sxs-lookup"><span data-stu-id="995ec-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="995ec-130">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="995ec-130">JSON Representation</span></span>
<span data-ttu-id="995ec-131">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="995ec-131">Here is a JSON representation of the resource.</span></span>
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





