---
title: windowsAutopilotDeploymentProfile リソースの種類
description: Windows 自動操縦展開プロファイル
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 1c79cc44ae9ffbe96097a0100f55a22b3d873e0e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35999032"
---
# <a name="windowsautopilotdeploymentprofile-resource-type"></a><span data-ttu-id="971e6-103">windowsAutopilotDeploymentProfile リソースの種類</span><span class="sxs-lookup"><span data-stu-id="971e6-103">windowsAutopilotDeploymentProfile resource type</span></span>

> <span data-ttu-id="971e6-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="971e6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="971e6-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="971e6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="971e6-106">Windows 自動操縦展開プロファイル</span><span class="sxs-lookup"><span data-stu-id="971e6-106">Windows Autopilot Deployment Profile</span></span>

## <a name="methods"></a><span data-ttu-id="971e6-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="971e6-107">Methods</span></span>
|<span data-ttu-id="971e6-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="971e6-108">Method</span></span>|<span data-ttu-id="971e6-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="971e6-109">Return Type</span></span>|<span data-ttu-id="971e6-110">説明</span><span class="sxs-lookup"><span data-stu-id="971e6-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="971e6-111">WindowsAutopilotDeploymentProfile を取得する</span><span class="sxs-lookup"><span data-stu-id="971e6-111">Get windowsAutopilotDeploymentProfile</span></span>](../api/intune-enrollment-windowsautopilotdeploymentprofile-get.md)|[<span data-ttu-id="971e6-112">windowsAutopilotDeploymentProfile</span><span class="sxs-lookup"><span data-stu-id="971e6-112">windowsAutopilotDeploymentProfile</span></span>](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)|<span data-ttu-id="971e6-113">[WindowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="971e6-113">Read properties and relationships of the [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md) object.</span></span>|
|[<span data-ttu-id="971e6-114">assign アクション</span><span class="sxs-lookup"><span data-stu-id="971e6-114">assign action</span></span>](../api/intune-enrollment-windowsautopilotdeploymentprofile-assign.md)|<span data-ttu-id="971e6-115">なし</span><span class="sxs-lookup"><span data-stu-id="971e6-115">None</span></span>|<span data-ttu-id="971e6-116">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="971e6-116">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="971e6-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="971e6-117">Properties</span></span>
|<span data-ttu-id="971e6-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="971e6-118">Property</span></span>|<span data-ttu-id="971e6-119">型</span><span class="sxs-lookup"><span data-stu-id="971e6-119">Type</span></span>|<span data-ttu-id="971e6-120">説明</span><span class="sxs-lookup"><span data-stu-id="971e6-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="971e6-121">id</span><span class="sxs-lookup"><span data-stu-id="971e6-121">id</span></span>|<span data-ttu-id="971e6-122">文字列</span><span class="sxs-lookup"><span data-stu-id="971e6-122">String</span></span>|<span data-ttu-id="971e6-123">プロファイルキー</span><span class="sxs-lookup"><span data-stu-id="971e6-123">Profile Key</span></span>|
|<span data-ttu-id="971e6-124">displayName</span><span class="sxs-lookup"><span data-stu-id="971e6-124">displayName</span></span>|<span data-ttu-id="971e6-125">String</span><span class="sxs-lookup"><span data-stu-id="971e6-125">String</span></span>|<span data-ttu-id="971e6-126">プロファイルの名前</span><span class="sxs-lookup"><span data-stu-id="971e6-126">Name of the profile</span></span>|
|<span data-ttu-id="971e6-127">description</span><span class="sxs-lookup"><span data-stu-id="971e6-127">description</span></span>|<span data-ttu-id="971e6-128">String</span><span class="sxs-lookup"><span data-stu-id="971e6-128">String</span></span>|<span data-ttu-id="971e6-129">プロファイルの説明</span><span class="sxs-lookup"><span data-stu-id="971e6-129">Description of the profile</span></span>|
|<span data-ttu-id="971e6-130">language</span><span class="sxs-lookup"><span data-stu-id="971e6-130">language</span></span>|<span data-ttu-id="971e6-131">String</span><span class="sxs-lookup"><span data-stu-id="971e6-131">String</span></span>|<span data-ttu-id="971e6-132">デバイスで構成されている言語</span><span class="sxs-lookup"><span data-stu-id="971e6-132">Language configured on the device</span></span>|
|<span data-ttu-id="971e6-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="971e6-133">createdDateTime</span></span>|<span data-ttu-id="971e6-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="971e6-134">DateTimeOffset</span></span>|<span data-ttu-id="971e6-135">プロファイルの作成時刻</span><span class="sxs-lookup"><span data-stu-id="971e6-135">Profile creation time</span></span>|
|<span data-ttu-id="971e6-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="971e6-136">lastModifiedDateTime</span></span>|<span data-ttu-id="971e6-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="971e6-137">DateTimeOffset</span></span>|<span data-ttu-id="971e6-138">プロファイルの最終変更日時</span><span class="sxs-lookup"><span data-stu-id="971e6-138">Profile last modified time</span></span>|
|<span data-ttu-id="971e6-139">outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="971e6-139">outOfBoxExperienceSettings</span></span>|[<span data-ttu-id="971e6-140">outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="971e6-140">outOfBoxExperienceSettings</span></span>](../resources/intune-enrollment-outofboxexperiencesettings.md)|<span data-ttu-id="971e6-141">不在時の環境設定</span><span class="sxs-lookup"><span data-stu-id="971e6-141">Out of box experience setting</span></span>|
|<span data-ttu-id="971e6-142">enrollmentStatusScreenSettings</span><span class="sxs-lookup"><span data-stu-id="971e6-142">enrollmentStatusScreenSettings</span></span>|[<span data-ttu-id="971e6-143">windowsEnrollmentStatusScreenSettings</span><span class="sxs-lookup"><span data-stu-id="971e6-143">windowsEnrollmentStatusScreenSettings</span></span>](../resources/intune-enrollment-windowsenrollmentstatusscreensettings.md)|<span data-ttu-id="971e6-144">登録の状態画面の設定</span><span class="sxs-lookup"><span data-stu-id="971e6-144">Enrollment status screen setting</span></span>|
|<span data-ttu-id="971e6-145">extractHardwareHash</span><span class="sxs-lookup"><span data-stu-id="971e6-145">extractHardwareHash</span></span>|<span data-ttu-id="971e6-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="971e6-146">Boolean</span></span>|<span data-ttu-id="971e6-147">プロファイルのハードウェアハッシュ抽出</span><span class="sxs-lookup"><span data-stu-id="971e6-147">HardwareHash Extraction for the profile</span></span>|
|<span data-ttu-id="971e6-148">deviceNameTemplate</span><span class="sxs-lookup"><span data-stu-id="971e6-148">deviceNameTemplate</span></span>|<span data-ttu-id="971e6-149">String</span><span class="sxs-lookup"><span data-stu-id="971e6-149">String</span></span>|<span data-ttu-id="971e6-150">自動操縦デバイスの名前を指定するときに使用するテンプレートを指定します。</span><span class="sxs-lookup"><span data-stu-id="971e6-150">The template used to name the AutoPilot Device.</span></span> <span data-ttu-id="971e6-151">これはカスタムテキストにすることができ、デバイスのシリアル番号またはランダムに生成された番号のいずれかを含めることもできます。</span><span class="sxs-lookup"><span data-stu-id="971e6-151">This can be a custom text and can also contain either the serial number of the device, or a randomly generated number.</span></span> <span data-ttu-id="971e6-152">テンプレートによって生成されるテキストの合計の長さは、15文字以下でなければなりません。</span><span class="sxs-lookup"><span data-stu-id="971e6-152">The total length of the text generated by the template can be no more than 15 characters.</span></span>|
|<span data-ttu-id="971e6-153">deviceType</span><span class="sxs-lookup"><span data-stu-id="971e6-153">deviceType</span></span>|[<span data-ttu-id="971e6-154">windowsAutopilotDeviceType</span><span class="sxs-lookup"><span data-stu-id="971e6-154">windowsAutopilotDeviceType</span></span>](../resources/intune-enrollment-windowsautopilotdevicetype.md)|<span data-ttu-id="971e6-155">このプロファイルを適用できる自動操縦デバイスの種類。</span><span class="sxs-lookup"><span data-stu-id="971e6-155">The AutoPilot device type that this profile is applicable to.</span></span> <span data-ttu-id="971e6-156">可能な値は、`windowsPc`、`surfaceHub2` です。</span><span class="sxs-lookup"><span data-stu-id="971e6-156">Possible values are: `windowsPc`, `surfaceHub2`.</span></span>|
|<span data-ttu-id="971e6-157">Enableホワイトグローブ</span><span class="sxs-lookup"><span data-stu-id="971e6-157">enableWhiteGlove</span></span>|<span data-ttu-id="971e6-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="971e6-158">Boolean</span></span>|<span data-ttu-id="971e6-159">プロファイルの自動操縦白の手袋を有効にします。</span><span class="sxs-lookup"><span data-stu-id="971e6-159">Enable Autopilot White Glove for the profile.</span></span>|
|<span data-ttu-id="971e6-160">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="971e6-160">roleScopeTagIds</span></span>|<span data-ttu-id="971e6-161">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="971e6-161">String collection</span></span>|<span data-ttu-id="971e6-162">プロファイルのスコープタグ。</span><span class="sxs-lookup"><span data-stu-id="971e6-162">Scope tags for the profile.</span></span>|

## <a name="relationships"></a><span data-ttu-id="971e6-163">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="971e6-163">Relationships</span></span>
|<span data-ttu-id="971e6-164">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="971e6-164">Relationship</span></span>|<span data-ttu-id="971e6-165">型</span><span class="sxs-lookup"><span data-stu-id="971e6-165">Type</span></span>|<span data-ttu-id="971e6-166">説明</span><span class="sxs-lookup"><span data-stu-id="971e6-166">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="971e6-167">assignedDevices</span><span class="sxs-lookup"><span data-stu-id="971e6-167">assignedDevices</span></span>|<span data-ttu-id="971e6-168">[windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="971e6-168">[windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) collection</span></span>|<span data-ttu-id="971e6-169">プロファイルに割り当てられているデバイスのリスト。</span><span class="sxs-lookup"><span data-stu-id="971e6-169">The list of assigned devices for the profile.</span></span>|
|<span data-ttu-id="971e6-170">assignments</span><span class="sxs-lookup"><span data-stu-id="971e6-170">assignments</span></span>|<span data-ttu-id="971e6-171">[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="971e6-171">[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) collection</span></span>|<span data-ttu-id="971e6-172">プロファイルのグループの割り当てのリスト。</span><span class="sxs-lookup"><span data-stu-id="971e6-172">The list of group assignments for the profile.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="971e6-173">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="971e6-173">JSON Representation</span></span>
<span data-ttu-id="971e6-174">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="971e6-174">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsAutopilotDeploymentProfile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsAutopilotDeploymentProfile",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "language": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "outOfBoxExperienceSettings": {
    "@odata.type": "microsoft.graph.outOfBoxExperienceSettings",
    "hidePrivacySettings": true,
    "hideEULA": true,
    "userType": "String",
    "deviceUsageType": "String",
    "skipKeyboardSelectionPage": true,
    "hideEscapeLink": true
  },
  "enrollmentStatusScreenSettings": {
    "@odata.type": "microsoft.graph.windowsEnrollmentStatusScreenSettings",
    "hideInstallationProgress": true,
    "allowDeviceUseBeforeProfileAndAppInstallComplete": true,
    "blockDeviceSetupRetryByUser": true,
    "allowLogCollectionOnInstallFailure": true,
    "customErrorMessage": "String",
    "installProgressTimeoutInMinutes": 1024,
    "allowDeviceUseOnInstallFailure": true
  },
  "extractHardwareHash": true,
  "deviceNameTemplate": "String",
  "deviceType": "String",
  "enableWhiteGlove": true,
  "roleScopeTagIds": [
    "String"
  ]
}
```





