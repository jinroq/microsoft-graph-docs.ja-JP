---
title: deviceConfigurationSettingState リソースの種類
description: 指定されたデバイスのデバイス構成設定の状態。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d79d4c35572c98c82f80f8903d42cfa3b983c2e9
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30252904"
---
# <a name="deviceconfigurationsettingstate-resource-type"></a><span data-ttu-id="7094f-103">deviceConfigurationSettingState リソースの種類</span><span class="sxs-lookup"><span data-stu-id="7094f-103">deviceConfigurationSettingState resource type</span></span>

> <span data-ttu-id="7094f-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="7094f-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7094f-105">指定されたデバイスのデバイス構成設定の状態。</span><span class="sxs-lookup"><span data-stu-id="7094f-105">Device Configuration Setting State for a given device.</span></span>

## <a name="properties"></a><span data-ttu-id="7094f-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7094f-106">Properties</span></span>
|<span data-ttu-id="7094f-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7094f-107">Property</span></span>|<span data-ttu-id="7094f-108">型</span><span class="sxs-lookup"><span data-stu-id="7094f-108">Type</span></span>|<span data-ttu-id="7094f-109">説明</span><span class="sxs-lookup"><span data-stu-id="7094f-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7094f-110">setting</span><span class="sxs-lookup"><span data-stu-id="7094f-110">setting</span></span>|<span data-ttu-id="7094f-111">String</span><span class="sxs-lookup"><span data-stu-id="7094f-111">String</span></span>|<span data-ttu-id="7094f-112">レポートされている設定値です。</span><span class="sxs-lookup"><span data-stu-id="7094f-112">The setting that is being reported</span></span>|
|<span data-ttu-id="7094f-113">settingName</span><span class="sxs-lookup"><span data-stu-id="7094f-113">settingName</span></span>|<span data-ttu-id="7094f-114">String</span><span class="sxs-lookup"><span data-stu-id="7094f-114">String</span></span>|<span data-ttu-id="7094f-115">レポートされている、ローカライズされた設定名またはユーザー フレンドリな設定名です</span><span class="sxs-lookup"><span data-stu-id="7094f-115">Localized/user friendly setting name that is being reported</span></span>|
|<span data-ttu-id="7094f-116">instanceDisplayName</span><span class="sxs-lookup"><span data-stu-id="7094f-116">instanceDisplayName</span></span>|<span data-ttu-id="7094f-117">String</span><span class="sxs-lookup"><span data-stu-id="7094f-117">String</span></span>|<span data-ttu-id="7094f-118">レポートされている設定インスタンスの名前です。</span><span class="sxs-lookup"><span data-stu-id="7094f-118">Name of setting instance that is being reported.</span></span>|
|<span data-ttu-id="7094f-119">state</span><span class="sxs-lookup"><span data-stu-id="7094f-119">state</span></span>|[<span data-ttu-id="7094f-120">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="7094f-120">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="7094f-121">設定のコンプライアンス状態。</span><span class="sxs-lookup"><span data-stu-id="7094f-121">The compliance state of the setting.</span></span> <span data-ttu-id="7094f-122">可能な値は、`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned` です。</span><span class="sxs-lookup"><span data-stu-id="7094f-122">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="7094f-123">errorCode</span><span class="sxs-lookup"><span data-stu-id="7094f-123">errorCode</span></span>|<span data-ttu-id="7094f-124">Int64</span><span class="sxs-lookup"><span data-stu-id="7094f-124">Int64</span></span>|<span data-ttu-id="7094f-125">設定のエラー コード</span><span class="sxs-lookup"><span data-stu-id="7094f-125">Error code for the setting</span></span>|
|<span data-ttu-id="7094f-126">errorDescription</span><span class="sxs-lookup"><span data-stu-id="7094f-126">errorDescription</span></span>|<span data-ttu-id="7094f-127">String</span><span class="sxs-lookup"><span data-stu-id="7094f-127">String</span></span>|<span data-ttu-id="7094f-128">エラーの説明</span><span class="sxs-lookup"><span data-stu-id="7094f-128">Error description</span></span>|
|<span data-ttu-id="7094f-129">userId</span><span class="sxs-lookup"><span data-stu-id="7094f-129">userId</span></span>|<span data-ttu-id="7094f-130">String</span><span class="sxs-lookup"><span data-stu-id="7094f-130">String</span></span>|<span data-ttu-id="7094f-131">UserId</span><span class="sxs-lookup"><span data-stu-id="7094f-131">UserId</span></span>|
|<span data-ttu-id="7094f-132">userName</span><span class="sxs-lookup"><span data-stu-id="7094f-132">userName</span></span>|<span data-ttu-id="7094f-133">String</span><span class="sxs-lookup"><span data-stu-id="7094f-133">String</span></span>|<span data-ttu-id="7094f-134">UserName</span><span class="sxs-lookup"><span data-stu-id="7094f-134">UserName</span></span>|
|<span data-ttu-id="7094f-135">userEmail</span><span class="sxs-lookup"><span data-stu-id="7094f-135">userEmail</span></span>|<span data-ttu-id="7094f-136">String</span><span class="sxs-lookup"><span data-stu-id="7094f-136">String</span></span>|<span data-ttu-id="7094f-137">UserEmail</span><span class="sxs-lookup"><span data-stu-id="7094f-137">UserEmail</span></span>|
|<span data-ttu-id="7094f-138">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="7094f-138">userPrincipalName</span></span>|<span data-ttu-id="7094f-139">String</span><span class="sxs-lookup"><span data-stu-id="7094f-139">String</span></span>|<span data-ttu-id="7094f-140">UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="7094f-140">UserPrincipalName.</span></span>|
|<span data-ttu-id="7094f-141">ソース</span><span class="sxs-lookup"><span data-stu-id="7094f-141">sources</span></span>|<span data-ttu-id="7094f-142">[settingSource](../resources/intune-deviceconfig-settingsource.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="7094f-142">[settingSource](../resources/intune-deviceconfig-settingsource.md) collection</span></span>|<span data-ttu-id="7094f-143">投稿ポリシー</span><span class="sxs-lookup"><span data-stu-id="7094f-143">Contributing policies</span></span>|
|<span data-ttu-id="7094f-144">currentValue</span><span class="sxs-lookup"><span data-stu-id="7094f-144">currentValue</span></span>|<span data-ttu-id="7094f-145">String</span><span class="sxs-lookup"><span data-stu-id="7094f-145">String</span></span>|<span data-ttu-id="7094f-146">デバイスに関する設定の現在の値</span><span class="sxs-lookup"><span data-stu-id="7094f-146">Current value of setting on device</span></span>|

## <a name="relationships"></a><span data-ttu-id="7094f-147">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="7094f-147">Relationships</span></span>
<span data-ttu-id="7094f-148">なし</span><span class="sxs-lookup"><span data-stu-id="7094f-148">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7094f-149">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="7094f-149">JSON Representation</span></span>
<span data-ttu-id="7094f-150">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="7094f-150">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceConfigurationSettingState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceConfigurationSettingState",
  "setting": "String",
  "settingName": "String",
  "instanceDisplayName": "String",
  "state": "String",
  "errorCode": 1024,
  "errorDescription": "String",
  "userId": "String",
  "userName": "String",
  "userEmail": "String",
  "userPrincipalName": "String",
  "sources": [
    {
      "@odata.type": "microsoft.graph.settingSource",
      "id": "String",
      "displayName": "String"
    }
  ],
  "currentValue": "String"
}
```



