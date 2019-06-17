---
title: windowsAutopilotDeploymentProfile リソースの種類
description: Windows 自動操縦展開プロファイル
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: cfa37dd838e515978db7f6763d1b8e69b5c66417
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34993923"
---
# <a name="windowsautopilotdeploymentprofile-resource-type"></a><span data-ttu-id="49d3c-103">windowsAutopilotDeploymentProfile リソースの種類</span><span class="sxs-lookup"><span data-stu-id="49d3c-103">windowsAutopilotDeploymentProfile resource type</span></span>

> <span data-ttu-id="49d3c-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="49d3c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="49d3c-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="49d3c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="49d3c-106">Windows 自動操縦展開プロファイル</span><span class="sxs-lookup"><span data-stu-id="49d3c-106">Windows Autopilot Deployment Profile</span></span>

## <a name="methods"></a><span data-ttu-id="49d3c-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="49d3c-107">Methods</span></span>
|<span data-ttu-id="49d3c-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="49d3c-108">Method</span></span>|<span data-ttu-id="49d3c-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="49d3c-109">Return Type</span></span>|<span data-ttu-id="49d3c-110">説明</span><span class="sxs-lookup"><span data-stu-id="49d3c-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="49d3c-111">WindowsAutopilotDeploymentProfile を取得する</span><span class="sxs-lookup"><span data-stu-id="49d3c-111">Get windowsAutopilotDeploymentProfile</span></span>](../api/intune-enrollment-windowsautopilotdeploymentprofile-get.md)|[<span data-ttu-id="49d3c-112">windowsAutopilotDeploymentProfile</span><span class="sxs-lookup"><span data-stu-id="49d3c-112">windowsAutopilotDeploymentProfile</span></span>](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)|<span data-ttu-id="49d3c-113">[WindowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="49d3c-113">Read properties and relationships of the [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md) object.</span></span>|
|[<span data-ttu-id="49d3c-114">assign アクション</span><span class="sxs-lookup"><span data-stu-id="49d3c-114">assign action</span></span>](../api/intune-enrollment-windowsautopilotdeploymentprofile-assign.md)|<span data-ttu-id="49d3c-115">なし</span><span class="sxs-lookup"><span data-stu-id="49d3c-115">None</span></span>|<span data-ttu-id="49d3c-116">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="49d3c-116">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="49d3c-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="49d3c-117">Properties</span></span>
|<span data-ttu-id="49d3c-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="49d3c-118">Property</span></span>|<span data-ttu-id="49d3c-119">型</span><span class="sxs-lookup"><span data-stu-id="49d3c-119">Type</span></span>|<span data-ttu-id="49d3c-120">説明</span><span class="sxs-lookup"><span data-stu-id="49d3c-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="49d3c-121">id</span><span class="sxs-lookup"><span data-stu-id="49d3c-121">id</span></span>|<span data-ttu-id="49d3c-122">文字列</span><span class="sxs-lookup"><span data-stu-id="49d3c-122">String</span></span>|<span data-ttu-id="49d3c-123">プロファイルキー</span><span class="sxs-lookup"><span data-stu-id="49d3c-123">Profile Key</span></span>|
|<span data-ttu-id="49d3c-124">displayName</span><span class="sxs-lookup"><span data-stu-id="49d3c-124">displayName</span></span>|<span data-ttu-id="49d3c-125">String</span><span class="sxs-lookup"><span data-stu-id="49d3c-125">String</span></span>|<span data-ttu-id="49d3c-126">プロファイルの名前</span><span class="sxs-lookup"><span data-stu-id="49d3c-126">Name of the profile</span></span>|
|<span data-ttu-id="49d3c-127">description</span><span class="sxs-lookup"><span data-stu-id="49d3c-127">description</span></span>|<span data-ttu-id="49d3c-128">String</span><span class="sxs-lookup"><span data-stu-id="49d3c-128">String</span></span>|<span data-ttu-id="49d3c-129">プロファイルの説明</span><span class="sxs-lookup"><span data-stu-id="49d3c-129">Description of the profile</span></span>|
|<span data-ttu-id="49d3c-130">language</span><span class="sxs-lookup"><span data-stu-id="49d3c-130">language</span></span>|<span data-ttu-id="49d3c-131">String</span><span class="sxs-lookup"><span data-stu-id="49d3c-131">String</span></span>|<span data-ttu-id="49d3c-132">デバイスで構成されている言語</span><span class="sxs-lookup"><span data-stu-id="49d3c-132">Language configured on the device</span></span>|
|<span data-ttu-id="49d3c-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="49d3c-133">createdDateTime</span></span>|<span data-ttu-id="49d3c-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="49d3c-134">DateTimeOffset</span></span>|<span data-ttu-id="49d3c-135">プロファイルの作成時刻</span><span class="sxs-lookup"><span data-stu-id="49d3c-135">Profile creation time</span></span>|
|<span data-ttu-id="49d3c-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="49d3c-136">lastModifiedDateTime</span></span>|<span data-ttu-id="49d3c-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="49d3c-137">DateTimeOffset</span></span>|<span data-ttu-id="49d3c-138">プロファイルの最終変更日時</span><span class="sxs-lookup"><span data-stu-id="49d3c-138">Profile last modified time</span></span>|
|<span data-ttu-id="49d3c-139">outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="49d3c-139">outOfBoxExperienceSettings</span></span>|[<span data-ttu-id="49d3c-140">outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="49d3c-140">outOfBoxExperienceSettings</span></span>](../resources/intune-enrollment-outofboxexperiencesettings.md)|<span data-ttu-id="49d3c-141">不在時の環境設定</span><span class="sxs-lookup"><span data-stu-id="49d3c-141">Out of box experience setting</span></span>|
|<span data-ttu-id="49d3c-142">enrollmentStatusScreenSettings</span><span class="sxs-lookup"><span data-stu-id="49d3c-142">enrollmentStatusScreenSettings</span></span>|[<span data-ttu-id="49d3c-143">windowsEnrollmentStatusScreenSettings</span><span class="sxs-lookup"><span data-stu-id="49d3c-143">windowsEnrollmentStatusScreenSettings</span></span>](../resources/intune-enrollment-windowsenrollmentstatusscreensettings.md)|<span data-ttu-id="49d3c-144">登録の状態画面の設定</span><span class="sxs-lookup"><span data-stu-id="49d3c-144">Enrollment status screen setting</span></span>|
|<span data-ttu-id="49d3c-145">extractHardwareHash</span><span class="sxs-lookup"><span data-stu-id="49d3c-145">extractHardwareHash</span></span>|<span data-ttu-id="49d3c-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="49d3c-146">Boolean</span></span>|<span data-ttu-id="49d3c-147">プロファイルのハードウェアハッシュ抽出</span><span class="sxs-lookup"><span data-stu-id="49d3c-147">HardwareHash Extraction for the profile</span></span>|
|<span data-ttu-id="49d3c-148">deviceNameTemplate</span><span class="sxs-lookup"><span data-stu-id="49d3c-148">deviceNameTemplate</span></span>|<span data-ttu-id="49d3c-149">String</span><span class="sxs-lookup"><span data-stu-id="49d3c-149">String</span></span>|<span data-ttu-id="49d3c-150">自動操縦デバイスの名前を指定するときに使用するテンプレートを指定します。</span><span class="sxs-lookup"><span data-stu-id="49d3c-150">The template used to name the AutoPilot Device.</span></span> <span data-ttu-id="49d3c-151">これはカスタムテキストにすることができ、デバイスのシリアル番号またはランダムに生成された番号のいずれかを含めることもできます。</span><span class="sxs-lookup"><span data-stu-id="49d3c-151">This can be a custom text and can also contain either the serial number of the device, or a randomly generated number.</span></span> <span data-ttu-id="49d3c-152">テンプレートによって生成されるテキストの合計の長さは、15文字以下でなければなりません。</span><span class="sxs-lookup"><span data-stu-id="49d3c-152">The total length of the text generated by the template can be no more than 15 characters.</span></span>|
|<span data-ttu-id="49d3c-153">deviceType</span><span class="sxs-lookup"><span data-stu-id="49d3c-153">deviceType</span></span>|[<span data-ttu-id="49d3c-154">windowsAutopilotDeviceType</span><span class="sxs-lookup"><span data-stu-id="49d3c-154">windowsAutopilotDeviceType</span></span>](../resources/intune-enrollment-windowsautopilotdevicetype.md)|<span data-ttu-id="49d3c-155">このプロファイルを適用できる自動操縦デバイスの種類。</span><span class="sxs-lookup"><span data-stu-id="49d3c-155">The AutoPilot device type that this profile is applicable to.</span></span> <span data-ttu-id="49d3c-156">可能な値は、`windowsPc`、`surfaceHub2` です。</span><span class="sxs-lookup"><span data-stu-id="49d3c-156">Possible values are: `windowsPc`, `surfaceHub2`.</span></span>|
|<span data-ttu-id="49d3c-157">Enableホワイトグローブ</span><span class="sxs-lookup"><span data-stu-id="49d3c-157">enableWhiteGlove</span></span>|<span data-ttu-id="49d3c-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="49d3c-158">Boolean</span></span>|<span data-ttu-id="49d3c-159">プロファイルの自動操縦白の手袋を有効にします。</span><span class="sxs-lookup"><span data-stu-id="49d3c-159">Enable Autopilot White Glove for the profile.</span></span>|
|<span data-ttu-id="49d3c-160">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="49d3c-160">roleScopeTagIds</span></span>|<span data-ttu-id="49d3c-161">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="49d3c-161">String collection</span></span>|<span data-ttu-id="49d3c-162">プロファイルのスコープタグ。</span><span class="sxs-lookup"><span data-stu-id="49d3c-162">Scope tags for the profile.</span></span>|

## <a name="relationships"></a><span data-ttu-id="49d3c-163">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="49d3c-163">Relationships</span></span>
|<span data-ttu-id="49d3c-164">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="49d3c-164">Relationship</span></span>|<span data-ttu-id="49d3c-165">型</span><span class="sxs-lookup"><span data-stu-id="49d3c-165">Type</span></span>|<span data-ttu-id="49d3c-166">説明</span><span class="sxs-lookup"><span data-stu-id="49d3c-166">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="49d3c-167">assignedDevices</span><span class="sxs-lookup"><span data-stu-id="49d3c-167">assignedDevices</span></span>|<span data-ttu-id="49d3c-168">[windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="49d3c-168">[windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) collection</span></span>|<span data-ttu-id="49d3c-169">プロファイルに割り当てられているデバイスのリスト。</span><span class="sxs-lookup"><span data-stu-id="49d3c-169">The list of assigned devices for the profile.</span></span>|
|<span data-ttu-id="49d3c-170">assignments</span><span class="sxs-lookup"><span data-stu-id="49d3c-170">assignments</span></span>|<span data-ttu-id="49d3c-171">[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="49d3c-171">[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) collection</span></span>|<span data-ttu-id="49d3c-172">プロファイルのグループの割り当てのリスト。</span><span class="sxs-lookup"><span data-stu-id="49d3c-172">The list of group assignments for the profile.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="49d3c-173">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="49d3c-173">JSON Representation</span></span>
<span data-ttu-id="49d3c-174">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="49d3c-174">Here is a JSON representation of the resource.</span></span>
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





