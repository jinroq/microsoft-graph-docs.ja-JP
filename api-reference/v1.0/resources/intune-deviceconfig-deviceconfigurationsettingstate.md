---
title: deviceConfigurationSettingState リソースの種類
description: 指定されたデバイスのデバイス構成設定の状態。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c50ed17421b88f2cb6137458ff853bfa92796c2b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36031669"
---
# <a name="deviceconfigurationsettingstate-resource-type"></a><span data-ttu-id="8a38b-103">deviceConfigurationSettingState リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8a38b-103">deviceConfigurationSettingState resource type</span></span>

> <span data-ttu-id="8a38b-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="8a38b-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8a38b-105">指定されたデバイスのデバイス構成設定の状態。</span><span class="sxs-lookup"><span data-stu-id="8a38b-105">Device Configuration Setting State for a given device.</span></span>

## <a name="properties"></a><span data-ttu-id="8a38b-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8a38b-106">Properties</span></span>
|<span data-ttu-id="8a38b-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8a38b-107">Property</span></span>|<span data-ttu-id="8a38b-108">型</span><span class="sxs-lookup"><span data-stu-id="8a38b-108">Type</span></span>|<span data-ttu-id="8a38b-109">説明</span><span class="sxs-lookup"><span data-stu-id="8a38b-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8a38b-110">setting</span><span class="sxs-lookup"><span data-stu-id="8a38b-110">setting</span></span>|<span data-ttu-id="8a38b-111">String</span><span class="sxs-lookup"><span data-stu-id="8a38b-111">String</span></span>|<span data-ttu-id="8a38b-112">レポートされる設定値。</span><span class="sxs-lookup"><span data-stu-id="8a38b-112">The setting that is being reported</span></span>|
|<span data-ttu-id="8a38b-113">settingName</span><span class="sxs-lookup"><span data-stu-id="8a38b-113">settingName</span></span>|<span data-ttu-id="8a38b-114">String</span><span class="sxs-lookup"><span data-stu-id="8a38b-114">String</span></span>|<span data-ttu-id="8a38b-115">レポートされている、ローカライズされた設定名またはユーザー フレンドリな設定名</span><span class="sxs-lookup"><span data-stu-id="8a38b-115">Localized/user friendly setting name that is being reported</span></span>|
|<span data-ttu-id="8a38b-116">instanceDisplayName</span><span class="sxs-lookup"><span data-stu-id="8a38b-116">instanceDisplayName</span></span>|<span data-ttu-id="8a38b-117">String</span><span class="sxs-lookup"><span data-stu-id="8a38b-117">String</span></span>|<span data-ttu-id="8a38b-118">レポートされている設定インスタンスの名前です。</span><span class="sxs-lookup"><span data-stu-id="8a38b-118">Name of setting instance that is being reported.</span></span>|
|<span data-ttu-id="8a38b-119">state</span><span class="sxs-lookup"><span data-stu-id="8a38b-119">state</span></span>|[<span data-ttu-id="8a38b-120">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="8a38b-120">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="8a38b-121">設定のコンプライアンス状態。</span><span class="sxs-lookup"><span data-stu-id="8a38b-121">The compliance state of the setting.</span></span> <span data-ttu-id="8a38b-122">可能な値は、`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned` です。</span><span class="sxs-lookup"><span data-stu-id="8a38b-122">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="8a38b-123">errorCode</span><span class="sxs-lookup"><span data-stu-id="8a38b-123">errorCode</span></span>|<span data-ttu-id="8a38b-124">Int64</span><span class="sxs-lookup"><span data-stu-id="8a38b-124">Int64</span></span>|<span data-ttu-id="8a38b-125">設定のエラー コード</span><span class="sxs-lookup"><span data-stu-id="8a38b-125">Error code for the setting</span></span>|
|<span data-ttu-id="8a38b-126">errorDescription</span><span class="sxs-lookup"><span data-stu-id="8a38b-126">errorDescription</span></span>|<span data-ttu-id="8a38b-127">String</span><span class="sxs-lookup"><span data-stu-id="8a38b-127">String</span></span>|<span data-ttu-id="8a38b-128">エラーの説明</span><span class="sxs-lookup"><span data-stu-id="8a38b-128">Error description</span></span>|
|<span data-ttu-id="8a38b-129">userId</span><span class="sxs-lookup"><span data-stu-id="8a38b-129">userId</span></span>|<span data-ttu-id="8a38b-130">String</span><span class="sxs-lookup"><span data-stu-id="8a38b-130">String</span></span>|<span data-ttu-id="8a38b-131">UserId</span><span class="sxs-lookup"><span data-stu-id="8a38b-131">UserId</span></span>|
|<span data-ttu-id="8a38b-132">userName</span><span class="sxs-lookup"><span data-stu-id="8a38b-132">userName</span></span>|<span data-ttu-id="8a38b-133">String</span><span class="sxs-lookup"><span data-stu-id="8a38b-133">String</span></span>|<span data-ttu-id="8a38b-134">UserName</span><span class="sxs-lookup"><span data-stu-id="8a38b-134">UserName</span></span>|
|<span data-ttu-id="8a38b-135">userEmail</span><span class="sxs-lookup"><span data-stu-id="8a38b-135">userEmail</span></span>|<span data-ttu-id="8a38b-136">String</span><span class="sxs-lookup"><span data-stu-id="8a38b-136">String</span></span>|<span data-ttu-id="8a38b-137">UserEmail</span><span class="sxs-lookup"><span data-stu-id="8a38b-137">UserEmail</span></span>|
|<span data-ttu-id="8a38b-138">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="8a38b-138">userPrincipalName</span></span>|<span data-ttu-id="8a38b-139">String</span><span class="sxs-lookup"><span data-stu-id="8a38b-139">String</span></span>|<span data-ttu-id="8a38b-140">UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="8a38b-140">UserPrincipalName.</span></span>|
|<span data-ttu-id="8a38b-141">sources</span><span class="sxs-lookup"><span data-stu-id="8a38b-141">sources</span></span>|<span data-ttu-id="8a38b-142">[settingSource](../resources/intune-deviceconfig-settingsource.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="8a38b-142">[settingSource](../resources/intune-deviceconfig-settingsource.md) collection</span></span>|<span data-ttu-id="8a38b-143">投稿ポリシー</span><span class="sxs-lookup"><span data-stu-id="8a38b-143">Contributing policies</span></span>|
|<span data-ttu-id="8a38b-144">currentValue</span><span class="sxs-lookup"><span data-stu-id="8a38b-144">currentValue</span></span>|<span data-ttu-id="8a38b-145">String</span><span class="sxs-lookup"><span data-stu-id="8a38b-145">String</span></span>|<span data-ttu-id="8a38b-146">デバイスに関する設定の現在の値</span><span class="sxs-lookup"><span data-stu-id="8a38b-146">Current value of setting on device</span></span>|

## <a name="relationships"></a><span data-ttu-id="8a38b-147">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="8a38b-147">Relationships</span></span>
<span data-ttu-id="8a38b-148">なし</span><span class="sxs-lookup"><span data-stu-id="8a38b-148">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8a38b-149">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8a38b-149">JSON Representation</span></span>
<span data-ttu-id="8a38b-150">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="8a38b-150">Here is a JSON representation of the resource.</span></span>
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



