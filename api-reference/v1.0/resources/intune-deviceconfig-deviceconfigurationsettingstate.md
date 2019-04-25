---
title: deviceConfigurationSettingState リソースの種類
description: 指定されたデバイスのデバイス構成設定の状態。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d79d4c35572c98c82f80f8903d42cfa3b983c2e9
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32573446"
---
# <a name="deviceconfigurationsettingstate-resource-type"></a><span data-ttu-id="b5db4-103">deviceConfigurationSettingState リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b5db4-103">deviceConfigurationSettingState resource type</span></span>

> <span data-ttu-id="b5db4-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="b5db4-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b5db4-105">指定されたデバイスのデバイス構成設定の状態。</span><span class="sxs-lookup"><span data-stu-id="b5db4-105">Device Configuration Setting State for a given device.</span></span>

## <a name="properties"></a><span data-ttu-id="b5db4-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b5db4-106">Properties</span></span>
|<span data-ttu-id="b5db4-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b5db4-107">Property</span></span>|<span data-ttu-id="b5db4-108">型</span><span class="sxs-lookup"><span data-stu-id="b5db4-108">Type</span></span>|<span data-ttu-id="b5db4-109">説明</span><span class="sxs-lookup"><span data-stu-id="b5db4-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b5db4-110">setting</span><span class="sxs-lookup"><span data-stu-id="b5db4-110">setting</span></span>|<span data-ttu-id="b5db4-111">String</span><span class="sxs-lookup"><span data-stu-id="b5db4-111">String</span></span>|<span data-ttu-id="b5db4-112">レポートされる設定値。</span><span class="sxs-lookup"><span data-stu-id="b5db4-112">The setting that is being reported</span></span>|
|<span data-ttu-id="b5db4-113">settingName</span><span class="sxs-lookup"><span data-stu-id="b5db4-113">settingName</span></span>|<span data-ttu-id="b5db4-114">String</span><span class="sxs-lookup"><span data-stu-id="b5db4-114">String</span></span>|<span data-ttu-id="b5db4-115">レポートされている、ローカライズされた設定名またはユーザー フレンドリな設定名</span><span class="sxs-lookup"><span data-stu-id="b5db4-115">Localized/user friendly setting name that is being reported</span></span>|
|<span data-ttu-id="b5db4-116">instanceDisplayName</span><span class="sxs-lookup"><span data-stu-id="b5db4-116">instanceDisplayName</span></span>|<span data-ttu-id="b5db4-117">String</span><span class="sxs-lookup"><span data-stu-id="b5db4-117">String</span></span>|<span data-ttu-id="b5db4-118">レポートされている設定インスタンスの名前です。</span><span class="sxs-lookup"><span data-stu-id="b5db4-118">Name of setting instance that is being reported.</span></span>|
|<span data-ttu-id="b5db4-119">state</span><span class="sxs-lookup"><span data-stu-id="b5db4-119">state</span></span>|[<span data-ttu-id="b5db4-120">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="b5db4-120">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="b5db4-121">設定のコンプライアンス状態。</span><span class="sxs-lookup"><span data-stu-id="b5db4-121">The compliance state of the setting.</span></span> <span data-ttu-id="b5db4-122">可能な値は、`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned` です。</span><span class="sxs-lookup"><span data-stu-id="b5db4-122">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="b5db4-123">errorCode</span><span class="sxs-lookup"><span data-stu-id="b5db4-123">errorCode</span></span>|<span data-ttu-id="b5db4-124">Int64</span><span class="sxs-lookup"><span data-stu-id="b5db4-124">Int64</span></span>|<span data-ttu-id="b5db4-125">設定のエラー コード</span><span class="sxs-lookup"><span data-stu-id="b5db4-125">Error code for the setting</span></span>|
|<span data-ttu-id="b5db4-126">errorDescription</span><span class="sxs-lookup"><span data-stu-id="b5db4-126">errorDescription</span></span>|<span data-ttu-id="b5db4-127">String</span><span class="sxs-lookup"><span data-stu-id="b5db4-127">String</span></span>|<span data-ttu-id="b5db4-128">エラーの説明</span><span class="sxs-lookup"><span data-stu-id="b5db4-128">Error description</span></span>|
|<span data-ttu-id="b5db4-129">userId</span><span class="sxs-lookup"><span data-stu-id="b5db4-129">userId</span></span>|<span data-ttu-id="b5db4-130">String</span><span class="sxs-lookup"><span data-stu-id="b5db4-130">String</span></span>|<span data-ttu-id="b5db4-131">UserId</span><span class="sxs-lookup"><span data-stu-id="b5db4-131">UserId</span></span>|
|<span data-ttu-id="b5db4-132">userName</span><span class="sxs-lookup"><span data-stu-id="b5db4-132">userName</span></span>|<span data-ttu-id="b5db4-133">String</span><span class="sxs-lookup"><span data-stu-id="b5db4-133">String</span></span>|<span data-ttu-id="b5db4-134">UserName</span><span class="sxs-lookup"><span data-stu-id="b5db4-134">UserName</span></span>|
|<span data-ttu-id="b5db4-135">userEmail</span><span class="sxs-lookup"><span data-stu-id="b5db4-135">userEmail</span></span>|<span data-ttu-id="b5db4-136">String</span><span class="sxs-lookup"><span data-stu-id="b5db4-136">String</span></span>|<span data-ttu-id="b5db4-137">UserEmail</span><span class="sxs-lookup"><span data-stu-id="b5db4-137">UserEmail</span></span>|
|<span data-ttu-id="b5db4-138">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="b5db4-138">userPrincipalName</span></span>|<span data-ttu-id="b5db4-139">String</span><span class="sxs-lookup"><span data-stu-id="b5db4-139">String</span></span>|<span data-ttu-id="b5db4-140">UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="b5db4-140">UserPrincipalName.</span></span>|
|<span data-ttu-id="b5db4-141">sources</span><span class="sxs-lookup"><span data-stu-id="b5db4-141">sources</span></span>|<span data-ttu-id="b5db4-142">[settingSource](../resources/intune-deviceconfig-settingsource.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="b5db4-142">[settingSource](../resources/intune-deviceconfig-settingsource.md) collection</span></span>|<span data-ttu-id="b5db4-143">投稿ポリシー</span><span class="sxs-lookup"><span data-stu-id="b5db4-143">Contributing policies</span></span>|
|<span data-ttu-id="b5db4-144">currentValue</span><span class="sxs-lookup"><span data-stu-id="b5db4-144">currentValue</span></span>|<span data-ttu-id="b5db4-145">String</span><span class="sxs-lookup"><span data-stu-id="b5db4-145">String</span></span>|<span data-ttu-id="b5db4-146">デバイスに関する設定の現在の値</span><span class="sxs-lookup"><span data-stu-id="b5db4-146">Current value of setting on device</span></span>|

## <a name="relationships"></a><span data-ttu-id="b5db4-147">関係</span><span class="sxs-lookup"><span data-stu-id="b5db4-147">Relationships</span></span>
<span data-ttu-id="b5db4-148">なし</span><span class="sxs-lookup"><span data-stu-id="b5db4-148">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b5db4-149">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b5db4-149">JSON Representation</span></span>
<span data-ttu-id="b5db4-150">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="b5db4-150">Here is a JSON representation of the resource.</span></span>
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



