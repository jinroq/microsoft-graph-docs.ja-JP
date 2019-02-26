---
title: deviceConfigurationSettingState リソースの種類
description: 指定されたデバイスのデバイス構成設定の状態。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0acfcd697815ee9403e6144c5da34dd824022de3
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30165885"
---
# <a name="deviceconfigurationsettingstate-resource-type"></a><span data-ttu-id="f1608-103">deviceConfigurationSettingState リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f1608-103">deviceConfigurationSettingState resource type</span></span>

> <span data-ttu-id="f1608-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f1608-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f1608-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="f1608-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f1608-106">指定されたデバイスのデバイス構成設定の状態。</span><span class="sxs-lookup"><span data-stu-id="f1608-106">Device Configuration Setting State for a given device.</span></span>

## <a name="properties"></a><span data-ttu-id="f1608-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f1608-107">Properties</span></span>
|<span data-ttu-id="f1608-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f1608-108">Property</span></span>|<span data-ttu-id="f1608-109">型</span><span class="sxs-lookup"><span data-stu-id="f1608-109">Type</span></span>|<span data-ttu-id="f1608-110">説明</span><span class="sxs-lookup"><span data-stu-id="f1608-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f1608-111">setting</span><span class="sxs-lookup"><span data-stu-id="f1608-111">setting</span></span>|<span data-ttu-id="f1608-112">String</span><span class="sxs-lookup"><span data-stu-id="f1608-112">String</span></span>|<span data-ttu-id="f1608-113">レポートされている設定値です。</span><span class="sxs-lookup"><span data-stu-id="f1608-113">The setting that is being reported</span></span>|
|<span data-ttu-id="f1608-114">settingName</span><span class="sxs-lookup"><span data-stu-id="f1608-114">settingName</span></span>|<span data-ttu-id="f1608-115">String</span><span class="sxs-lookup"><span data-stu-id="f1608-115">String</span></span>|<span data-ttu-id="f1608-116">レポートされている、ローカライズされた設定名またはユーザー フレンドリな設定名です</span><span class="sxs-lookup"><span data-stu-id="f1608-116">Localized/user friendly setting name that is being reported</span></span>|
|<span data-ttu-id="f1608-117">instanceDisplayName</span><span class="sxs-lookup"><span data-stu-id="f1608-117">instanceDisplayName</span></span>|<span data-ttu-id="f1608-118">String</span><span class="sxs-lookup"><span data-stu-id="f1608-118">String</span></span>|<span data-ttu-id="f1608-119">レポートされている設定インスタンスの名前です。</span><span class="sxs-lookup"><span data-stu-id="f1608-119">Name of setting instance that is being reported.</span></span>|
|<span data-ttu-id="f1608-120">state</span><span class="sxs-lookup"><span data-stu-id="f1608-120">state</span></span>|[<span data-ttu-id="f1608-121">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="f1608-121">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="f1608-122">設定のコンプライアンス状態。</span><span class="sxs-lookup"><span data-stu-id="f1608-122">The compliance state of the setting.</span></span> <span data-ttu-id="f1608-123">可能な値は、`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned` です。</span><span class="sxs-lookup"><span data-stu-id="f1608-123">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="f1608-124">errorCode</span><span class="sxs-lookup"><span data-stu-id="f1608-124">errorCode</span></span>|<span data-ttu-id="f1608-125">Int64</span><span class="sxs-lookup"><span data-stu-id="f1608-125">Int64</span></span>|<span data-ttu-id="f1608-126">設定のエラー コード</span><span class="sxs-lookup"><span data-stu-id="f1608-126">Error code for the setting</span></span>|
|<span data-ttu-id="f1608-127">errorDescription</span><span class="sxs-lookup"><span data-stu-id="f1608-127">errorDescription</span></span>|<span data-ttu-id="f1608-128">String</span><span class="sxs-lookup"><span data-stu-id="f1608-128">String</span></span>|<span data-ttu-id="f1608-129">エラーの説明</span><span class="sxs-lookup"><span data-stu-id="f1608-129">Error description</span></span>|
|<span data-ttu-id="f1608-130">userId</span><span class="sxs-lookup"><span data-stu-id="f1608-130">userId</span></span>|<span data-ttu-id="f1608-131">String</span><span class="sxs-lookup"><span data-stu-id="f1608-131">String</span></span>|<span data-ttu-id="f1608-132">UserId</span><span class="sxs-lookup"><span data-stu-id="f1608-132">UserId</span></span>|
|<span data-ttu-id="f1608-133">userName</span><span class="sxs-lookup"><span data-stu-id="f1608-133">userName</span></span>|<span data-ttu-id="f1608-134">String</span><span class="sxs-lookup"><span data-stu-id="f1608-134">String</span></span>|<span data-ttu-id="f1608-135">UserName</span><span class="sxs-lookup"><span data-stu-id="f1608-135">UserName</span></span>|
|<span data-ttu-id="f1608-136">userEmail</span><span class="sxs-lookup"><span data-stu-id="f1608-136">userEmail</span></span>|<span data-ttu-id="f1608-137">String</span><span class="sxs-lookup"><span data-stu-id="f1608-137">String</span></span>|<span data-ttu-id="f1608-138">UserEmail</span><span class="sxs-lookup"><span data-stu-id="f1608-138">UserEmail</span></span>|
|<span data-ttu-id="f1608-139">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="f1608-139">userPrincipalName</span></span>|<span data-ttu-id="f1608-140">String</span><span class="sxs-lookup"><span data-stu-id="f1608-140">String</span></span>|<span data-ttu-id="f1608-141">UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="f1608-141">UserPrincipalName.</span></span>|
|<span data-ttu-id="f1608-142">ソース</span><span class="sxs-lookup"><span data-stu-id="f1608-142">sources</span></span>|<span data-ttu-id="f1608-143">[settingSource](../resources/intune-deviceconfig-settingsource.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="f1608-143">[settingSource](../resources/intune-deviceconfig-settingsource.md) collection</span></span>|<span data-ttu-id="f1608-144">投稿ポリシー</span><span class="sxs-lookup"><span data-stu-id="f1608-144">Contributing policies</span></span>|
|<span data-ttu-id="f1608-145">currentValue</span><span class="sxs-lookup"><span data-stu-id="f1608-145">currentValue</span></span>|<span data-ttu-id="f1608-146">String</span><span class="sxs-lookup"><span data-stu-id="f1608-146">String</span></span>|<span data-ttu-id="f1608-147">デバイスに関する設定の現在の値</span><span class="sxs-lookup"><span data-stu-id="f1608-147">Current value of setting on device</span></span>|

## <a name="relationships"></a><span data-ttu-id="f1608-148">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="f1608-148">Relationships</span></span>
<span data-ttu-id="f1608-149">なし</span><span class="sxs-lookup"><span data-stu-id="f1608-149">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f1608-150">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f1608-150">JSON Representation</span></span>
<span data-ttu-id="f1608-151">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="f1608-151">Here is a JSON representation of the resource.</span></span>
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




