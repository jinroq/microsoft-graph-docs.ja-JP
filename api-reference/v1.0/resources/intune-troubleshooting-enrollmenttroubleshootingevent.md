---
title: enrollmentTroubleshootingEvent リソースの種類
description: 登録エラーを表すイベント。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: aaf617e75c08c0f2be2e9351dc9a8b750a4b49b4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27985929"
---
# <a name="enrollmenttroubleshootingevent-resource-type"></a><span data-ttu-id="29e8e-103">enrollmentTroubleshootingEvent リソースの種類</span><span class="sxs-lookup"><span data-stu-id="29e8e-103">enrollmentTroubleshootingEvent resource type</span></span>

> <span data-ttu-id="29e8e-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="29e8e-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="29e8e-105">登録エラーを表すイベント。</span><span class="sxs-lookup"><span data-stu-id="29e8e-105">Event representing an enrollment failure.</span></span>

<span data-ttu-id="29e8e-106">[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="29e8e-106">Inherits from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>

## <a name="methods"></a><span data-ttu-id="29e8e-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="29e8e-107">Methods</span></span>
|<span data-ttu-id="29e8e-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="29e8e-108">Method</span></span>|<span data-ttu-id="29e8e-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="29e8e-109">Return Type</span></span>|<span data-ttu-id="29e8e-110">説明</span><span class="sxs-lookup"><span data-stu-id="29e8e-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="29e8e-111">List enrollmentTroubleshootingEvents</span><span class="sxs-lookup"><span data-stu-id="29e8e-111">List enrollmentTroubleshootingEvents</span></span>](../api/intune-troubleshooting-enrollmenttroubleshootingevent-list.md)|<span data-ttu-id="29e8e-112">[enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="29e8e-112">[enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) collection</span></span>|<span data-ttu-id="29e8e-113">[enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="29e8e-113">List properties and relationships of the [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) objects.</span></span>|
|[<span data-ttu-id="29e8e-114">Get enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="29e8e-114">Get enrollmentTroubleshootingEvent</span></span>](../api/intune-troubleshooting-enrollmenttroubleshootingevent-get.md)|[<span data-ttu-id="29e8e-115">enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="29e8e-115">enrollmentTroubleshootingEvent</span></span>](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md)|<span data-ttu-id="29e8e-116">[enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="29e8e-116">Read properties and relationships of the [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object.</span></span>|
|[<span data-ttu-id="29e8e-117">Create enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="29e8e-117">Create enrollmentTroubleshootingEvent</span></span>](../api/intune-troubleshooting-enrollmenttroubleshootingevent-create.md)|[<span data-ttu-id="29e8e-118">enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="29e8e-118">enrollmentTroubleshootingEvent</span></span>](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md)|<span data-ttu-id="29e8e-119">新しい [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="29e8e-119">Create a new [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object.</span></span>|
|[<span data-ttu-id="29e8e-120">Delete enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="29e8e-120">Delete enrollmentTroubleshootingEvent</span></span>](../api/intune-troubleshooting-enrollmenttroubleshootingevent-delete.md)|<span data-ttu-id="29e8e-121">なし</span><span class="sxs-lookup"><span data-stu-id="29e8e-121">None</span></span>|<span data-ttu-id="29e8e-122">[enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="29e8e-122">Deletes a [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md).</span></span>|
|[<span data-ttu-id="29e8e-123">Update enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="29e8e-123">Update enrollmentTroubleshootingEvent</span></span>](../api/intune-troubleshooting-enrollmenttroubleshootingevent-update.md)|[<span data-ttu-id="29e8e-124">enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="29e8e-124">enrollmentTroubleshootingEvent</span></span>](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md)|<span data-ttu-id="29e8e-125">[enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="29e8e-125">Update the properties of a [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="29e8e-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="29e8e-126">Properties</span></span>
|<span data-ttu-id="29e8e-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="29e8e-127">Property</span></span>|<span data-ttu-id="29e8e-128">型</span><span class="sxs-lookup"><span data-stu-id="29e8e-128">Type</span></span>|<span data-ttu-id="29e8e-129">説明</span><span class="sxs-lookup"><span data-stu-id="29e8e-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="29e8e-130">ID</span><span class="sxs-lookup"><span data-stu-id="29e8e-130">id</span></span>|<span data-ttu-id="29e8e-131">String</span><span class="sxs-lookup"><span data-stu-id="29e8e-131">String</span></span>|<span data-ttu-id="29e8e-132">オブジェクトの UUID。[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) から継承</span><span class="sxs-lookup"><span data-stu-id="29e8e-132">UUID for the object Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="29e8e-133">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="29e8e-133">eventDateTime</span></span>|<span data-ttu-id="29e8e-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="29e8e-134">DateTimeOffset</span></span>|<span data-ttu-id="29e8e-135">インシデントが発生した時間。</span><span class="sxs-lookup"><span data-stu-id="29e8e-135">Time when the event occurred .</span></span> <span data-ttu-id="29e8e-136">[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="29e8e-136">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="29e8e-137">correlationId</span><span class="sxs-lookup"><span data-stu-id="29e8e-137">correlationId</span></span>|<span data-ttu-id="29e8e-138">String</span><span class="sxs-lookup"><span data-stu-id="29e8e-138">String</span></span>|<span data-ttu-id="29e8e-139">サービスのエラーをトレースするための ID。</span><span class="sxs-lookup"><span data-stu-id="29e8e-139">Id used for tracing the failure in the service.</span></span> <span data-ttu-id="29e8e-140">[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="29e8e-140">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="29e8e-141">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="29e8e-141">managedDeviceIdentifier</span></span>|<span data-ttu-id="29e8e-142">String</span><span class="sxs-lookup"><span data-stu-id="29e8e-142">String</span></span>|<span data-ttu-id="29e8e-143">Intune によって作成または収集されるデバイス識別子。</span><span class="sxs-lookup"><span data-stu-id="29e8e-143">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="29e8e-144">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="29e8e-144">operatingSystem</span></span>|<span data-ttu-id="29e8e-145">String</span><span class="sxs-lookup"><span data-stu-id="29e8e-145">String</span></span>|<span data-ttu-id="29e8e-146">オペレーティング システム。</span><span class="sxs-lookup"><span data-stu-id="29e8e-146">Operating System.</span></span>|
|<span data-ttu-id="29e8e-147">osVersion</span><span class="sxs-lookup"><span data-stu-id="29e8e-147">osVersion</span></span>|<span data-ttu-id="29e8e-148">String</span><span class="sxs-lookup"><span data-stu-id="29e8e-148">String</span></span>|<span data-ttu-id="29e8e-149">OS バージョン。</span><span class="sxs-lookup"><span data-stu-id="29e8e-149">OS Version.</span></span>|
|<span data-ttu-id="29e8e-150">userId</span><span class="sxs-lookup"><span data-stu-id="29e8e-150">userId</span></span>|<span data-ttu-id="29e8e-151">String</span><span class="sxs-lookup"><span data-stu-id="29e8e-151">String</span></span>|<span data-ttu-id="29e8e-152">デバイスを登録しようとするユーザーの識別子。</span><span class="sxs-lookup"><span data-stu-id="29e8e-152">Identifier for the user that tried to enroll the device.</span></span>|
|<span data-ttu-id="29e8e-153">deviceId</span><span class="sxs-lookup"><span data-stu-id="29e8e-153">deviceId</span></span>|<span data-ttu-id="29e8e-154">String</span><span class="sxs-lookup"><span data-stu-id="29e8e-154">String</span></span>|<span data-ttu-id="29e8e-155">Azure AD デバイス識別子。</span><span class="sxs-lookup"><span data-stu-id="29e8e-155">Azure AD device identifier.</span></span>|
|<span data-ttu-id="29e8e-156">enrollmentType</span><span class="sxs-lookup"><span data-stu-id="29e8e-156">enrollmentType</span></span>|[<span data-ttu-id="29e8e-157">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="29e8e-157">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="29e8e-158">登録の種類。</span><span class="sxs-lookup"><span data-stu-id="29e8e-158">Type of the enrollment.</span></span> <span data-ttu-id="29e8e-159">可能な値は、`unknown`、`userEnrollment`、`deviceEnrollmentManager`、`appleBulkWithUser`、`appleBulkWithoutUser`、`windowsAzureADJoin`、`windowsBulkUserless`、`windowsAutoEnrollment`、`windowsBulkAzureDomainJoin`、`windowsCoManagement` です。</span><span class="sxs-lookup"><span data-stu-id="29e8e-159">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span></span>|
|<span data-ttu-id="29e8e-160">failureCategory</span><span class="sxs-lookup"><span data-stu-id="29e8e-160">failureCategory</span></span>|[<span data-ttu-id="29e8e-161">deviceEnrollmentFailureReason</span><span class="sxs-lookup"><span data-stu-id="29e8e-161">deviceEnrollmentFailureReason</span></span>](../resources/intune-troubleshooting-deviceenrollmentfailurereason.md)|<span data-ttu-id="29e8e-162">高レベルのエラー カテゴリ。</span><span class="sxs-lookup"><span data-stu-id="29e8e-162">Highlevel failure category.</span></span> <span data-ttu-id="29e8e-163">可能な値は、`unknown`、`authentication`、`authorization`、`accountValidation`、`userValidation`、`deviceNotSupported`、`inMaintenance`、`badRequest`、`featureNotSupported`、`enrollmentRestrictionsEnforced`、`clientDisconnected`、`userAbandonment` です。</span><span class="sxs-lookup"><span data-stu-id="29e8e-163">Possible values are: `unknown`, `authentication`, `authorization`, `accountValidation`, `userValidation`, `deviceNotSupported`, `inMaintenance`, `badRequest`, `featureNotSupported`, `enrollmentRestrictionsEnforced`, `clientDisconnected`, `userAbandonment`.</span></span>|
|<span data-ttu-id="29e8e-164">failureReason</span><span class="sxs-lookup"><span data-stu-id="29e8e-164">failureReason</span></span>|<span data-ttu-id="29e8e-165">String</span><span class="sxs-lookup"><span data-stu-id="29e8e-165">String</span></span>|<span data-ttu-id="29e8e-166">詳細なエラーの理由:</span><span class="sxs-lookup"><span data-stu-id="29e8e-166">Detailed failure reason.</span></span>|

## <a name="relationships"></a><span data-ttu-id="29e8e-167">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="29e8e-167">Relationships</span></span>
<span data-ttu-id="29e8e-168">なし</span><span class="sxs-lookup"><span data-stu-id="29e8e-168">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="29e8e-169">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="29e8e-169">JSON Representation</span></span>
<span data-ttu-id="29e8e-170">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="29e8e-170">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.enrollmentTroubleshootingEvent"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.enrollmentTroubleshootingEvent",
  "id": "String (identifier)",
  "eventDateTime": "String (timestamp)",
  "correlationId": "String",
  "managedDeviceIdentifier": "String",
  "operatingSystem": "String",
  "osVersion": "String",
  "userId": "String",
  "deviceId": "String",
  "enrollmentType": "String",
  "failureCategory": "String",
  "failureReason": "String"
}
```

<!-- {
  "type": "#page.annotation",
  "suppressions": [
     "Warning: Enum deviceEnrollmentFailureReason has some values specified and others unspecified."
  ],
}
-->



