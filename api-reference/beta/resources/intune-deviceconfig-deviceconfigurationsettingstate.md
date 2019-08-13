---
title: deviceConfigurationSettingState リソースの種類
description: 指定されたデバイスのデバイス構成設定の状態。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 347699a1160c7788ca3933a3bcbedf1833265bd0
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36332947"
---
# <a name="deviceconfigurationsettingstate-resource-type"></a><span data-ttu-id="b07ab-103">deviceConfigurationSettingState リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b07ab-103">deviceConfigurationSettingState resource type</span></span>

> <span data-ttu-id="b07ab-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b07ab-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b07ab-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="b07ab-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b07ab-106">指定されたデバイスのデバイス構成設定の状態。</span><span class="sxs-lookup"><span data-stu-id="b07ab-106">Device Configuration Setting State for a given device.</span></span>

## <a name="properties"></a><span data-ttu-id="b07ab-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b07ab-107">Properties</span></span>
|<span data-ttu-id="b07ab-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b07ab-108">Property</span></span>|<span data-ttu-id="b07ab-109">型</span><span class="sxs-lookup"><span data-stu-id="b07ab-109">Type</span></span>|<span data-ttu-id="b07ab-110">説明</span><span class="sxs-lookup"><span data-stu-id="b07ab-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b07ab-111">setting</span><span class="sxs-lookup"><span data-stu-id="b07ab-111">setting</span></span>|<span data-ttu-id="b07ab-112">String</span><span class="sxs-lookup"><span data-stu-id="b07ab-112">String</span></span>|<span data-ttu-id="b07ab-113">レポートされる設定値。</span><span class="sxs-lookup"><span data-stu-id="b07ab-113">The setting that is being reported</span></span>|
|<span data-ttu-id="b07ab-114">settingName</span><span class="sxs-lookup"><span data-stu-id="b07ab-114">settingName</span></span>|<span data-ttu-id="b07ab-115">String</span><span class="sxs-lookup"><span data-stu-id="b07ab-115">String</span></span>|<span data-ttu-id="b07ab-116">レポートされている、ローカライズされた設定名またはユーザー フレンドリな設定名</span><span class="sxs-lookup"><span data-stu-id="b07ab-116">Localized/user friendly setting name that is being reported</span></span>|
|<span data-ttu-id="b07ab-117">instanceDisplayName</span><span class="sxs-lookup"><span data-stu-id="b07ab-117">instanceDisplayName</span></span>|<span data-ttu-id="b07ab-118">String</span><span class="sxs-lookup"><span data-stu-id="b07ab-118">String</span></span>|<span data-ttu-id="b07ab-119">レポートされている設定インスタンスの名前です。</span><span class="sxs-lookup"><span data-stu-id="b07ab-119">Name of setting instance that is being reported.</span></span>|
|<span data-ttu-id="b07ab-120">state</span><span class="sxs-lookup"><span data-stu-id="b07ab-120">state</span></span>|[<span data-ttu-id="b07ab-121">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="b07ab-121">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="b07ab-122">設定のコンプライアンス状態。</span><span class="sxs-lookup"><span data-stu-id="b07ab-122">The compliance state of the setting.</span></span> <span data-ttu-id="b07ab-123">可能な値は、`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned` です。</span><span class="sxs-lookup"><span data-stu-id="b07ab-123">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="b07ab-124">errorCode</span><span class="sxs-lookup"><span data-stu-id="b07ab-124">errorCode</span></span>|<span data-ttu-id="b07ab-125">Int64</span><span class="sxs-lookup"><span data-stu-id="b07ab-125">Int64</span></span>|<span data-ttu-id="b07ab-126">設定のエラー コード</span><span class="sxs-lookup"><span data-stu-id="b07ab-126">Error code for the setting</span></span>|
|<span data-ttu-id="b07ab-127">errorDescription</span><span class="sxs-lookup"><span data-stu-id="b07ab-127">errorDescription</span></span>|<span data-ttu-id="b07ab-128">String</span><span class="sxs-lookup"><span data-stu-id="b07ab-128">String</span></span>|<span data-ttu-id="b07ab-129">エラーの説明</span><span class="sxs-lookup"><span data-stu-id="b07ab-129">Error description</span></span>|
|<span data-ttu-id="b07ab-130">userId</span><span class="sxs-lookup"><span data-stu-id="b07ab-130">userId</span></span>|<span data-ttu-id="b07ab-131">String</span><span class="sxs-lookup"><span data-stu-id="b07ab-131">String</span></span>|<span data-ttu-id="b07ab-132">UserId</span><span class="sxs-lookup"><span data-stu-id="b07ab-132">UserId</span></span>|
|<span data-ttu-id="b07ab-133">userName</span><span class="sxs-lookup"><span data-stu-id="b07ab-133">userName</span></span>|<span data-ttu-id="b07ab-134">String</span><span class="sxs-lookup"><span data-stu-id="b07ab-134">String</span></span>|<span data-ttu-id="b07ab-135">UserName</span><span class="sxs-lookup"><span data-stu-id="b07ab-135">UserName</span></span>|
|<span data-ttu-id="b07ab-136">userEmail</span><span class="sxs-lookup"><span data-stu-id="b07ab-136">userEmail</span></span>|<span data-ttu-id="b07ab-137">String</span><span class="sxs-lookup"><span data-stu-id="b07ab-137">String</span></span>|<span data-ttu-id="b07ab-138">UserEmail</span><span class="sxs-lookup"><span data-stu-id="b07ab-138">UserEmail</span></span>|
|<span data-ttu-id="b07ab-139">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="b07ab-139">userPrincipalName</span></span>|<span data-ttu-id="b07ab-140">String</span><span class="sxs-lookup"><span data-stu-id="b07ab-140">String</span></span>|<span data-ttu-id="b07ab-141">UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="b07ab-141">UserPrincipalName.</span></span>|
|<span data-ttu-id="b07ab-142">sources</span><span class="sxs-lookup"><span data-stu-id="b07ab-142">sources</span></span>|<span data-ttu-id="b07ab-143">[settingSource](../resources/intune-deviceconfig-settingsource.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="b07ab-143">[settingSource](../resources/intune-deviceconfig-settingsource.md) collection</span></span>|<span data-ttu-id="b07ab-144">投稿ポリシー</span><span class="sxs-lookup"><span data-stu-id="b07ab-144">Contributing policies</span></span>|
|<span data-ttu-id="b07ab-145">currentValue</span><span class="sxs-lookup"><span data-stu-id="b07ab-145">currentValue</span></span>|<span data-ttu-id="b07ab-146">String</span><span class="sxs-lookup"><span data-stu-id="b07ab-146">String</span></span>|<span data-ttu-id="b07ab-147">デバイスに関する設定の現在の値</span><span class="sxs-lookup"><span data-stu-id="b07ab-147">Current value of setting on device</span></span>|

## <a name="relationships"></a><span data-ttu-id="b07ab-148">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b07ab-148">Relationships</span></span>
<span data-ttu-id="b07ab-149">なし</span><span class="sxs-lookup"><span data-stu-id="b07ab-149">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b07ab-150">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b07ab-150">JSON Representation</span></span>
<span data-ttu-id="b07ab-151">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="b07ab-151">Here is a JSON representation of the resource.</span></span>
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



