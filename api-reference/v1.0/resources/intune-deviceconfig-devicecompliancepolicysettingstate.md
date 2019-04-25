---
title: deviceCompliancePolicySettingState リソースの種類
description: 特定のデバイスに関する、デバイス コンプライアンス ポリシーの設定状態です。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c4d291f84a8c4404ff5b4425680260997b6b452f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32572417"
---
# <a name="devicecompliancepolicysettingstate-resource-type"></a><span data-ttu-id="6a482-103">deviceCompliancePolicySettingState リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6a482-103">deviceCompliancePolicySettingState resource type</span></span>

> <span data-ttu-id="6a482-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="6a482-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6a482-105">特定のデバイスに関する、デバイス コンプライアンス ポリシーの設定状態です。</span><span class="sxs-lookup"><span data-stu-id="6a482-105">Device Compilance Policy Setting State for a given device.</span></span>

## <a name="properties"></a><span data-ttu-id="6a482-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6a482-106">Properties</span></span>
|<span data-ttu-id="6a482-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6a482-107">Property</span></span>|<span data-ttu-id="6a482-108">型</span><span class="sxs-lookup"><span data-stu-id="6a482-108">Type</span></span>|<span data-ttu-id="6a482-109">説明</span><span class="sxs-lookup"><span data-stu-id="6a482-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6a482-110">setting</span><span class="sxs-lookup"><span data-stu-id="6a482-110">setting</span></span>|<span data-ttu-id="6a482-111">String</span><span class="sxs-lookup"><span data-stu-id="6a482-111">String</span></span>|<span data-ttu-id="6a482-112">レポートされる設定値。</span><span class="sxs-lookup"><span data-stu-id="6a482-112">The setting that is being reported</span></span>|
|<span data-ttu-id="6a482-113">settingName</span><span class="sxs-lookup"><span data-stu-id="6a482-113">settingName</span></span>|<span data-ttu-id="6a482-114">String</span><span class="sxs-lookup"><span data-stu-id="6a482-114">String</span></span>|<span data-ttu-id="6a482-115">レポートされている、ローカライズされた設定名またはユーザー フレンドリな設定名</span><span class="sxs-lookup"><span data-stu-id="6a482-115">Localized/user friendly setting name that is being reported</span></span>|
|<span data-ttu-id="6a482-116">instanceDisplayName</span><span class="sxs-lookup"><span data-stu-id="6a482-116">instanceDisplayName</span></span>|<span data-ttu-id="6a482-117">String</span><span class="sxs-lookup"><span data-stu-id="6a482-117">String</span></span>|<span data-ttu-id="6a482-118">レポートされている設定インスタンスの名前です。</span><span class="sxs-lookup"><span data-stu-id="6a482-118">Name of setting instance that is being reported.</span></span>|
|<span data-ttu-id="6a482-119">state</span><span class="sxs-lookup"><span data-stu-id="6a482-119">state</span></span>|[<span data-ttu-id="6a482-120">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="6a482-120">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="6a482-121">設定のコンプライアンス状態。</span><span class="sxs-lookup"><span data-stu-id="6a482-121">The compliance state of the setting.</span></span> <span data-ttu-id="6a482-122">可能な値は、`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned` です。</span><span class="sxs-lookup"><span data-stu-id="6a482-122">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="6a482-123">errorCode</span><span class="sxs-lookup"><span data-stu-id="6a482-123">errorCode</span></span>|<span data-ttu-id="6a482-124">Int64</span><span class="sxs-lookup"><span data-stu-id="6a482-124">Int64</span></span>|<span data-ttu-id="6a482-125">設定のエラー コード</span><span class="sxs-lookup"><span data-stu-id="6a482-125">Error code for the setting</span></span>|
|<span data-ttu-id="6a482-126">errorDescription</span><span class="sxs-lookup"><span data-stu-id="6a482-126">errorDescription</span></span>|<span data-ttu-id="6a482-127">String</span><span class="sxs-lookup"><span data-stu-id="6a482-127">String</span></span>|<span data-ttu-id="6a482-128">エラーの説明</span><span class="sxs-lookup"><span data-stu-id="6a482-128">Error description</span></span>|
|<span data-ttu-id="6a482-129">userId</span><span class="sxs-lookup"><span data-stu-id="6a482-129">userId</span></span>|<span data-ttu-id="6a482-130">String</span><span class="sxs-lookup"><span data-stu-id="6a482-130">String</span></span>|<span data-ttu-id="6a482-131">UserId</span><span class="sxs-lookup"><span data-stu-id="6a482-131">UserId</span></span>|
|<span data-ttu-id="6a482-132">userName</span><span class="sxs-lookup"><span data-stu-id="6a482-132">userName</span></span>|<span data-ttu-id="6a482-133">String</span><span class="sxs-lookup"><span data-stu-id="6a482-133">String</span></span>|<span data-ttu-id="6a482-134">UserName</span><span class="sxs-lookup"><span data-stu-id="6a482-134">UserName</span></span>|
|<span data-ttu-id="6a482-135">userEmail</span><span class="sxs-lookup"><span data-stu-id="6a482-135">userEmail</span></span>|<span data-ttu-id="6a482-136">String</span><span class="sxs-lookup"><span data-stu-id="6a482-136">String</span></span>|<span data-ttu-id="6a482-137">UserEmail</span><span class="sxs-lookup"><span data-stu-id="6a482-137">UserEmail</span></span>|
|<span data-ttu-id="6a482-138">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="6a482-138">userPrincipalName</span></span>|<span data-ttu-id="6a482-139">String</span><span class="sxs-lookup"><span data-stu-id="6a482-139">String</span></span>|<span data-ttu-id="6a482-140">UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="6a482-140">UserPrincipalName.</span></span>|
|<span data-ttu-id="6a482-141">sources</span><span class="sxs-lookup"><span data-stu-id="6a482-141">sources</span></span>|<span data-ttu-id="6a482-142">[settingSource](../resources/intune-deviceconfig-settingsource.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="6a482-142">[settingSource](../resources/intune-deviceconfig-settingsource.md) collection</span></span>|<span data-ttu-id="6a482-143">投稿ポリシー</span><span class="sxs-lookup"><span data-stu-id="6a482-143">Contributing policies</span></span>|
|<span data-ttu-id="6a482-144">currentValue</span><span class="sxs-lookup"><span data-stu-id="6a482-144">currentValue</span></span>|<span data-ttu-id="6a482-145">String</span><span class="sxs-lookup"><span data-stu-id="6a482-145">String</span></span>|<span data-ttu-id="6a482-146">デバイスに関する設定の現在の値</span><span class="sxs-lookup"><span data-stu-id="6a482-146">Current value of setting on device</span></span>|

## <a name="relationships"></a><span data-ttu-id="6a482-147">関係</span><span class="sxs-lookup"><span data-stu-id="6a482-147">Relationships</span></span>
<span data-ttu-id="6a482-148">なし</span><span class="sxs-lookup"><span data-stu-id="6a482-148">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6a482-149">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6a482-149">JSON Representation</span></span>
<span data-ttu-id="6a482-150">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="6a482-150">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceCompliancePolicySettingState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicySettingState",
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



