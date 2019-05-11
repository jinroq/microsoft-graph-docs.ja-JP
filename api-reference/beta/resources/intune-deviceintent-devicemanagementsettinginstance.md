---
title: deviceManagementSettingInstance リソースの種類
description: 設定インスタンスの基本型
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b780fad1df833a1a5d431835364493ac5afc3c6b
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33943334"
---
# <a name="devicemanagementsettinginstance-resource-type"></a><span data-ttu-id="dc478-103">deviceManagementSettingInstance リソースの種類</span><span class="sxs-lookup"><span data-stu-id="dc478-103">deviceManagementSettingInstance resource type</span></span>

> <span data-ttu-id="dc478-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dc478-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dc478-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="dc478-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dc478-106">設定インスタンスの基本型</span><span class="sxs-lookup"><span data-stu-id="dc478-106">Base type for a setting instance</span></span>

## <a name="methods"></a><span data-ttu-id="dc478-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="dc478-107">Methods</span></span>
|<span data-ttu-id="dc478-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="dc478-108">Method</span></span>|<span data-ttu-id="dc478-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="dc478-109">Return Type</span></span>|<span data-ttu-id="dc478-110">説明</span><span class="sxs-lookup"><span data-stu-id="dc478-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="dc478-111">DeviceManagementSettingInstances を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="dc478-111">List deviceManagementSettingInstances</span></span>](../api/intune-deviceintent-devicemanagementsettinginstance-list.md)|<span data-ttu-id="dc478-112">[Devicemanagementsettinginstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="dc478-112">[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md) collection</span></span>|<span data-ttu-id="dc478-113">[Devicemanagementsettinginstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="dc478-113">List properties and relationships of the [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md) objects.</span></span>|
|[<span data-ttu-id="dc478-114">DeviceManagementSettingInstance を取得する</span><span class="sxs-lookup"><span data-stu-id="dc478-114">Get deviceManagementSettingInstance</span></span>](../api/intune-deviceintent-devicemanagementsettinginstance-get.md)|[<span data-ttu-id="dc478-115">deviceManagementSettingInstance</span><span class="sxs-lookup"><span data-stu-id="dc478-115">deviceManagementSettingInstance</span></span>](../resources/intune-deviceintent-devicemanagementsettinginstance.md)|<span data-ttu-id="dc478-116">[Devicemanagementsettinginstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="dc478-116">Read properties and relationships of the [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="dc478-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="dc478-117">Properties</span></span>
|<span data-ttu-id="dc478-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="dc478-118">Property</span></span>|<span data-ttu-id="dc478-119">型</span><span class="sxs-lookup"><span data-stu-id="dc478-119">Type</span></span>|<span data-ttu-id="dc478-120">説明</span><span class="sxs-lookup"><span data-stu-id="dc478-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dc478-121">id</span><span class="sxs-lookup"><span data-stu-id="dc478-121">id</span></span>|<span data-ttu-id="dc478-122">String</span><span class="sxs-lookup"><span data-stu-id="dc478-122">String</span></span>|<span data-ttu-id="dc478-123">設定インスタンス ID</span><span class="sxs-lookup"><span data-stu-id="dc478-123">The setting instance ID</span></span>|
|<span data-ttu-id="dc478-124">definitionId</span><span class="sxs-lookup"><span data-stu-id="dc478-124">definitionId</span></span>|<span data-ttu-id="dc478-125">String</span><span class="sxs-lookup"><span data-stu-id="dc478-125">String</span></span>|<span data-ttu-id="dc478-126">このインスタンスの設定定義の ID</span><span class="sxs-lookup"><span data-stu-id="dc478-126">The ID of the setting definition for this instance</span></span>|
|<span data-ttu-id="dc478-127">valueJson</span><span class="sxs-lookup"><span data-stu-id="dc478-127">valueJson</span></span>|<span data-ttu-id="dc478-128">String</span><span class="sxs-lookup"><span data-stu-id="dc478-128">String</span></span>|<span data-ttu-id="dc478-129">値の JSON 表現</span><span class="sxs-lookup"><span data-stu-id="dc478-129">JSON representation of the value</span></span>|

## <a name="relationships"></a><span data-ttu-id="dc478-130">関係</span><span class="sxs-lookup"><span data-stu-id="dc478-130">Relationships</span></span>
<span data-ttu-id="dc478-131">なし</span><span class="sxs-lookup"><span data-stu-id="dc478-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="dc478-132">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="dc478-132">JSON Representation</span></span>
<span data-ttu-id="dc478-133">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="dc478-133">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementSettingInstance"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementSettingInstance",
  "id": "String (identifier)",
  "definitionId": "String",
  "valueJson": "String"
}
```




