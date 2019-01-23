---
title: deviceConfigurationSettingState リソースの種類
description: 指定されたデバイスのデバイス構成設定の状態。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 9355cdf0aab60208246fdae699cda78be65d62ff
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29415188"
---
# <a name="deviceconfigurationsettingstate-resource-type"></a><span data-ttu-id="b402a-103">deviceConfigurationSettingState リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b402a-103">deviceConfigurationSettingState resource type</span></span>

> <span data-ttu-id="b402a-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="b402a-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="b402a-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b402a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b402a-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="b402a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b402a-107">指定されたデバイスのデバイス構成設定の状態。</span><span class="sxs-lookup"><span data-stu-id="b402a-107">Device Configuration Setting State for a given device.</span></span>

## <a name="properties"></a><span data-ttu-id="b402a-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b402a-108">Properties</span></span>
|<span data-ttu-id="b402a-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b402a-109">Property</span></span>|<span data-ttu-id="b402a-110">型</span><span class="sxs-lookup"><span data-stu-id="b402a-110">Type</span></span>|<span data-ttu-id="b402a-111">説明</span><span class="sxs-lookup"><span data-stu-id="b402a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b402a-112">setting</span><span class="sxs-lookup"><span data-stu-id="b402a-112">setting</span></span>|<span data-ttu-id="b402a-113">String</span><span class="sxs-lookup"><span data-stu-id="b402a-113">String</span></span>|<span data-ttu-id="b402a-114">レポートされている設定値です。</span><span class="sxs-lookup"><span data-stu-id="b402a-114">The setting that is being reported</span></span>|
|<span data-ttu-id="b402a-115">settingName</span><span class="sxs-lookup"><span data-stu-id="b402a-115">settingName</span></span>|<span data-ttu-id="b402a-116">String</span><span class="sxs-lookup"><span data-stu-id="b402a-116">String</span></span>|<span data-ttu-id="b402a-117">レポートされている、ローカライズされた設定名またはユーザー フレンドリな設定名です</span><span class="sxs-lookup"><span data-stu-id="b402a-117">Localized/user friendly setting name that is being reported</span></span>|
|<span data-ttu-id="b402a-118">instanceDisplayName</span><span class="sxs-lookup"><span data-stu-id="b402a-118">instanceDisplayName</span></span>|<span data-ttu-id="b402a-119">String</span><span class="sxs-lookup"><span data-stu-id="b402a-119">String</span></span>|<span data-ttu-id="b402a-120">レポートされている設定インスタンスの名前です。</span><span class="sxs-lookup"><span data-stu-id="b402a-120">Name of setting instance that is being reported.</span></span>|
|<span data-ttu-id="b402a-121">state</span><span class="sxs-lookup"><span data-stu-id="b402a-121">state</span></span>|[<span data-ttu-id="b402a-122">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="b402a-122">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="b402a-123">設定のコンプライアンスの状態です。</span><span class="sxs-lookup"><span data-stu-id="b402a-123">The compliance state of the setting.</span></span> <span data-ttu-id="b402a-124">可能な値は、`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned` です。</span><span class="sxs-lookup"><span data-stu-id="b402a-124">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="b402a-125">errorCode</span><span class="sxs-lookup"><span data-stu-id="b402a-125">errorCode</span></span>|<span data-ttu-id="b402a-126">Int64</span><span class="sxs-lookup"><span data-stu-id="b402a-126">Int64</span></span>|<span data-ttu-id="b402a-127">設定のエラー コード</span><span class="sxs-lookup"><span data-stu-id="b402a-127">Error code for the setting</span></span>|
|<span data-ttu-id="b402a-128">errorDescription</span><span class="sxs-lookup"><span data-stu-id="b402a-128">errorDescription</span></span>|<span data-ttu-id="b402a-129">String</span><span class="sxs-lookup"><span data-stu-id="b402a-129">String</span></span>|<span data-ttu-id="b402a-130">エラーの説明</span><span class="sxs-lookup"><span data-stu-id="b402a-130">Error description</span></span>|
|<span data-ttu-id="b402a-131">userId</span><span class="sxs-lookup"><span data-stu-id="b402a-131">userId</span></span>|<span data-ttu-id="b402a-132">String</span><span class="sxs-lookup"><span data-stu-id="b402a-132">String</span></span>|<span data-ttu-id="b402a-133">UserId</span><span class="sxs-lookup"><span data-stu-id="b402a-133">UserId</span></span>|
|<span data-ttu-id="b402a-134">userName</span><span class="sxs-lookup"><span data-stu-id="b402a-134">userName</span></span>|<span data-ttu-id="b402a-135">String</span><span class="sxs-lookup"><span data-stu-id="b402a-135">String</span></span>|<span data-ttu-id="b402a-136">UserName</span><span class="sxs-lookup"><span data-stu-id="b402a-136">UserName</span></span>|
|<span data-ttu-id="b402a-137">userEmail</span><span class="sxs-lookup"><span data-stu-id="b402a-137">userEmail</span></span>|<span data-ttu-id="b402a-138">String</span><span class="sxs-lookup"><span data-stu-id="b402a-138">String</span></span>|<span data-ttu-id="b402a-139">UserEmail</span><span class="sxs-lookup"><span data-stu-id="b402a-139">UserEmail</span></span>|
|<span data-ttu-id="b402a-140">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="b402a-140">userPrincipalName</span></span>|<span data-ttu-id="b402a-141">String</span><span class="sxs-lookup"><span data-stu-id="b402a-141">String</span></span>|<span data-ttu-id="b402a-142">UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="b402a-142">UserPrincipalName.</span></span>|
|<span data-ttu-id="b402a-143">ソース</span><span class="sxs-lookup"><span data-stu-id="b402a-143">sources</span></span>|<span data-ttu-id="b402a-144">[settingSource](../resources/intune-deviceconfig-settingsource.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="b402a-144">[settingSource](../resources/intune-deviceconfig-settingsource.md) collection</span></span>|<span data-ttu-id="b402a-145">投稿ポリシー</span><span class="sxs-lookup"><span data-stu-id="b402a-145">Contributing policies</span></span>|
|<span data-ttu-id="b402a-146">currentValue</span><span class="sxs-lookup"><span data-stu-id="b402a-146">currentValue</span></span>|<span data-ttu-id="b402a-147">String</span><span class="sxs-lookup"><span data-stu-id="b402a-147">String</span></span>|<span data-ttu-id="b402a-148">デバイスに関する設定の現在の値</span><span class="sxs-lookup"><span data-stu-id="b402a-148">Current value of setting on device</span></span>|

## <a name="relationships"></a><span data-ttu-id="b402a-149">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b402a-149">Relationships</span></span>
<span data-ttu-id="b402a-150">なし</span><span class="sxs-lookup"><span data-stu-id="b402a-150">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b402a-151">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b402a-151">JSON Representation</span></span>
<span data-ttu-id="b402a-152">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="b402a-152">Here is a JSON representation of the resource.</span></span>
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




