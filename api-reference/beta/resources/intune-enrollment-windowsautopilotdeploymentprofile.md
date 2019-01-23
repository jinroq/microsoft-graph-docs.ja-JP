---
title: windowsAutopilotDeploymentProfile リソースの種類
description: Windows 自動操縦装置の配置のプロファイル
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 7f97603980f4e76c4dd2f63287822a1e8e984ded
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29394111"
---
# <a name="windowsautopilotdeploymentprofile-resource-type"></a><span data-ttu-id="78580-103">windowsAutopilotDeploymentProfile リソースの種類</span><span class="sxs-lookup"><span data-stu-id="78580-103">windowsAutopilotDeploymentProfile resource type</span></span>

> <span data-ttu-id="78580-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="78580-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="78580-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="78580-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="78580-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="78580-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="78580-107">Windows 自動操縦装置の配置のプロファイル</span><span class="sxs-lookup"><span data-stu-id="78580-107">Windows Autopilot Deployment Profile</span></span>

## <a name="methods"></a><span data-ttu-id="78580-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="78580-108">Methods</span></span>
|<span data-ttu-id="78580-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="78580-109">Method</span></span>|<span data-ttu-id="78580-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="78580-110">Return Type</span></span>|<span data-ttu-id="78580-111">説明</span><span class="sxs-lookup"><span data-stu-id="78580-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="78580-112">WindowsAutopilotDeploymentProfile を取得します。</span><span class="sxs-lookup"><span data-stu-id="78580-112">Get windowsAutopilotDeploymentProfile</span></span>](../api/intune-enrollment-windowsautopilotdeploymentprofile-get.md)|[<span data-ttu-id="78580-113">windowsAutopilotDeploymentProfile</span><span class="sxs-lookup"><span data-stu-id="78580-113">windowsAutopilotDeploymentProfile</span></span>](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)|<span data-ttu-id="78580-114">[WindowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="78580-114">Read properties and relationships of the [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md) object.</span></span>|
|[<span data-ttu-id="78580-115">assign action</span><span class="sxs-lookup"><span data-stu-id="78580-115">assign action</span></span>](../api/intune-enrollment-windowsautopilotdeploymentprofile-assign.md)|<span data-ttu-id="78580-116">なし</span><span class="sxs-lookup"><span data-stu-id="78580-116">None</span></span>|<span data-ttu-id="78580-117">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="78580-117">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="78580-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="78580-118">Properties</span></span>
|<span data-ttu-id="78580-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="78580-119">Property</span></span>|<span data-ttu-id="78580-120">型</span><span class="sxs-lookup"><span data-stu-id="78580-120">Type</span></span>|<span data-ttu-id="78580-121">説明</span><span class="sxs-lookup"><span data-stu-id="78580-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="78580-122">id</span><span class="sxs-lookup"><span data-stu-id="78580-122">id</span></span>|<span data-ttu-id="78580-123">String</span><span class="sxs-lookup"><span data-stu-id="78580-123">String</span></span>|<span data-ttu-id="78580-124">プロファイル キー</span><span class="sxs-lookup"><span data-stu-id="78580-124">Profile Key</span></span>|
|<span data-ttu-id="78580-125">displayName</span><span class="sxs-lookup"><span data-stu-id="78580-125">displayName</span></span>|<span data-ttu-id="78580-126">String</span><span class="sxs-lookup"><span data-stu-id="78580-126">String</span></span>|<span data-ttu-id="78580-127">プロファイルの名前</span><span class="sxs-lookup"><span data-stu-id="78580-127">Name of the profile</span></span>|
|<span data-ttu-id="78580-128">説明</span><span class="sxs-lookup"><span data-stu-id="78580-128">description</span></span>|<span data-ttu-id="78580-129">String</span><span class="sxs-lookup"><span data-stu-id="78580-129">String</span></span>|<span data-ttu-id="78580-130">プロファイルの説明</span><span class="sxs-lookup"><span data-stu-id="78580-130">Description of the profile</span></span>|
|<span data-ttu-id="78580-131">language</span><span class="sxs-lookup"><span data-stu-id="78580-131">language</span></span>|<span data-ttu-id="78580-132">String</span><span class="sxs-lookup"><span data-stu-id="78580-132">String</span></span>|<span data-ttu-id="78580-133">デバイスで構成されている言語</span><span class="sxs-lookup"><span data-stu-id="78580-133">Language configured on the device</span></span>|
|<span data-ttu-id="78580-134">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="78580-134">createdDateTime</span></span>|<span data-ttu-id="78580-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="78580-135">DateTimeOffset</span></span>|<span data-ttu-id="78580-136">プロファイルの作成時</span><span class="sxs-lookup"><span data-stu-id="78580-136">Profile creation time</span></span>|
|<span data-ttu-id="78580-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="78580-137">lastModifiedDateTime</span></span>|<span data-ttu-id="78580-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="78580-138">DateTimeOffset</span></span>|<span data-ttu-id="78580-139">プロファイルの最終更新時刻</span><span class="sxs-lookup"><span data-stu-id="78580-139">Profile last modified time</span></span>|
|<span data-ttu-id="78580-140">outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="78580-140">outOfBoxExperienceSettings</span></span>|[<span data-ttu-id="78580-141">outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="78580-141">outOfBoxExperienceSettings</span></span>](../resources/intune-enrollment-outofboxexperiencesettings.md)|<span data-ttu-id="78580-142">ボックスの設定が発生します。</span><span class="sxs-lookup"><span data-stu-id="78580-142">Out of box experience setting</span></span>|
|<span data-ttu-id="78580-143">enrollmentStatusScreenSettings</span><span class="sxs-lookup"><span data-stu-id="78580-143">enrollmentStatusScreenSettings</span></span>|[<span data-ttu-id="78580-144">windowsEnrollmentStatusScreenSettings</span><span class="sxs-lookup"><span data-stu-id="78580-144">windowsEnrollmentStatusScreenSettings</span></span>](../resources/intune-enrollment-windowsenrollmentstatusscreensettings.md)|<span data-ttu-id="78580-145">登録ステータス画面の設定</span><span class="sxs-lookup"><span data-stu-id="78580-145">Enrollment status screen setting</span></span>|
|<span data-ttu-id="78580-146">extractHardwareHash</span><span class="sxs-lookup"><span data-stu-id="78580-146">extractHardwareHash</span></span>|<span data-ttu-id="78580-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="78580-147">Boolean</span></span>|<span data-ttu-id="78580-148">プロファイルの HardwareHash の抽出</span><span class="sxs-lookup"><span data-stu-id="78580-148">HardwareHash Extraction for the profile</span></span>|
|<span data-ttu-id="78580-149">deviceNameTemplate</span><span class="sxs-lookup"><span data-stu-id="78580-149">deviceNameTemplate</span></span>|<span data-ttu-id="78580-150">String</span><span class="sxs-lookup"><span data-stu-id="78580-150">String</span></span>|<span data-ttu-id="78580-151">自動操縦装置のデバイスの名前を指定するために使用するテンプレートです。</span><span class="sxs-lookup"><span data-stu-id="78580-151">The template used to name the AutoPilot Device.</span></span> <span data-ttu-id="78580-152">これは、ユーザー設定のテキスト、デバイスのシリアル番号またはランダムに生成された番号のいずれかが含まれていることもできます。</span><span class="sxs-lookup"><span data-stu-id="78580-152">This can be a custom text and can also contain either the serial number of the device, or a randomly generated number.</span></span> <span data-ttu-id="78580-153">テンプレートによって生成されたテキストの長さの合計は、15 個以内の文字を使用できます。</span><span class="sxs-lookup"><span data-stu-id="78580-153">The total length of the text generated by the template can be no more than 15 characters.</span></span>|

## <a name="relationships"></a><span data-ttu-id="78580-154">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="78580-154">Relationships</span></span>
|<span data-ttu-id="78580-155">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="78580-155">Relationship</span></span>|<span data-ttu-id="78580-156">型</span><span class="sxs-lookup"><span data-stu-id="78580-156">Type</span></span>|<span data-ttu-id="78580-157">説明</span><span class="sxs-lookup"><span data-stu-id="78580-157">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="78580-158">assignedDevices</span><span class="sxs-lookup"><span data-stu-id="78580-158">assignedDevices</span></span>|<span data-ttu-id="78580-159">[windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="78580-159">[windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) collection</span></span>|<span data-ttu-id="78580-160">プロファイルに割り当てられているデバイスの一覧です。</span><span class="sxs-lookup"><span data-stu-id="78580-160">The list of assigned devices for the profile.</span></span>|
|<span data-ttu-id="78580-161">assignments</span><span class="sxs-lookup"><span data-stu-id="78580-161">assignments</span></span>|<span data-ttu-id="78580-162">[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="78580-162">[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) collection</span></span>|<span data-ttu-id="78580-163">一連のプロファイルの割り当てをグループ化します。</span><span class="sxs-lookup"><span data-stu-id="78580-163">The list of group assignments for the profile.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="78580-164">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="78580-164">JSON Representation</span></span>
<span data-ttu-id="78580-165">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="78580-165">Here is a JSON representation of the resource.</span></span>
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
  "deviceNameTemplate": "String"
}
```




