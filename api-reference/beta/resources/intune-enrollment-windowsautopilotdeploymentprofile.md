---
title: windowsAutopilotDeploymentProfile リソースの種類
description: Windows 自動操縦展開プロファイル
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b3b815e0184ab9969af348338c07c3fabf0b0597
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30168874"
---
# <a name="windowsautopilotdeploymentprofile-resource-type"></a><span data-ttu-id="8793d-103">windowsAutopilotDeploymentProfile リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8793d-103">windowsAutopilotDeploymentProfile resource type</span></span>

> <span data-ttu-id="8793d-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8793d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8793d-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="8793d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8793d-106">Windows 自動操縦展開プロファイル</span><span class="sxs-lookup"><span data-stu-id="8793d-106">Windows Autopilot Deployment Profile</span></span>

## <a name="methods"></a><span data-ttu-id="8793d-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="8793d-107">Methods</span></span>
|<span data-ttu-id="8793d-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="8793d-108">Method</span></span>|<span data-ttu-id="8793d-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="8793d-109">Return Type</span></span>|<span data-ttu-id="8793d-110">説明</span><span class="sxs-lookup"><span data-stu-id="8793d-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="8793d-111">windowsAutopilotDeploymentProfile を取得する</span><span class="sxs-lookup"><span data-stu-id="8793d-111">Get windowsAutopilotDeploymentProfile</span></span>](../api/intune-enrollment-windowsautopilotdeploymentprofile-get.md)|[<span data-ttu-id="8793d-112">windowsAutopilotDeploymentProfile</span><span class="sxs-lookup"><span data-stu-id="8793d-112">windowsAutopilotDeploymentProfile</span></span>](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)|<span data-ttu-id="8793d-113">[windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="8793d-113">Read properties and relationships of the [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md) object.</span></span>|
|[<span data-ttu-id="8793d-114">assign action</span><span class="sxs-lookup"><span data-stu-id="8793d-114">assign action</span></span>](../api/intune-enrollment-windowsautopilotdeploymentprofile-assign.md)|<span data-ttu-id="8793d-115">なし</span><span class="sxs-lookup"><span data-stu-id="8793d-115">None</span></span>|<span data-ttu-id="8793d-116">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="8793d-116">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="8793d-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8793d-117">Properties</span></span>
|<span data-ttu-id="8793d-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8793d-118">Property</span></span>|<span data-ttu-id="8793d-119">型</span><span class="sxs-lookup"><span data-stu-id="8793d-119">Type</span></span>|<span data-ttu-id="8793d-120">説明</span><span class="sxs-lookup"><span data-stu-id="8793d-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8793d-121">id</span><span class="sxs-lookup"><span data-stu-id="8793d-121">id</span></span>|<span data-ttu-id="8793d-122">文字列</span><span class="sxs-lookup"><span data-stu-id="8793d-122">String</span></span>|<span data-ttu-id="8793d-123">プロファイルキー</span><span class="sxs-lookup"><span data-stu-id="8793d-123">Profile Key</span></span>|
|<span data-ttu-id="8793d-124">displayName</span><span class="sxs-lookup"><span data-stu-id="8793d-124">displayName</span></span>|<span data-ttu-id="8793d-125">String</span><span class="sxs-lookup"><span data-stu-id="8793d-125">String</span></span>|<span data-ttu-id="8793d-126">プロファイルの名前</span><span class="sxs-lookup"><span data-stu-id="8793d-126">Name of the profile</span></span>|
|<span data-ttu-id="8793d-127">説明</span><span class="sxs-lookup"><span data-stu-id="8793d-127">description</span></span>|<span data-ttu-id="8793d-128">文字列</span><span class="sxs-lookup"><span data-stu-id="8793d-128">String</span></span>|<span data-ttu-id="8793d-129">プロファイルの説明</span><span class="sxs-lookup"><span data-stu-id="8793d-129">Description of the profile</span></span>|
|<span data-ttu-id="8793d-130">language</span><span class="sxs-lookup"><span data-stu-id="8793d-130">language</span></span>|<span data-ttu-id="8793d-131">String</span><span class="sxs-lookup"><span data-stu-id="8793d-131">String</span></span>|<span data-ttu-id="8793d-132">デバイスで構成されている言語</span><span class="sxs-lookup"><span data-stu-id="8793d-132">Language configured on the device</span></span>|
|<span data-ttu-id="8793d-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8793d-133">createdDateTime</span></span>|<span data-ttu-id="8793d-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8793d-134">DateTimeOffset</span></span>|<span data-ttu-id="8793d-135">プロファイルの作成時刻</span><span class="sxs-lookup"><span data-stu-id="8793d-135">Profile creation time</span></span>|
|<span data-ttu-id="8793d-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8793d-136">lastModifiedDateTime</span></span>|<span data-ttu-id="8793d-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8793d-137">DateTimeOffset</span></span>|<span data-ttu-id="8793d-138">プロファイルの最終変更日時</span><span class="sxs-lookup"><span data-stu-id="8793d-138">Profile last modified time</span></span>|
|<span data-ttu-id="8793d-139">outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="8793d-139">outOfBoxExperienceSettings</span></span>|[<span data-ttu-id="8793d-140">outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="8793d-140">outOfBoxExperienceSettings</span></span>](../resources/intune-enrollment-outofboxexperiencesettings.md)|<span data-ttu-id="8793d-141">不在時の環境設定</span><span class="sxs-lookup"><span data-stu-id="8793d-141">Out of box experience setting</span></span>|
|<span data-ttu-id="8793d-142">enrollmentStatusScreenSettings</span><span class="sxs-lookup"><span data-stu-id="8793d-142">enrollmentStatusScreenSettings</span></span>|[<span data-ttu-id="8793d-143">windowsEnrollmentStatusScreenSettings</span><span class="sxs-lookup"><span data-stu-id="8793d-143">windowsEnrollmentStatusScreenSettings</span></span>](../resources/intune-enrollment-windowsenrollmentstatusscreensettings.md)|<span data-ttu-id="8793d-144">登録の状態画面の設定</span><span class="sxs-lookup"><span data-stu-id="8793d-144">Enrollment status screen setting</span></span>|
|<span data-ttu-id="8793d-145">extractHardwareHash</span><span class="sxs-lookup"><span data-stu-id="8793d-145">extractHardwareHash</span></span>|<span data-ttu-id="8793d-146">ブール値</span><span class="sxs-lookup"><span data-stu-id="8793d-146">Boolean</span></span>|<span data-ttu-id="8793d-147">プロファイルのハードウェアハッシュ抽出</span><span class="sxs-lookup"><span data-stu-id="8793d-147">HardwareHash Extraction for the profile</span></span>|
|<span data-ttu-id="8793d-148">deviceNameTemplate</span><span class="sxs-lookup"><span data-stu-id="8793d-148">deviceNameTemplate</span></span>|<span data-ttu-id="8793d-149">String</span><span class="sxs-lookup"><span data-stu-id="8793d-149">String</span></span>|<span data-ttu-id="8793d-150">自動操縦デバイスの名前を指定するときに使用するテンプレートを指定します。</span><span class="sxs-lookup"><span data-stu-id="8793d-150">The template used to name the AutoPilot Device.</span></span> <span data-ttu-id="8793d-151">これはカスタムテキストにすることができ、デバイスのシリアル番号またはランダムに生成された番号のいずれかを含めることもできます。</span><span class="sxs-lookup"><span data-stu-id="8793d-151">This can be a custom text and can also contain either the serial number of the device, or a randomly generated number.</span></span> <span data-ttu-id="8793d-152">テンプレートによって生成されるテキストの合計の長さは、15文字以下でなければなりません。</span><span class="sxs-lookup"><span data-stu-id="8793d-152">The total length of the text generated by the template can be no more than 15 characters.</span></span>|
|<span data-ttu-id="8793d-153">enableホワイトグローブ</span><span class="sxs-lookup"><span data-stu-id="8793d-153">enableWhiteGlove</span></span>|<span data-ttu-id="8793d-154">ブール値</span><span class="sxs-lookup"><span data-stu-id="8793d-154">Boolean</span></span>|<span data-ttu-id="8793d-155">プロファイルの自動操縦白の手袋を有効にします。</span><span class="sxs-lookup"><span data-stu-id="8793d-155">Enable Autopilot White Glove for the profile.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8793d-156">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="8793d-156">Relationships</span></span>
|<span data-ttu-id="8793d-157">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="8793d-157">Relationship</span></span>|<span data-ttu-id="8793d-158">型</span><span class="sxs-lookup"><span data-stu-id="8793d-158">Type</span></span>|<span data-ttu-id="8793d-159">説明</span><span class="sxs-lookup"><span data-stu-id="8793d-159">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8793d-160">assignedDevices</span><span class="sxs-lookup"><span data-stu-id="8793d-160">assignedDevices</span></span>|<span data-ttu-id="8793d-161">[windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="8793d-161">[windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) collection</span></span>|<span data-ttu-id="8793d-162">プロファイルに割り当てられているデバイスのリスト。</span><span class="sxs-lookup"><span data-stu-id="8793d-162">The list of assigned devices for the profile.</span></span>|
|<span data-ttu-id="8793d-163">assignments</span><span class="sxs-lookup"><span data-stu-id="8793d-163">assignments</span></span>|<span data-ttu-id="8793d-164">[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="8793d-164">[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) collection</span></span>|<span data-ttu-id="8793d-165">プロファイルのグループの割り当てのリスト。</span><span class="sxs-lookup"><span data-stu-id="8793d-165">The list of group assignments for the profile.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8793d-166">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8793d-166">JSON Representation</span></span>
<span data-ttu-id="8793d-167">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="8793d-167">Here is a JSON representation of the resource.</span></span>
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
  "enableWhiteGlove": true
}
```




