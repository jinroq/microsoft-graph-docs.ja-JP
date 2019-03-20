---
title: windowsAutopilotDeploymentProfile リソースの種類
description: Windows 自動操縦展開プロファイル
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 69035ba93b04ac66ce9e8883c7b5f7b04dff429a
ms.sourcegitcommit: f58ff560fa02ac95e296375c143b0922fb6a425c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/19/2019
ms.locfileid: "30572461"
---
# <a name="windowsautopilotdeploymentprofile-resource-type"></a><span data-ttu-id="18b85-103">windowsAutopilotDeploymentProfile リソースの種類</span><span class="sxs-lookup"><span data-stu-id="18b85-103">windowsAutopilotDeploymentProfile resource type</span></span>

> <span data-ttu-id="18b85-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="18b85-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="18b85-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="18b85-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="18b85-106">Windows 自動操縦展開プロファイル</span><span class="sxs-lookup"><span data-stu-id="18b85-106">Windows Autopilot Deployment Profile</span></span>

## <a name="methods"></a><span data-ttu-id="18b85-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="18b85-107">Methods</span></span>
|<span data-ttu-id="18b85-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="18b85-108">Method</span></span>|<span data-ttu-id="18b85-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="18b85-109">Return Type</span></span>|<span data-ttu-id="18b85-110">説明</span><span class="sxs-lookup"><span data-stu-id="18b85-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="18b85-111">windowsAutopilotDeploymentProfile を取得する</span><span class="sxs-lookup"><span data-stu-id="18b85-111">Get windowsAutopilotDeploymentProfile</span></span>](../api/intune-enrollment-windowsautopilotdeploymentprofile-get.md)|[<span data-ttu-id="18b85-112">windowsAutopilotDeploymentProfile</span><span class="sxs-lookup"><span data-stu-id="18b85-112">windowsAutopilotDeploymentProfile</span></span>](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)|<span data-ttu-id="18b85-113">[windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="18b85-113">Read properties and relationships of the [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md) object.</span></span>|
|[<span data-ttu-id="18b85-114">assign アクション</span><span class="sxs-lookup"><span data-stu-id="18b85-114">assign action</span></span>](../api/intune-enrollment-windowsautopilotdeploymentprofile-assign.md)|<span data-ttu-id="18b85-115">なし</span><span class="sxs-lookup"><span data-stu-id="18b85-115">None</span></span>|<span data-ttu-id="18b85-116">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="18b85-116">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="18b85-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="18b85-117">Properties</span></span>
|<span data-ttu-id="18b85-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="18b85-118">Property</span></span>|<span data-ttu-id="18b85-119">種類</span><span class="sxs-lookup"><span data-stu-id="18b85-119">Type</span></span>|<span data-ttu-id="18b85-120">説明</span><span class="sxs-lookup"><span data-stu-id="18b85-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="18b85-121">id</span><span class="sxs-lookup"><span data-stu-id="18b85-121">id</span></span>|<span data-ttu-id="18b85-122">String</span><span class="sxs-lookup"><span data-stu-id="18b85-122">String</span></span>|<span data-ttu-id="18b85-123">プロファイルキー</span><span class="sxs-lookup"><span data-stu-id="18b85-123">Profile Key</span></span>|
|<span data-ttu-id="18b85-124">displayName</span><span class="sxs-lookup"><span data-stu-id="18b85-124">displayName</span></span>|<span data-ttu-id="18b85-125">String</span><span class="sxs-lookup"><span data-stu-id="18b85-125">String</span></span>|<span data-ttu-id="18b85-126">プロファイルの名前</span><span class="sxs-lookup"><span data-stu-id="18b85-126">Name of the profile</span></span>|
|<span data-ttu-id="18b85-127">description</span><span class="sxs-lookup"><span data-stu-id="18b85-127">description</span></span>|<span data-ttu-id="18b85-128">String</span><span class="sxs-lookup"><span data-stu-id="18b85-128">String</span></span>|<span data-ttu-id="18b85-129">プロファイルの説明</span><span class="sxs-lookup"><span data-stu-id="18b85-129">Description of the profile</span></span>|
|<span data-ttu-id="18b85-130">language</span><span class="sxs-lookup"><span data-stu-id="18b85-130">language</span></span>|<span data-ttu-id="18b85-131">String</span><span class="sxs-lookup"><span data-stu-id="18b85-131">String</span></span>|<span data-ttu-id="18b85-132">デバイスで構成されている言語</span><span class="sxs-lookup"><span data-stu-id="18b85-132">Language configured on the device</span></span>|
|<span data-ttu-id="18b85-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="18b85-133">createdDateTime</span></span>|<span data-ttu-id="18b85-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="18b85-134">DateTimeOffset</span></span>|<span data-ttu-id="18b85-135">プロファイルの作成時刻</span><span class="sxs-lookup"><span data-stu-id="18b85-135">Profile creation time</span></span>|
|<span data-ttu-id="18b85-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="18b85-136">lastModifiedDateTime</span></span>|<span data-ttu-id="18b85-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="18b85-137">DateTimeOffset</span></span>|<span data-ttu-id="18b85-138">プロファイルの最終変更日時</span><span class="sxs-lookup"><span data-stu-id="18b85-138">Profile last modified time</span></span>|
|<span data-ttu-id="18b85-139">outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="18b85-139">outOfBoxExperienceSettings</span></span>|[<span data-ttu-id="18b85-140">outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="18b85-140">outOfBoxExperienceSettings</span></span>](../resources/intune-enrollment-outofboxexperiencesettings.md)|<span data-ttu-id="18b85-141">不在時の環境設定</span><span class="sxs-lookup"><span data-stu-id="18b85-141">Out of box experience setting</span></span>|
|<span data-ttu-id="18b85-142">enrollmentStatusScreenSettings</span><span class="sxs-lookup"><span data-stu-id="18b85-142">enrollmentStatusScreenSettings</span></span>|[<span data-ttu-id="18b85-143">windowsEnrollmentStatusScreenSettings</span><span class="sxs-lookup"><span data-stu-id="18b85-143">windowsEnrollmentStatusScreenSettings</span></span>](../resources/intune-enrollment-windowsenrollmentstatusscreensettings.md)|<span data-ttu-id="18b85-144">登録の状態画面の設定</span><span class="sxs-lookup"><span data-stu-id="18b85-144">Enrollment status screen setting</span></span>|
|<span data-ttu-id="18b85-145">extractHardwareHash</span><span class="sxs-lookup"><span data-stu-id="18b85-145">extractHardwareHash</span></span>|<span data-ttu-id="18b85-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="18b85-146">Boolean</span></span>|<span data-ttu-id="18b85-147">プロファイルのハードウェアハッシュ抽出</span><span class="sxs-lookup"><span data-stu-id="18b85-147">HardwareHash Extraction for the profile</span></span>|
|<span data-ttu-id="18b85-148">deviceNameTemplate</span><span class="sxs-lookup"><span data-stu-id="18b85-148">deviceNameTemplate</span></span>|<span data-ttu-id="18b85-149">String</span><span class="sxs-lookup"><span data-stu-id="18b85-149">String</span></span>|<span data-ttu-id="18b85-150">自動操縦デバイスの名前を指定するときに使用するテンプレートを指定します。</span><span class="sxs-lookup"><span data-stu-id="18b85-150">The template used to name the AutoPilot Device.</span></span> <span data-ttu-id="18b85-151">これはカスタムテキストにすることができ、デバイスのシリアル番号またはランダムに生成された番号のいずれかを含めることもできます。</span><span class="sxs-lookup"><span data-stu-id="18b85-151">This can be a custom text and can also contain either the serial number of the device, or a randomly generated number.</span></span> <span data-ttu-id="18b85-152">テンプレートによって生成されるテキストの合計の長さは、15文字以下でなければなりません。</span><span class="sxs-lookup"><span data-stu-id="18b85-152">The total length of the text generated by the template can be no more than 15 characters.</span></span>|
|<span data-ttu-id="18b85-153">deviceType</span><span class="sxs-lookup"><span data-stu-id="18b85-153">deviceType</span></span>|[<span data-ttu-id="18b85-154">windowsAutopilotDeviceType</span><span class="sxs-lookup"><span data-stu-id="18b85-154">windowsAutopilotDeviceType</span></span>](../resources/intune-enrollment-windowsautopilotdevicetype.md)|<span data-ttu-id="18b85-155">このプロファイルを適用できる自動操縦デバイスの種類。</span><span class="sxs-lookup"><span data-stu-id="18b85-155">The AutoPilot device type that this profile is applicable to.</span></span> <span data-ttu-id="18b85-156">可能な値は、`windowsPc`、`surfaceHub2` です。</span><span class="sxs-lookup"><span data-stu-id="18b85-156">Possible values are: `windowsPc`, `surfaceHub2`.</span></span>|
|<span data-ttu-id="18b85-157">enableホワイトグローブ</span><span class="sxs-lookup"><span data-stu-id="18b85-157">enableWhiteGlove</span></span>|<span data-ttu-id="18b85-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="18b85-158">Boolean</span></span>|<span data-ttu-id="18b85-159">プロファイルの自動操縦白の手袋を有効にします。</span><span class="sxs-lookup"><span data-stu-id="18b85-159">Enable Autopilot White Glove for the profile.</span></span>|

## <a name="relationships"></a><span data-ttu-id="18b85-160">関係</span><span class="sxs-lookup"><span data-stu-id="18b85-160">Relationships</span></span>
|<span data-ttu-id="18b85-161">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="18b85-161">Relationship</span></span>|<span data-ttu-id="18b85-162">型</span><span class="sxs-lookup"><span data-stu-id="18b85-162">Type</span></span>|<span data-ttu-id="18b85-163">説明</span><span class="sxs-lookup"><span data-stu-id="18b85-163">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="18b85-164">assignedDevices</span><span class="sxs-lookup"><span data-stu-id="18b85-164">assignedDevices</span></span>|<span data-ttu-id="18b85-165">[windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="18b85-165">[windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) collection</span></span>|<span data-ttu-id="18b85-166">プロファイルに割り当てられているデバイスのリスト。</span><span class="sxs-lookup"><span data-stu-id="18b85-166">The list of assigned devices for the profile.</span></span>|
|<span data-ttu-id="18b85-167">assignments</span><span class="sxs-lookup"><span data-stu-id="18b85-167">assignments</span></span>|<span data-ttu-id="18b85-168">[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="18b85-168">[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) collection</span></span>|<span data-ttu-id="18b85-169">プロファイルのグループの割り当てのリスト。</span><span class="sxs-lookup"><span data-stu-id="18b85-169">The list of group assignments for the profile.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="18b85-170">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="18b85-170">JSON Representation</span></span>
<span data-ttu-id="18b85-171">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="18b85-171">Here is a JSON representation of the resource.</span></span>
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
  "enableWhiteGlove": true
}
```




