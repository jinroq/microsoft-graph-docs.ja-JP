---
title: deviceManagementSettings リソースの種類
description: まだ文書化されていません
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 4f676eed1acbf6711f526e612bd6c073b749607d
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29417666"
---
# <a name="devicemanagementsettings-resource-type"></a><span data-ttu-id="ce40b-103">deviceManagementSettings リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ce40b-103">deviceManagementSettings resource type</span></span>

> <span data-ttu-id="ce40b-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="ce40b-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ce40b-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ce40b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ce40b-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="ce40b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ce40b-107">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="ce40b-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="ce40b-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ce40b-108">Properties</span></span>
|<span data-ttu-id="ce40b-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ce40b-109">Property</span></span>|<span data-ttu-id="ce40b-110">型</span><span class="sxs-lookup"><span data-stu-id="ce40b-110">Type</span></span>|<span data-ttu-id="ce40b-111">説明</span><span class="sxs-lookup"><span data-stu-id="ce40b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ce40b-112">deviceComplianceCheckinThresholdDays</span><span class="sxs-lookup"><span data-stu-id="ce40b-112">deviceComplianceCheckinThresholdDays</span></span>|<span data-ttu-id="ce40b-113">Int32</span><span class="sxs-lookup"><span data-stu-id="ce40b-113">Int32</span></span>|<span data-ttu-id="ce40b-114">デバイスがチェックインせずに移動し、準拠性を維持できる日数です。</span><span class="sxs-lookup"><span data-stu-id="ce40b-114">The number of days a device is allowed to go without checking in to remain compliant.</span></span> <span data-ttu-id="ce40b-115">有効な値は 0 から 120 までです</span><span class="sxs-lookup"><span data-stu-id="ce40b-115">Valid values 0 to 120</span></span>|
|<span data-ttu-id="ce40b-116">isScheduledActionEnabled</span><span class="sxs-lookup"><span data-stu-id="ce40b-116">isScheduledActionEnabled</span></span>|<span data-ttu-id="ce40b-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="ce40b-117">Boolean</span></span>|<span data-ttu-id="ce40b-118">ルールのスケジュール済みアクションの機能が有効かどうか。</span><span class="sxs-lookup"><span data-stu-id="ce40b-118">Is feature enabled or not for scheduled action for rule.</span></span>|
|<span data-ttu-id="ce40b-119">secureByDefault</span><span class="sxs-lookup"><span data-stu-id="ce40b-119">secureByDefault</span></span>|<span data-ttu-id="ce40b-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="ce40b-120">Boolean</span></span>|<span data-ttu-id="ce40b-121">これが true の場合に、対象となるコンプライアンス ポリシーがないと、デバイスは非準拠となります</span><span class="sxs-lookup"><span data-stu-id="ce40b-121">Device should be noncompliant when there is no compliance policy targeted when this is true</span></span>|
|<span data-ttu-id="ce40b-122">enhancedJailBreak</span><span class="sxs-lookup"><span data-stu-id="ce40b-122">enhancedJailBreak</span></span>|<span data-ttu-id="ce40b-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="ce40b-123">Boolean</span></span>|<span data-ttu-id="ce40b-124">機能が有効かではなく、jailbreak の検出を強化します。</span><span class="sxs-lookup"><span data-stu-id="ce40b-124">Is feature enabled or not for enhanced jailbreak detection.</span></span>|
|<span data-ttu-id="ce40b-125">deviceInactivityBeforeRetirementInDay</span><span class="sxs-lookup"><span data-stu-id="ce40b-125">deviceInactivityBeforeRetirementInDay</span></span>|<span data-ttu-id="ce40b-126">Int32</span><span class="sxs-lookup"><span data-stu-id="ce40b-126">Int32</span></span>|<span data-ttu-id="ce40b-127">デバイスをチェックしません指定した日数、会社のデータを削除する可能性があり、デバイスを [管理] ではできません。</span><span class="sxs-lookup"><span data-stu-id="ce40b-127">When the device does not check in for specified number of days, the company data might be removed and the device will not be under management.</span></span> <span data-ttu-id="ce40b-128">有効な値の 30 ~ 270</span><span class="sxs-lookup"><span data-stu-id="ce40b-128">Valid values 30 to 270</span></span>|
|<span data-ttu-id="ce40b-129">derivedCredentialProvider</span><span class="sxs-lookup"><span data-stu-id="ce40b-129">derivedCredentialProvider</span></span>|[<span data-ttu-id="ce40b-130">derivedCredentialProviderType</span><span class="sxs-lookup"><span data-stu-id="ce40b-130">derivedCredentialProviderType</span></span>](../resources/intune-deviceconfig-derivedcredentialprovidertype.md)|<span data-ttu-id="ce40b-131">派生した資格情報プロバイダーはこのアカウントに使用します。</span><span class="sxs-lookup"><span data-stu-id="ce40b-131">The Derived Credential Provider to use for this account.</span></span> <span data-ttu-id="ce40b-132">可能な値は、`notConfigured`、`entrustDataCard`、`purebred`、`xTec`、`intercede` です。</span><span class="sxs-lookup"><span data-stu-id="ce40b-132">Possible values are: `notConfigured`, `entrustDataCard`, `purebred`, `xTec`, `intercede`.</span></span>|
|<span data-ttu-id="ce40b-133">derivedCredentialUrl</span><span class="sxs-lookup"><span data-stu-id="ce40b-133">derivedCredentialUrl</span></span>|<span data-ttu-id="ce40b-134">String</span><span class="sxs-lookup"><span data-stu-id="ce40b-134">String</span></span>|<span data-ttu-id="ce40b-135">資格情報プロバイダーの派生のセルフ サービスの URI です。</span><span class="sxs-lookup"><span data-stu-id="ce40b-135">The Derived Credential Provider self-service URI.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ce40b-136">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ce40b-136">Relationships</span></span>
<span data-ttu-id="ce40b-137">なし</span><span class="sxs-lookup"><span data-stu-id="ce40b-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ce40b-138">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ce40b-138">JSON Representation</span></span>
<span data-ttu-id="ce40b-139">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="ce40b-139">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementSettings",
  "deviceComplianceCheckinThresholdDays": 1024,
  "isScheduledActionEnabled": true,
  "secureByDefault": true,
  "enhancedJailBreak": true,
  "deviceInactivityBeforeRetirementInDay": 1024,
  "derivedCredentialProvider": "String",
  "derivedCredentialUrl": "String"
}
```




