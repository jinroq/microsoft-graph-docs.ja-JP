---
title: deviceManagementSettings リソースの種類
description: まだ文書化されていません
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 4be3b818ec414d99af677965ed7324d8b52a9099
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36004548"
---
# <a name="devicemanagementsettings-resource-type"></a><span data-ttu-id="552b4-103">deviceManagementSettings リソースの種類</span><span class="sxs-lookup"><span data-stu-id="552b4-103">deviceManagementSettings resource type</span></span>

> <span data-ttu-id="552b4-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="552b4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="552b4-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="552b4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="552b4-106">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="552b4-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="552b4-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="552b4-107">Properties</span></span>
|<span data-ttu-id="552b4-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="552b4-108">Property</span></span>|<span data-ttu-id="552b4-109">型</span><span class="sxs-lookup"><span data-stu-id="552b4-109">Type</span></span>|<span data-ttu-id="552b4-110">説明</span><span class="sxs-lookup"><span data-stu-id="552b4-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="552b4-111">deviceComplianceCheckinThresholdDays</span><span class="sxs-lookup"><span data-stu-id="552b4-111">deviceComplianceCheckinThresholdDays</span></span>|<span data-ttu-id="552b4-112">Int32</span><span class="sxs-lookup"><span data-stu-id="552b4-112">Int32</span></span>|<span data-ttu-id="552b4-113">デバイスがチェックインせずに移動し、準拠性を維持できる日数です。</span><span class="sxs-lookup"><span data-stu-id="552b4-113">The number of days a device is allowed to go without checking in to remain compliant.</span></span> <span data-ttu-id="552b4-114">有効な値は 0 から 120 までです</span><span class="sxs-lookup"><span data-stu-id="552b4-114">Valid values 0 to 120</span></span>|
|<span data-ttu-id="552b4-115">isScheduledActionEnabled</span><span class="sxs-lookup"><span data-stu-id="552b4-115">isScheduledActionEnabled</span></span>|<span data-ttu-id="552b4-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="552b4-116">Boolean</span></span>|<span data-ttu-id="552b4-117">ルールのスケジュール済みアクションの機能が有効かどうか。</span><span class="sxs-lookup"><span data-stu-id="552b4-117">Is feature enabled or not for scheduled action for rule.</span></span>|
|<span data-ttu-id="552b4-118">secureByDefault</span><span class="sxs-lookup"><span data-stu-id="552b4-118">secureByDefault</span></span>|<span data-ttu-id="552b4-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="552b4-119">Boolean</span></span>|<span data-ttu-id="552b4-120">これが true の場合に、対象となるコンプライアンス ポリシーがないと、デバイスは非準拠となります</span><span class="sxs-lookup"><span data-stu-id="552b4-120">Device should be noncompliant when there is no compliance policy targeted when this is true</span></span>|
|<span data-ttu-id="552b4-121">enhancedJailBreak</span><span class="sxs-lookup"><span data-stu-id="552b4-121">enhancedJailBreak</span></span>|<span data-ttu-id="552b4-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="552b4-122">Boolean</span></span>|<span data-ttu-id="552b4-123">拡張 jailbreak 検出では、機能が有効または無効になっています。</span><span class="sxs-lookup"><span data-stu-id="552b4-123">Is feature enabled or not for enhanced jailbreak detection.</span></span>|
|<span data-ttu-id="552b4-124">deviceInactivityBeforeRetirementInDay</span><span class="sxs-lookup"><span data-stu-id="552b4-124">deviceInactivityBeforeRetirementInDay</span></span>|<span data-ttu-id="552b4-125">Int32</span><span class="sxs-lookup"><span data-stu-id="552b4-125">Int32</span></span>|<span data-ttu-id="552b4-126">指定した日数が経過してもデバイスがチェックインされない場合は、会社のデータが削除されている可能性があり、デバイスは管理下にありません。</span><span class="sxs-lookup"><span data-stu-id="552b4-126">When the device does not check in for specified number of days, the company data might be removed and the device will not be under management.</span></span> <span data-ttu-id="552b4-127">有効な値は 30 ~ 270</span><span class="sxs-lookup"><span data-stu-id="552b4-127">Valid values 30 to 270</span></span>|
|<span data-ttu-id="552b4-128">derivedCredentialProvider</span><span class="sxs-lookup"><span data-stu-id="552b4-128">derivedCredentialProvider</span></span>|[<span data-ttu-id="552b4-129">derivedCredentialProviderType</span><span class="sxs-lookup"><span data-stu-id="552b4-129">derivedCredentialProviderType</span></span>](../resources/intune-deviceconfig-derivedcredentialprovidertype.md)|<span data-ttu-id="552b4-130">このアカウントに使用する派生資格情報プロバイダー。</span><span class="sxs-lookup"><span data-stu-id="552b4-130">The Derived Credential Provider to use for this account.</span></span> <span data-ttu-id="552b4-131">可能な値は、`notConfigured`、`entrustDataCard`、`purebred`、`xTec`、`intercede` です。</span><span class="sxs-lookup"><span data-stu-id="552b4-131">Possible values are: `notConfigured`, `entrustDataCard`, `purebred`, `xTec`, `intercede`.</span></span>|
|<span data-ttu-id="552b4-132">derivedCredentialUrl</span><span class="sxs-lookup"><span data-stu-id="552b4-132">derivedCredentialUrl</span></span>|<span data-ttu-id="552b4-133">String</span><span class="sxs-lookup"><span data-stu-id="552b4-133">String</span></span>|<span data-ttu-id="552b4-134">派生資格情報プロバイダーセルフサービス URI。</span><span class="sxs-lookup"><span data-stu-id="552b4-134">The Derived Credential Provider self-service URI.</span></span>|
|<span data-ttu-id="552b4-135">androidDeviceAdministratorEnrollmentEnabled</span><span class="sxs-lookup"><span data-stu-id="552b4-135">androidDeviceAdministratorEnrollmentEnabled</span></span>|<span data-ttu-id="552b4-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="552b4-136">Boolean</span></span>|<span data-ttu-id="552b4-137">このアカウントに対して Android デバイス管理者の登録が有効になっているかどうかを判断するプロパティ。</span><span class="sxs-lookup"><span data-stu-id="552b4-137">The property to determine if Android device administrator enrollment is enabled for this account.</span></span>|

## <a name="relationships"></a><span data-ttu-id="552b4-138">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="552b4-138">Relationships</span></span>
<span data-ttu-id="552b4-139">なし</span><span class="sxs-lookup"><span data-stu-id="552b4-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="552b4-140">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="552b4-140">JSON Representation</span></span>
<span data-ttu-id="552b4-141">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="552b4-141">Here is a JSON representation of the resource.</span></span>
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
  "derivedCredentialUrl": "String",
  "androidDeviceAdministratorEnrollmentEnabled": true
}
```





