---
title: enrollmentTroubleshootingEvent リソースの種類
description: 登録エラーを表すイベント。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 1d79a85c979eb7f8c4dd734724f5a984b814e724
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27987777"
---
# <a name="enrollmenttroubleshootingevent-resource-type"></a><span data-ttu-id="c22a7-103">enrollmentTroubleshootingEvent リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c22a7-103">enrollmentTroubleshootingEvent resource type</span></span>

> <span data-ttu-id="c22a7-104">**重要:** Microsoft Graph のベータ版の API はプレビュー中で、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c22a7-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c22a7-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c22a7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c22a7-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="c22a7-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c22a7-107">登録エラーを表すイベント。</span><span class="sxs-lookup"><span data-stu-id="c22a7-107">Event representing an enrollment failure.</span></span>

<span data-ttu-id="c22a7-108">[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="c22a7-108">Inherits from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>

## <a name="methods"></a><span data-ttu-id="c22a7-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="c22a7-109">Methods</span></span>
|<span data-ttu-id="c22a7-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="c22a7-110">Method</span></span>|<span data-ttu-id="c22a7-111">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="c22a7-111">Return Type</span></span>|<span data-ttu-id="c22a7-112">説明</span><span class="sxs-lookup"><span data-stu-id="c22a7-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c22a7-113">List enrollmentTroubleshootingEvents</span><span class="sxs-lookup"><span data-stu-id="c22a7-113">List enrollmentTroubleshootingEvents</span></span>](../api/intune-troubleshooting-enrollmenttroubleshootingevent-list.md)|<span data-ttu-id="c22a7-114">[enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="c22a7-114">[enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) collection</span></span>|<span data-ttu-id="c22a7-115">[enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="c22a7-115">List properties and relationships of the [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) objects.</span></span>|
|[<span data-ttu-id="c22a7-116">Get enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="c22a7-116">Get enrollmentTroubleshootingEvent</span></span>](../api/intune-troubleshooting-enrollmenttroubleshootingevent-get.md)|[<span data-ttu-id="c22a7-117">enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="c22a7-117">enrollmentTroubleshootingEvent</span></span>](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md)|<span data-ttu-id="c22a7-118">[enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="c22a7-118">Read properties and relationships of the [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object.</span></span>|
|[<span data-ttu-id="c22a7-119">Create enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="c22a7-119">Create enrollmentTroubleshootingEvent</span></span>](../api/intune-troubleshooting-enrollmenttroubleshootingevent-create.md)|[<span data-ttu-id="c22a7-120">enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="c22a7-120">enrollmentTroubleshootingEvent</span></span>](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md)|<span data-ttu-id="c22a7-121">新しい [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="c22a7-121">Create a new [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object.</span></span>|
|[<span data-ttu-id="c22a7-122">Delete enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="c22a7-122">Delete enrollmentTroubleshootingEvent</span></span>](../api/intune-troubleshooting-enrollmenttroubleshootingevent-delete.md)|<span data-ttu-id="c22a7-123">なし</span><span class="sxs-lookup"><span data-stu-id="c22a7-123">None</span></span>|<span data-ttu-id="c22a7-124">[enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="c22a7-124">Deletes a [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md).</span></span>|
|[<span data-ttu-id="c22a7-125">Update enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="c22a7-125">Update enrollmentTroubleshootingEvent</span></span>](../api/intune-troubleshooting-enrollmenttroubleshootingevent-update.md)|[<span data-ttu-id="c22a7-126">enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="c22a7-126">enrollmentTroubleshootingEvent</span></span>](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md)|<span data-ttu-id="c22a7-127">[enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="c22a7-127">Update the properties of a [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="c22a7-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c22a7-128">Properties</span></span>
|<span data-ttu-id="c22a7-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c22a7-129">Property</span></span>|<span data-ttu-id="c22a7-130">型</span><span class="sxs-lookup"><span data-stu-id="c22a7-130">Type</span></span>|<span data-ttu-id="c22a7-131">説明</span><span class="sxs-lookup"><span data-stu-id="c22a7-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c22a7-132">ID</span><span class="sxs-lookup"><span data-stu-id="c22a7-132">id</span></span>|<span data-ttu-id="c22a7-133">String</span><span class="sxs-lookup"><span data-stu-id="c22a7-133">String</span></span>|<span data-ttu-id="c22a7-134">オブジェクトの UUID。[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) から継承</span><span class="sxs-lookup"><span data-stu-id="c22a7-134">UUID for the object Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="c22a7-135">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="c22a7-135">eventDateTime</span></span>|<span data-ttu-id="c22a7-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c22a7-136">DateTimeOffset</span></span>|<span data-ttu-id="c22a7-137">インシデントが発生した時間。</span><span class="sxs-lookup"><span data-stu-id="c22a7-137">Time when the event occurred .</span></span> <span data-ttu-id="c22a7-138">[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c22a7-138">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="c22a7-139">correlationId</span><span class="sxs-lookup"><span data-stu-id="c22a7-139">correlationId</span></span>|<span data-ttu-id="c22a7-140">String</span><span class="sxs-lookup"><span data-stu-id="c22a7-140">String</span></span>|<span data-ttu-id="c22a7-141">サービスのエラーをトレースするための ID。</span><span class="sxs-lookup"><span data-stu-id="c22a7-141">Id used for tracing the failure in the service.</span></span> <span data-ttu-id="c22a7-142">[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c22a7-142">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="c22a7-143">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="c22a7-143">managedDeviceIdentifier</span></span>|<span data-ttu-id="c22a7-144">String</span><span class="sxs-lookup"><span data-stu-id="c22a7-144">String</span></span>|<span data-ttu-id="c22a7-145">Intune によって作成または収集されるデバイス識別子。</span><span class="sxs-lookup"><span data-stu-id="c22a7-145">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="c22a7-146">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="c22a7-146">operatingSystem</span></span>|<span data-ttu-id="c22a7-147">String</span><span class="sxs-lookup"><span data-stu-id="c22a7-147">String</span></span>|<span data-ttu-id="c22a7-148">オペレーティング システム。</span><span class="sxs-lookup"><span data-stu-id="c22a7-148">Operating System.</span></span>|
|<span data-ttu-id="c22a7-149">osVersion</span><span class="sxs-lookup"><span data-stu-id="c22a7-149">osVersion</span></span>|<span data-ttu-id="c22a7-150">String</span><span class="sxs-lookup"><span data-stu-id="c22a7-150">String</span></span>|<span data-ttu-id="c22a7-151">OS バージョン。</span><span class="sxs-lookup"><span data-stu-id="c22a7-151">OS Version.</span></span>|
|<span data-ttu-id="c22a7-152">userId</span><span class="sxs-lookup"><span data-stu-id="c22a7-152">userId</span></span>|<span data-ttu-id="c22a7-153">String</span><span class="sxs-lookup"><span data-stu-id="c22a7-153">String</span></span>|<span data-ttu-id="c22a7-154">デバイスを登録しようとするユーザーの識別子。</span><span class="sxs-lookup"><span data-stu-id="c22a7-154">Identifier for the user that tried to enroll the device.</span></span>|
|<span data-ttu-id="c22a7-155">deviceId</span><span class="sxs-lookup"><span data-stu-id="c22a7-155">deviceId</span></span>|<span data-ttu-id="c22a7-156">String</span><span class="sxs-lookup"><span data-stu-id="c22a7-156">String</span></span>|<span data-ttu-id="c22a7-157">Azure AD デバイス識別子。</span><span class="sxs-lookup"><span data-stu-id="c22a7-157">Azure AD device identifier.</span></span>|
|<span data-ttu-id="c22a7-158">enrollmentType</span><span class="sxs-lookup"><span data-stu-id="c22a7-158">enrollmentType</span></span>|[<span data-ttu-id="c22a7-159">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="c22a7-159">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="c22a7-160">登録の種類。</span><span class="sxs-lookup"><span data-stu-id="c22a7-160">Type of the enrollment.</span></span> <span data-ttu-id="c22a7-161">可能な値は、`unknown`、`userEnrollment`、`deviceEnrollmentManager`、`appleBulkWithUser`、`appleBulkWithoutUser`、`windowsAzureADJoin`、`windowsBulkUserless`、`windowsAutoEnrollment`、`windowsBulkAzureDomainJoin`、`windowsCoManagement` です。</span><span class="sxs-lookup"><span data-stu-id="c22a7-161">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span></span>|
|<span data-ttu-id="c22a7-162">failureCategory</span><span class="sxs-lookup"><span data-stu-id="c22a7-162">failureCategory</span></span>|[<span data-ttu-id="c22a7-163">deviceEnrollmentFailureReason</span><span class="sxs-lookup"><span data-stu-id="c22a7-163">deviceEnrollmentFailureReason</span></span>](../resources/intune-troubleshooting-deviceenrollmentfailurereason.md)|<span data-ttu-id="c22a7-164">高レベルのエラー カテゴリ。</span><span class="sxs-lookup"><span data-stu-id="c22a7-164">Highlevel failure category.</span></span> <span data-ttu-id="c22a7-165">可能な値は、`unknown`、`authentication`、`authorization`、`accountValidation`、`userValidation`、`deviceNotSupported`、`inMaintenance`、`badRequest`、`featureNotSupported`、`enrollmentRestrictionsEnforced`、`clientDisconnected`、`userAbandonment` です。</span><span class="sxs-lookup"><span data-stu-id="c22a7-165">Possible values are: `unknown`, `authentication`, `authorization`, `accountValidation`, `userValidation`, `deviceNotSupported`, `inMaintenance`, `badRequest`, `featureNotSupported`, `enrollmentRestrictionsEnforced`, `clientDisconnected`, `userAbandonment`.</span></span>|
|<span data-ttu-id="c22a7-166">failureReason</span><span class="sxs-lookup"><span data-stu-id="c22a7-166">failureReason</span></span>|<span data-ttu-id="c22a7-167">String</span><span class="sxs-lookup"><span data-stu-id="c22a7-167">String</span></span>|<span data-ttu-id="c22a7-168">詳細なエラーの理由:</span><span class="sxs-lookup"><span data-stu-id="c22a7-168">Detailed failure reason.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c22a7-169">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="c22a7-169">Relationships</span></span>
<span data-ttu-id="c22a7-170">なし</span><span class="sxs-lookup"><span data-stu-id="c22a7-170">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c22a7-171">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c22a7-171">JSON Representation</span></span>
<span data-ttu-id="c22a7-172">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="c22a7-172">Here is a JSON representation of the resource.</span></span>
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





