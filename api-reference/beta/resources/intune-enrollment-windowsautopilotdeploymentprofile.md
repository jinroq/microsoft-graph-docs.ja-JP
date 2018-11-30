---
title: windowsAutopilotDeploymentProfile リソースの種類
description: Windows 自動操縦装置の配置のプロファイル
ms.openlocfilehash: ed109af370d73d22d46198b206ba42dc4ebab2da
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067845"
---
# <a name="windowsautopilotdeploymentprofile-resource-type"></a><span data-ttu-id="dec2b-103">windowsAutopilotDeploymentProfile リソースの種類</span><span class="sxs-lookup"><span data-stu-id="dec2b-103">windowsAutopilotDeploymentProfile resource type</span></span>

> <span data-ttu-id="dec2b-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="dec2b-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dec2b-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dec2b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="dec2b-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="dec2b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="dec2b-107">Windows 自動操縦装置の配置のプロファイル</span><span class="sxs-lookup"><span data-stu-id="dec2b-107">Windows Autopilot Deployment Profile</span></span>
## <a name="methods"></a><span data-ttu-id="dec2b-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="dec2b-108">Methods</span></span>
|<span data-ttu-id="dec2b-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="dec2b-109">Method</span></span>|<span data-ttu-id="dec2b-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="dec2b-110">Return Type</span></span>|<span data-ttu-id="dec2b-111">説明</span><span class="sxs-lookup"><span data-stu-id="dec2b-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="dec2b-112">WindowsAutopilotDeploymentProfile を取得します。</span><span class="sxs-lookup"><span data-stu-id="dec2b-112">Get windowsAutopilotDeploymentProfile</span></span>](../api/intune-enrollment-windowsautopilotdeploymentprofile-get.md)|[<span data-ttu-id="dec2b-113">windowsAutopilotDeploymentProfile</span><span class="sxs-lookup"><span data-stu-id="dec2b-113">windowsAutopilotDeploymentProfile</span></span>](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)|<span data-ttu-id="dec2b-114">[WindowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="dec2b-114">Read properties and relationships of the [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md) object.</span></span>|
|[<span data-ttu-id="dec2b-115">assign action</span><span class="sxs-lookup"><span data-stu-id="dec2b-115">assign action</span></span>](../api/intune-enrollment-windowsautopilotdeploymentprofile-assign.md)|<span data-ttu-id="dec2b-116">なし</span><span class="sxs-lookup"><span data-stu-id="dec2b-116">None</span></span>|<span data-ttu-id="dec2b-117">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="dec2b-117">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="dec2b-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="dec2b-118">Properties</span></span>
|<span data-ttu-id="dec2b-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="dec2b-119">Property</span></span>|<span data-ttu-id="dec2b-120">型</span><span class="sxs-lookup"><span data-stu-id="dec2b-120">Type</span></span>|<span data-ttu-id="dec2b-121">説明</span><span class="sxs-lookup"><span data-stu-id="dec2b-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dec2b-122">id</span><span class="sxs-lookup"><span data-stu-id="dec2b-122">id</span></span>|<span data-ttu-id="dec2b-123">String</span><span class="sxs-lookup"><span data-stu-id="dec2b-123">String</span></span>|<span data-ttu-id="dec2b-124">プロファイル キー</span><span class="sxs-lookup"><span data-stu-id="dec2b-124">Profile Key</span></span>|
|<span data-ttu-id="dec2b-125">displayName</span><span class="sxs-lookup"><span data-stu-id="dec2b-125">displayName</span></span>|<span data-ttu-id="dec2b-126">String</span><span class="sxs-lookup"><span data-stu-id="dec2b-126">String</span></span>|<span data-ttu-id="dec2b-127">プロファイルの名前</span><span class="sxs-lookup"><span data-stu-id="dec2b-127">Name of the profile</span></span>|
|<span data-ttu-id="dec2b-128">説明</span><span class="sxs-lookup"><span data-stu-id="dec2b-128">description</span></span>|<span data-ttu-id="dec2b-129">String</span><span class="sxs-lookup"><span data-stu-id="dec2b-129">String</span></span>|<span data-ttu-id="dec2b-130">プロファイルの説明</span><span class="sxs-lookup"><span data-stu-id="dec2b-130">Description of the profile</span></span>|
|<span data-ttu-id="dec2b-131">language</span><span class="sxs-lookup"><span data-stu-id="dec2b-131">language</span></span>|<span data-ttu-id="dec2b-132">String</span><span class="sxs-lookup"><span data-stu-id="dec2b-132">String</span></span>|<span data-ttu-id="dec2b-133">デバイスで構成されている言語</span><span class="sxs-lookup"><span data-stu-id="dec2b-133">Language configured on the device</span></span>|
|<span data-ttu-id="dec2b-134">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="dec2b-134">createdDateTime</span></span>|<span data-ttu-id="dec2b-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dec2b-135">DateTimeOffset</span></span>|<span data-ttu-id="dec2b-136">プロファイルの作成時</span><span class="sxs-lookup"><span data-stu-id="dec2b-136">Profile creation time</span></span>|
|<span data-ttu-id="dec2b-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="dec2b-137">lastModifiedDateTime</span></span>|<span data-ttu-id="dec2b-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dec2b-138">DateTimeOffset</span></span>|<span data-ttu-id="dec2b-139">プロファイルの最終更新時刻</span><span class="sxs-lookup"><span data-stu-id="dec2b-139">Profile last modified time</span></span>|
|<span data-ttu-id="dec2b-140">outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="dec2b-140">outOfBoxExperienceSettings</span></span>|[<span data-ttu-id="dec2b-141">outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="dec2b-141">outOfBoxExperienceSettings</span></span>](../resources/intune-enrollment-outofboxexperiencesettings.md)|<span data-ttu-id="dec2b-142">ボックスの設定が発生します。</span><span class="sxs-lookup"><span data-stu-id="dec2b-142">Out of box experience setting</span></span>|
|<span data-ttu-id="dec2b-143">enrollmentStatusScreenSettings</span><span class="sxs-lookup"><span data-stu-id="dec2b-143">enrollmentStatusScreenSettings</span></span>|[<span data-ttu-id="dec2b-144">windowsEnrollmentStatusScreenSettings</span><span class="sxs-lookup"><span data-stu-id="dec2b-144">windowsEnrollmentStatusScreenSettings</span></span>](../resources/intune-enrollment-windowsenrollmentstatusscreensettings.md)|<span data-ttu-id="dec2b-145">登録ステータス画面の設定</span><span class="sxs-lookup"><span data-stu-id="dec2b-145">Enrollment status screen setting</span></span>|
|<span data-ttu-id="dec2b-146">extractHardwareHash</span><span class="sxs-lookup"><span data-stu-id="dec2b-146">extractHardwareHash</span></span>|<span data-ttu-id="dec2b-147">ブール値</span><span class="sxs-lookup"><span data-stu-id="dec2b-147">Boolean</span></span>|<span data-ttu-id="dec2b-148">プロファイルの HardwareHash の抽出</span><span class="sxs-lookup"><span data-stu-id="dec2b-148">HardwareHash Extraction for the profile</span></span>|
|<span data-ttu-id="dec2b-149">deviceNameTemplate</span><span class="sxs-lookup"><span data-stu-id="dec2b-149">deviceNameTemplate</span></span>|<span data-ttu-id="dec2b-150">String</span><span class="sxs-lookup"><span data-stu-id="dec2b-150">String</span></span>|<span data-ttu-id="dec2b-151">自動操縦装置のデバイスの名前を指定するために使用するテンプレートです。</span><span class="sxs-lookup"><span data-stu-id="dec2b-151">The template used to name the AutoPilot Device.</span></span> <span data-ttu-id="dec2b-152">これは、ユーザー設定のテキスト、デバイスのシリアル番号またはランダムに生成された番号のいずれかが含まれていることもできます。</span><span class="sxs-lookup"><span data-stu-id="dec2b-152">This can be a custom text and can also contain either the serial number of the device, or a randomly generated number.</span></span> <span data-ttu-id="dec2b-153">テンプレートによって生成されたテキストの長さの合計は、15 個以内の文字を使用できます。</span><span class="sxs-lookup"><span data-stu-id="dec2b-153">The total length of the text generated by the template can be no more than 15 characters.</span></span>|

## <a name="relationships"></a><span data-ttu-id="dec2b-154">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="dec2b-154">Relationships</span></span>
|<span data-ttu-id="dec2b-155">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="dec2b-155">Relationship</span></span>|<span data-ttu-id="dec2b-156">型</span><span class="sxs-lookup"><span data-stu-id="dec2b-156">Type</span></span>|<span data-ttu-id="dec2b-157">説明</span><span class="sxs-lookup"><span data-stu-id="dec2b-157">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dec2b-158">assignedDevices</span><span class="sxs-lookup"><span data-stu-id="dec2b-158">assignedDevices</span></span>|<span data-ttu-id="dec2b-159">[windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="dec2b-159">[windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) collection</span></span>|<span data-ttu-id="dec2b-160">プロファイルに割り当てられているデバイスの一覧です。</span><span class="sxs-lookup"><span data-stu-id="dec2b-160">The list of assigned devices for the profile.</span></span>|
|<span data-ttu-id="dec2b-161">assignments</span><span class="sxs-lookup"><span data-stu-id="dec2b-161">assignments</span></span>|<span data-ttu-id="dec2b-162">[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="dec2b-162">[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) collection</span></span>|<span data-ttu-id="dec2b-163">一連のプロファイルの割り当てをグループ化します。</span><span class="sxs-lookup"><span data-stu-id="dec2b-163">The list of group assignments for the profile.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="dec2b-164">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="dec2b-164">JSON Representation</span></span>
<span data-ttu-id="dec2b-165">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="dec2b-165">Here is a JSON representation of the resource.</span></span>
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





