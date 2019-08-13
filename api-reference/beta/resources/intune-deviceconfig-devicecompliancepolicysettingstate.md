---
title: deviceCompliancePolicySettingState リソースの種類
description: 特定のデバイスに関する、デバイス コンプライアンス ポリシーの設定状態です。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 27288df13fecbe7cc85b455d1df30b4885b17eec
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36333101"
---
# <a name="devicecompliancepolicysettingstate-resource-type"></a><span data-ttu-id="4c89f-103">deviceCompliancePolicySettingState リソースの種類</span><span class="sxs-lookup"><span data-stu-id="4c89f-103">deviceCompliancePolicySettingState resource type</span></span>

> <span data-ttu-id="4c89f-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4c89f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4c89f-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="4c89f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4c89f-106">特定のデバイスに関する、デバイス コンプライアンス ポリシーの設定状態です。</span><span class="sxs-lookup"><span data-stu-id="4c89f-106">Device Compilance Policy Setting State for a given device.</span></span>

## <a name="properties"></a><span data-ttu-id="4c89f-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4c89f-107">Properties</span></span>
|<span data-ttu-id="4c89f-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4c89f-108">Property</span></span>|<span data-ttu-id="4c89f-109">型</span><span class="sxs-lookup"><span data-stu-id="4c89f-109">Type</span></span>|<span data-ttu-id="4c89f-110">説明</span><span class="sxs-lookup"><span data-stu-id="4c89f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4c89f-111">setting</span><span class="sxs-lookup"><span data-stu-id="4c89f-111">setting</span></span>|<span data-ttu-id="4c89f-112">String</span><span class="sxs-lookup"><span data-stu-id="4c89f-112">String</span></span>|<span data-ttu-id="4c89f-113">レポートされる設定値。</span><span class="sxs-lookup"><span data-stu-id="4c89f-113">The setting that is being reported</span></span>|
|<span data-ttu-id="4c89f-114">settingName</span><span class="sxs-lookup"><span data-stu-id="4c89f-114">settingName</span></span>|<span data-ttu-id="4c89f-115">String</span><span class="sxs-lookup"><span data-stu-id="4c89f-115">String</span></span>|<span data-ttu-id="4c89f-116">レポートされている、ローカライズされた設定名またはユーザー フレンドリな設定名</span><span class="sxs-lookup"><span data-stu-id="4c89f-116">Localized/user friendly setting name that is being reported</span></span>|
|<span data-ttu-id="4c89f-117">instanceDisplayName</span><span class="sxs-lookup"><span data-stu-id="4c89f-117">instanceDisplayName</span></span>|<span data-ttu-id="4c89f-118">String</span><span class="sxs-lookup"><span data-stu-id="4c89f-118">String</span></span>|<span data-ttu-id="4c89f-119">レポートされている設定インスタンスの名前です。</span><span class="sxs-lookup"><span data-stu-id="4c89f-119">Name of setting instance that is being reported.</span></span>|
|<span data-ttu-id="4c89f-120">state</span><span class="sxs-lookup"><span data-stu-id="4c89f-120">state</span></span>|[<span data-ttu-id="4c89f-121">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="4c89f-121">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="4c89f-122">設定のコンプライアンス状態。</span><span class="sxs-lookup"><span data-stu-id="4c89f-122">The compliance state of the setting.</span></span> <span data-ttu-id="4c89f-123">可能な値は、`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned` です。</span><span class="sxs-lookup"><span data-stu-id="4c89f-123">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="4c89f-124">errorCode</span><span class="sxs-lookup"><span data-stu-id="4c89f-124">errorCode</span></span>|<span data-ttu-id="4c89f-125">Int64</span><span class="sxs-lookup"><span data-stu-id="4c89f-125">Int64</span></span>|<span data-ttu-id="4c89f-126">設定のエラー コード</span><span class="sxs-lookup"><span data-stu-id="4c89f-126">Error code for the setting</span></span>|
|<span data-ttu-id="4c89f-127">errorDescription</span><span class="sxs-lookup"><span data-stu-id="4c89f-127">errorDescription</span></span>|<span data-ttu-id="4c89f-128">String</span><span class="sxs-lookup"><span data-stu-id="4c89f-128">String</span></span>|<span data-ttu-id="4c89f-129">エラーの説明</span><span class="sxs-lookup"><span data-stu-id="4c89f-129">Error description</span></span>|
|<span data-ttu-id="4c89f-130">userId</span><span class="sxs-lookup"><span data-stu-id="4c89f-130">userId</span></span>|<span data-ttu-id="4c89f-131">String</span><span class="sxs-lookup"><span data-stu-id="4c89f-131">String</span></span>|<span data-ttu-id="4c89f-132">UserId</span><span class="sxs-lookup"><span data-stu-id="4c89f-132">UserId</span></span>|
|<span data-ttu-id="4c89f-133">userName</span><span class="sxs-lookup"><span data-stu-id="4c89f-133">userName</span></span>|<span data-ttu-id="4c89f-134">String</span><span class="sxs-lookup"><span data-stu-id="4c89f-134">String</span></span>|<span data-ttu-id="4c89f-135">UserName</span><span class="sxs-lookup"><span data-stu-id="4c89f-135">UserName</span></span>|
|<span data-ttu-id="4c89f-136">userEmail</span><span class="sxs-lookup"><span data-stu-id="4c89f-136">userEmail</span></span>|<span data-ttu-id="4c89f-137">String</span><span class="sxs-lookup"><span data-stu-id="4c89f-137">String</span></span>|<span data-ttu-id="4c89f-138">UserEmail</span><span class="sxs-lookup"><span data-stu-id="4c89f-138">UserEmail</span></span>|
|<span data-ttu-id="4c89f-139">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="4c89f-139">userPrincipalName</span></span>|<span data-ttu-id="4c89f-140">String</span><span class="sxs-lookup"><span data-stu-id="4c89f-140">String</span></span>|<span data-ttu-id="4c89f-141">UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="4c89f-141">UserPrincipalName.</span></span>|
|<span data-ttu-id="4c89f-142">sources</span><span class="sxs-lookup"><span data-stu-id="4c89f-142">sources</span></span>|<span data-ttu-id="4c89f-143">[settingSource](../resources/intune-deviceconfig-settingsource.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="4c89f-143">[settingSource](../resources/intune-deviceconfig-settingsource.md) collection</span></span>|<span data-ttu-id="4c89f-144">投稿ポリシー</span><span class="sxs-lookup"><span data-stu-id="4c89f-144">Contributing policies</span></span>|
|<span data-ttu-id="4c89f-145">currentValue</span><span class="sxs-lookup"><span data-stu-id="4c89f-145">currentValue</span></span>|<span data-ttu-id="4c89f-146">String</span><span class="sxs-lookup"><span data-stu-id="4c89f-146">String</span></span>|<span data-ttu-id="4c89f-147">デバイスに関する設定の現在の値</span><span class="sxs-lookup"><span data-stu-id="4c89f-147">Current value of setting on device</span></span>|

## <a name="relationships"></a><span data-ttu-id="4c89f-148">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="4c89f-148">Relationships</span></span>
<span data-ttu-id="4c89f-149">なし</span><span class="sxs-lookup"><span data-stu-id="4c89f-149">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4c89f-150">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="4c89f-150">JSON Representation</span></span>
<span data-ttu-id="4c89f-151">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="4c89f-151">Here is a JSON representation of the resource.</span></span>
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



