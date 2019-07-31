---
title: enrollmentTroubleshootingEvent リソースの種類
description: 登録エラーを表すイベント。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 722bd139bda92e09f7a49489968754952d8aca39
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36010304"
---
# <a name="enrollmenttroubleshootingevent-resource-type"></a><span data-ttu-id="175a6-103">enrollmentTroubleshootingEvent リソースの種類</span><span class="sxs-lookup"><span data-stu-id="175a6-103">enrollmentTroubleshootingEvent resource type</span></span>

> <span data-ttu-id="175a6-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="175a6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="175a6-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="175a6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="175a6-106">登録エラーを表すイベント。</span><span class="sxs-lookup"><span data-stu-id="175a6-106">Event representing an enrollment failure.</span></span>


<span data-ttu-id="175a6-107">[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="175a6-107">Inherits from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>

## <a name="methods"></a><span data-ttu-id="175a6-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="175a6-108">Methods</span></span>
|<span data-ttu-id="175a6-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="175a6-109">Method</span></span>|<span data-ttu-id="175a6-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="175a6-110">Return Type</span></span>|<span data-ttu-id="175a6-111">説明</span><span class="sxs-lookup"><span data-stu-id="175a6-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="175a6-112">List enrollmentTroubleshootingEvents</span><span class="sxs-lookup"><span data-stu-id="175a6-112">List enrollmentTroubleshootingEvents</span></span>](../api/intune-troubleshooting-enrollmenttroubleshootingevent-list.md)|<span data-ttu-id="175a6-113">[enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="175a6-113">[enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) collection</span></span>|<span data-ttu-id="175a6-114">[enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="175a6-114">List properties and relationships of the [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) objects.</span></span>|
|[<span data-ttu-id="175a6-115">Get enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="175a6-115">Get enrollmentTroubleshootingEvent</span></span>](../api/intune-troubleshooting-enrollmenttroubleshootingevent-get.md)|[<span data-ttu-id="175a6-116">enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="175a6-116">enrollmentTroubleshootingEvent</span></span>](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md)|<span data-ttu-id="175a6-117">[enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="175a6-117">Read properties and relationships of the [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object.</span></span>|
|[<span data-ttu-id="175a6-118">Create enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="175a6-118">Create enrollmentTroubleshootingEvent</span></span>](../api/intune-troubleshooting-enrollmenttroubleshootingevent-create.md)|[<span data-ttu-id="175a6-119">enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="175a6-119">enrollmentTroubleshootingEvent</span></span>](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md)|<span data-ttu-id="175a6-120">新しい [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="175a6-120">Create a new [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object.</span></span>|
|[<span data-ttu-id="175a6-121">Delete enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="175a6-121">Delete enrollmentTroubleshootingEvent</span></span>](../api/intune-troubleshooting-enrollmenttroubleshootingevent-delete.md)|<span data-ttu-id="175a6-122">なし</span><span class="sxs-lookup"><span data-stu-id="175a6-122">None</span></span>|<span data-ttu-id="175a6-123">[enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="175a6-123">Deletes a [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md).</span></span>|
|[<span data-ttu-id="175a6-124">Update enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="175a6-124">Update enrollmentTroubleshootingEvent</span></span>](../api/intune-troubleshooting-enrollmenttroubleshootingevent-update.md)|[<span data-ttu-id="175a6-125">enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="175a6-125">enrollmentTroubleshootingEvent</span></span>](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md)|<span data-ttu-id="175a6-126">[enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="175a6-126">Update the properties of a [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="175a6-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="175a6-127">Properties</span></span>
|<span data-ttu-id="175a6-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="175a6-128">Property</span></span>|<span data-ttu-id="175a6-129">型</span><span class="sxs-lookup"><span data-stu-id="175a6-129">Type</span></span>|<span data-ttu-id="175a6-130">説明</span><span class="sxs-lookup"><span data-stu-id="175a6-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="175a6-131">id</span><span class="sxs-lookup"><span data-stu-id="175a6-131">id</span></span>|<span data-ttu-id="175a6-132">文字列</span><span class="sxs-lookup"><span data-stu-id="175a6-132">String</span></span>|<span data-ttu-id="175a6-133">オブジェクトの UUID。[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) から継承</span><span class="sxs-lookup"><span data-stu-id="175a6-133">UUID for the object Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="175a6-134">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="175a6-134">eventDateTime</span></span>|<span data-ttu-id="175a6-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="175a6-135">DateTimeOffset</span></span>|<span data-ttu-id="175a6-136">インシデントが発生した時間。</span><span class="sxs-lookup"><span data-stu-id="175a6-136">Time when the event occurred .</span></span> <span data-ttu-id="175a6-137">[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="175a6-137">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="175a6-138">correlationId</span><span class="sxs-lookup"><span data-stu-id="175a6-138">correlationId</span></span>|<span data-ttu-id="175a6-139">String</span><span class="sxs-lookup"><span data-stu-id="175a6-139">String</span></span>|<span data-ttu-id="175a6-140">サービスのエラーをトレースするための ID。</span><span class="sxs-lookup"><span data-stu-id="175a6-140">Id used for tracing the failure in the service.</span></span> <span data-ttu-id="175a6-141">[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="175a6-141">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="175a6-142">トラブルシューティングのエラーの詳細</span><span class="sxs-lookup"><span data-stu-id="175a6-142">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="175a6-143">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="175a6-143">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="175a6-144">エラーとその修復に関する詳細情報を含むオブジェクト。</span><span class="sxs-lookup"><span data-stu-id="175a6-144">Object containing detailed information about the error and its remediation.</span></span> <span data-ttu-id="175a6-145">[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="175a6-145">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="175a6-146">eventName</span><span class="sxs-lookup"><span data-stu-id="175a6-146">eventName</span></span>|<span data-ttu-id="175a6-147">String</span><span class="sxs-lookup"><span data-stu-id="175a6-147">String</span></span>|<span data-ttu-id="175a6-148">トラブルシューティングイベントに対応するイベント名。</span><span class="sxs-lookup"><span data-stu-id="175a6-148">Event Name corresponding to the Troubleshooting Event.</span></span> <span data-ttu-id="175a6-149">[Devicemanagementトラブルシューティングイベント](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)から継承されるオプションフィールドです</span><span class="sxs-lookup"><span data-stu-id="175a6-149">It is an Optional field Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="175a6-150">additionalInformation</span><span class="sxs-lookup"><span data-stu-id="175a6-150">additionalInformation</span></span>|<span data-ttu-id="175a6-151">[keyValuePair](../resources/intune-shared-keyvaluepair.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="175a6-151">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="175a6-152">[Devicemanagementトラブルシューティングイベント](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)から継承されたトラブルシューティングイベントに関する追加情報を提供する文字列キーと文字列値のペアのセット。</span><span class="sxs-lookup"><span data-stu-id="175a6-152">A set of string key and string value pairs which provides additional information on the Troubleshooting event Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="175a6-153">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="175a6-153">managedDeviceIdentifier</span></span>|<span data-ttu-id="175a6-154">String</span><span class="sxs-lookup"><span data-stu-id="175a6-154">String</span></span>|<span data-ttu-id="175a6-155">Intune によって作成または収集されるデバイス識別子。</span><span class="sxs-lookup"><span data-stu-id="175a6-155">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="175a6-156">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="175a6-156">operatingSystem</span></span>|<span data-ttu-id="175a6-157">文字列</span><span class="sxs-lookup"><span data-stu-id="175a6-157">String</span></span>|<span data-ttu-id="175a6-158">オペレーティング システム。</span><span class="sxs-lookup"><span data-stu-id="175a6-158">Operating System.</span></span>|
|<span data-ttu-id="175a6-159">osVersion</span><span class="sxs-lookup"><span data-stu-id="175a6-159">osVersion</span></span>|<span data-ttu-id="175a6-160">String</span><span class="sxs-lookup"><span data-stu-id="175a6-160">String</span></span>|<span data-ttu-id="175a6-161">OS バージョン。</span><span class="sxs-lookup"><span data-stu-id="175a6-161">OS Version.</span></span>|
|<span data-ttu-id="175a6-162">userId</span><span class="sxs-lookup"><span data-stu-id="175a6-162">userId</span></span>|<span data-ttu-id="175a6-163">String</span><span class="sxs-lookup"><span data-stu-id="175a6-163">String</span></span>|<span data-ttu-id="175a6-164">デバイスを登録しようとするユーザーの識別子。</span><span class="sxs-lookup"><span data-stu-id="175a6-164">Identifier for the user that tried to enroll the device.</span></span>|
|<span data-ttu-id="175a6-165">deviceId</span><span class="sxs-lookup"><span data-stu-id="175a6-165">deviceId</span></span>|<span data-ttu-id="175a6-166">String</span><span class="sxs-lookup"><span data-stu-id="175a6-166">String</span></span>|<span data-ttu-id="175a6-167">Azure AD デバイス識別子。</span><span class="sxs-lookup"><span data-stu-id="175a6-167">Azure AD device identifier.</span></span>|
|<span data-ttu-id="175a6-168">enrollmentType</span><span class="sxs-lookup"><span data-stu-id="175a6-168">enrollmentType</span></span>|[<span data-ttu-id="175a6-169">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="175a6-169">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="175a6-170">登録の種類。</span><span class="sxs-lookup"><span data-stu-id="175a6-170">Type of the enrollment.</span></span> <span data-ttu-id="175a6-171">可能な値は、`unknown`、`userEnrollment`、`deviceEnrollmentManager`、`appleBulkWithUser`、`appleBulkWithoutUser`、`windowsAzureADJoin`、`windowsBulkUserless`、`windowsAutoEnrollment`、`windowsBulkAzureDomainJoin`、`windowsCoManagement` です。</span><span class="sxs-lookup"><span data-stu-id="175a6-171">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span></span>|
|<span data-ttu-id="175a6-172">failureCategory</span><span class="sxs-lookup"><span data-stu-id="175a6-172">failureCategory</span></span>|[<span data-ttu-id="175a6-173">deviceEnrollmentFailureReason</span><span class="sxs-lookup"><span data-stu-id="175a6-173">deviceEnrollmentFailureReason</span></span>](../resources/intune-troubleshooting-deviceenrollmentfailurereason.md)|<span data-ttu-id="175a6-174">高レベルのエラー カテゴリ。</span><span class="sxs-lookup"><span data-stu-id="175a6-174">Highlevel failure category.</span></span> <span data-ttu-id="175a6-175">可能な値は、`unknown`、`authentication`、`authorization`、`accountValidation`、`userValidation`、`deviceNotSupported`、`inMaintenance`、`badRequest`、`featureNotSupported`、`enrollmentRestrictionsEnforced`、`clientDisconnected`、`userAbandonment` です。</span><span class="sxs-lookup"><span data-stu-id="175a6-175">Possible values are: `unknown`, `authentication`, `authorization`, `accountValidation`, `userValidation`, `deviceNotSupported`, `inMaintenance`, `badRequest`, `featureNotSupported`, `enrollmentRestrictionsEnforced`, `clientDisconnected`, `userAbandonment`.</span></span>|
|<span data-ttu-id="175a6-176">failureReason</span><span class="sxs-lookup"><span data-stu-id="175a6-176">failureReason</span></span>|<span data-ttu-id="175a6-177">String</span><span class="sxs-lookup"><span data-stu-id="175a6-177">String</span></span>|<span data-ttu-id="175a6-178">詳細なエラーの理由:</span><span class="sxs-lookup"><span data-stu-id="175a6-178">Detailed failure reason.</span></span>|

## <a name="relationships"></a><span data-ttu-id="175a6-179">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="175a6-179">Relationships</span></span>
<span data-ttu-id="175a6-180">なし</span><span class="sxs-lookup"><span data-stu-id="175a6-180">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="175a6-181">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="175a6-181">JSON Representation</span></span>
<span data-ttu-id="175a6-182">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="175a6-182">Here is a JSON representation of the resource.</span></span>
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
  "troubleshootingErrorDetails": {
    "@odata.type": "microsoft.graph.deviceManagementTroubleshootingErrorDetails",
    "context": "String",
    "failure": "String",
    "failureDetails": "String",
    "remediation": "String",
    "resources": [
      {
        "@odata.type": "microsoft.graph.deviceManagementTroubleshootingErrorResource",
        "text": "String",
        "link": "String"
      }
    ]
  },
  "eventName": "String",
  "additionalInformation": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "String",
      "value": "String"
    }
  ],
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





