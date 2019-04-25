---
title: deviceCompliancePolicySettingState リソースの種類
description: 特定のデバイスに関する、デバイス コンプライアンス ポリシーの設定状態です。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b6c204294190f2f585ad19f7cad4f68e2f7fcc03
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32565822"
---
# <a name="devicecompliancepolicysettingstate-resource-type"></a><span data-ttu-id="7038b-103">deviceCompliancePolicySettingState リソースの種類</span><span class="sxs-lookup"><span data-stu-id="7038b-103">deviceCompliancePolicySettingState resource type</span></span>

> <span data-ttu-id="7038b-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7038b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7038b-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="7038b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7038b-106">特定のデバイスに関する、デバイス コンプライアンス ポリシーの設定状態です。</span><span class="sxs-lookup"><span data-stu-id="7038b-106">Device Compilance Policy Setting State for a given device.</span></span>

## <a name="properties"></a><span data-ttu-id="7038b-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7038b-107">Properties</span></span>
|<span data-ttu-id="7038b-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7038b-108">Property</span></span>|<span data-ttu-id="7038b-109">型</span><span class="sxs-lookup"><span data-stu-id="7038b-109">Type</span></span>|<span data-ttu-id="7038b-110">説明</span><span class="sxs-lookup"><span data-stu-id="7038b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7038b-111">setting</span><span class="sxs-lookup"><span data-stu-id="7038b-111">setting</span></span>|<span data-ttu-id="7038b-112">String</span><span class="sxs-lookup"><span data-stu-id="7038b-112">String</span></span>|<span data-ttu-id="7038b-113">レポートされる設定値。</span><span class="sxs-lookup"><span data-stu-id="7038b-113">The setting that is being reported</span></span>|
|<span data-ttu-id="7038b-114">settingName</span><span class="sxs-lookup"><span data-stu-id="7038b-114">settingName</span></span>|<span data-ttu-id="7038b-115">String</span><span class="sxs-lookup"><span data-stu-id="7038b-115">String</span></span>|<span data-ttu-id="7038b-116">レポートされている、ローカライズされた設定名またはユーザー フレンドリな設定名</span><span class="sxs-lookup"><span data-stu-id="7038b-116">Localized/user friendly setting name that is being reported</span></span>|
|<span data-ttu-id="7038b-117">instanceDisplayName</span><span class="sxs-lookup"><span data-stu-id="7038b-117">instanceDisplayName</span></span>|<span data-ttu-id="7038b-118">String</span><span class="sxs-lookup"><span data-stu-id="7038b-118">String</span></span>|<span data-ttu-id="7038b-119">レポートされている設定インスタンスの名前です。</span><span class="sxs-lookup"><span data-stu-id="7038b-119">Name of setting instance that is being reported.</span></span>|
|<span data-ttu-id="7038b-120">state</span><span class="sxs-lookup"><span data-stu-id="7038b-120">state</span></span>|[<span data-ttu-id="7038b-121">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="7038b-121">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="7038b-122">設定のコンプライアンス状態。</span><span class="sxs-lookup"><span data-stu-id="7038b-122">The compliance state of the setting.</span></span> <span data-ttu-id="7038b-123">可能な値は、`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned` です。</span><span class="sxs-lookup"><span data-stu-id="7038b-123">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="7038b-124">errorCode</span><span class="sxs-lookup"><span data-stu-id="7038b-124">errorCode</span></span>|<span data-ttu-id="7038b-125">Int64</span><span class="sxs-lookup"><span data-stu-id="7038b-125">Int64</span></span>|<span data-ttu-id="7038b-126">設定のエラー コード</span><span class="sxs-lookup"><span data-stu-id="7038b-126">Error code for the setting</span></span>|
|<span data-ttu-id="7038b-127">errorDescription</span><span class="sxs-lookup"><span data-stu-id="7038b-127">errorDescription</span></span>|<span data-ttu-id="7038b-128">String</span><span class="sxs-lookup"><span data-stu-id="7038b-128">String</span></span>|<span data-ttu-id="7038b-129">エラーの説明</span><span class="sxs-lookup"><span data-stu-id="7038b-129">Error description</span></span>|
|<span data-ttu-id="7038b-130">userId</span><span class="sxs-lookup"><span data-stu-id="7038b-130">userId</span></span>|<span data-ttu-id="7038b-131">String</span><span class="sxs-lookup"><span data-stu-id="7038b-131">String</span></span>|<span data-ttu-id="7038b-132">UserId</span><span class="sxs-lookup"><span data-stu-id="7038b-132">UserId</span></span>|
|<span data-ttu-id="7038b-133">userName</span><span class="sxs-lookup"><span data-stu-id="7038b-133">userName</span></span>|<span data-ttu-id="7038b-134">String</span><span class="sxs-lookup"><span data-stu-id="7038b-134">String</span></span>|<span data-ttu-id="7038b-135">UserName</span><span class="sxs-lookup"><span data-stu-id="7038b-135">UserName</span></span>|
|<span data-ttu-id="7038b-136">userEmail</span><span class="sxs-lookup"><span data-stu-id="7038b-136">userEmail</span></span>|<span data-ttu-id="7038b-137">String</span><span class="sxs-lookup"><span data-stu-id="7038b-137">String</span></span>|<span data-ttu-id="7038b-138">UserEmail</span><span class="sxs-lookup"><span data-stu-id="7038b-138">UserEmail</span></span>|
|<span data-ttu-id="7038b-139">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="7038b-139">userPrincipalName</span></span>|<span data-ttu-id="7038b-140">String</span><span class="sxs-lookup"><span data-stu-id="7038b-140">String</span></span>|<span data-ttu-id="7038b-141">UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="7038b-141">UserPrincipalName.</span></span>|
|<span data-ttu-id="7038b-142">sources</span><span class="sxs-lookup"><span data-stu-id="7038b-142">sources</span></span>|<span data-ttu-id="7038b-143">[settingSource](../resources/intune-deviceconfig-settingsource.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="7038b-143">[settingSource](../resources/intune-deviceconfig-settingsource.md) collection</span></span>|<span data-ttu-id="7038b-144">投稿ポリシー</span><span class="sxs-lookup"><span data-stu-id="7038b-144">Contributing policies</span></span>|
|<span data-ttu-id="7038b-145">currentValue</span><span class="sxs-lookup"><span data-stu-id="7038b-145">currentValue</span></span>|<span data-ttu-id="7038b-146">String</span><span class="sxs-lookup"><span data-stu-id="7038b-146">String</span></span>|<span data-ttu-id="7038b-147">デバイスに関する設定の現在の値</span><span class="sxs-lookup"><span data-stu-id="7038b-147">Current value of setting on device</span></span>|

## <a name="relationships"></a><span data-ttu-id="7038b-148">関係</span><span class="sxs-lookup"><span data-stu-id="7038b-148">Relationships</span></span>
<span data-ttu-id="7038b-149">なし</span><span class="sxs-lookup"><span data-stu-id="7038b-149">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7038b-150">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="7038b-150">JSON Representation</span></span>
<span data-ttu-id="7038b-151">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="7038b-151">Here is a JSON representation of the resource.</span></span>
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





