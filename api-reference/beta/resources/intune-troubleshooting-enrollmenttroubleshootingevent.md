---
title: enrollmentTroubleshootingEvent リソースの種類
description: 登録エラーを表すイベント。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5ee9f09b38ea39e126a6b6925689fc129fbea728
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31803662"
---
# <a name="enrollmenttroubleshootingevent-resource-type"></a><span data-ttu-id="c69e4-103">enrollmentTroubleshootingEvent リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c69e4-103">enrollmentTroubleshootingEvent resource type</span></span>

> <span data-ttu-id="c69e4-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c69e4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c69e4-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="c69e4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c69e4-106">登録エラーを表すイベント。</span><span class="sxs-lookup"><span data-stu-id="c69e4-106">Event representing an enrollment failure.</span></span>


<span data-ttu-id="c69e4-107">[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="c69e4-107">Inherits from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>

## <a name="methods"></a><span data-ttu-id="c69e4-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="c69e4-108">Methods</span></span>
|<span data-ttu-id="c69e4-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="c69e4-109">Method</span></span>|<span data-ttu-id="c69e4-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="c69e4-110">Return Type</span></span>|<span data-ttu-id="c69e4-111">説明</span><span class="sxs-lookup"><span data-stu-id="c69e4-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c69e4-112">enrollmentTroubleshootingEvent のリスト</span><span class="sxs-lookup"><span data-stu-id="c69e4-112">List enrollmentTroubleshootingEvents</span></span>](../api/intune-troubleshooting-enrollmenttroubleshootingevent-list.md)|<span data-ttu-id="c69e4-113">[enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="c69e4-113">[enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) collection</span></span>|<span data-ttu-id="c69e4-114">[enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="c69e4-114">List properties and relationships of the [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) objects.</span></span>|
|[<span data-ttu-id="c69e4-115">enrollmentTroubleshootingEvent の取得</span><span class="sxs-lookup"><span data-stu-id="c69e4-115">Get enrollmentTroubleshootingEvent</span></span>](../api/intune-troubleshooting-enrollmenttroubleshootingevent-get.md)|[<span data-ttu-id="c69e4-116">enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="c69e4-116">enrollmentTroubleshootingEvent</span></span>](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md)|<span data-ttu-id="c69e4-117">[enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="c69e4-117">Read properties and relationships of the [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object.</span></span>|
|[<span data-ttu-id="c69e4-118">enrollmentTroubleshootingEvent の作成</span><span class="sxs-lookup"><span data-stu-id="c69e4-118">Create enrollmentTroubleshootingEvent</span></span>](../api/intune-troubleshooting-enrollmenttroubleshootingevent-create.md)|[<span data-ttu-id="c69e4-119">enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="c69e4-119">enrollmentTroubleshootingEvent</span></span>](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md)|<span data-ttu-id="c69e4-120">新しい [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="c69e4-120">Create a new [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object.</span></span>|
|[<span data-ttu-id="c69e4-121">enrollmentTroubleshootingEvent の削除</span><span class="sxs-lookup"><span data-stu-id="c69e4-121">Delete enrollmentTroubleshootingEvent</span></span>](../api/intune-troubleshooting-enrollmenttroubleshootingevent-delete.md)|<span data-ttu-id="c69e4-122">なし</span><span class="sxs-lookup"><span data-stu-id="c69e4-122">None</span></span>|<span data-ttu-id="c69e4-123">[enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="c69e4-123">Deletes a [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md).</span></span>|
|[<span data-ttu-id="c69e4-124">enrollmentTroubleshootingEvent の更新</span><span class="sxs-lookup"><span data-stu-id="c69e4-124">Update enrollmentTroubleshootingEvent</span></span>](../api/intune-troubleshooting-enrollmenttroubleshootingevent-update.md)|[<span data-ttu-id="c69e4-125">enrollmentTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="c69e4-125">enrollmentTroubleshootingEvent</span></span>](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md)|<span data-ttu-id="c69e4-126">[enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="c69e4-126">Update the properties of a [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="c69e4-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c69e4-127">Properties</span></span>
|<span data-ttu-id="c69e4-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c69e4-128">Property</span></span>|<span data-ttu-id="c69e4-129">型</span><span class="sxs-lookup"><span data-stu-id="c69e4-129">Type</span></span>|<span data-ttu-id="c69e4-130">説明</span><span class="sxs-lookup"><span data-stu-id="c69e4-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c69e4-131">id</span><span class="sxs-lookup"><span data-stu-id="c69e4-131">id</span></span>|<span data-ttu-id="c69e4-132">String</span><span class="sxs-lookup"><span data-stu-id="c69e4-132">String</span></span>|<span data-ttu-id="c69e4-133">オブジェクトの UUID。[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) から継承</span><span class="sxs-lookup"><span data-stu-id="c69e4-133">UUID for the object Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="c69e4-134">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="c69e4-134">eventDateTime</span></span>|<span data-ttu-id="c69e4-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c69e4-135">DateTimeOffset</span></span>|<span data-ttu-id="c69e4-136">インシデントが発生した時間。</span><span class="sxs-lookup"><span data-stu-id="c69e4-136">Time when the event occurred .</span></span> <span data-ttu-id="c69e4-137">[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c69e4-137">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="c69e4-138">correlationId</span><span class="sxs-lookup"><span data-stu-id="c69e4-138">correlationId</span></span>|<span data-ttu-id="c69e4-139">文字列</span><span class="sxs-lookup"><span data-stu-id="c69e4-139">String</span></span>|<span data-ttu-id="c69e4-140">サービスのエラーをトレースするための ID。</span><span class="sxs-lookup"><span data-stu-id="c69e4-140">Id used for tracing the failure in the service.</span></span> <span data-ttu-id="c69e4-141">[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c69e4-141">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="c69e4-142">トラブルシューティングのエラーの詳細</span><span class="sxs-lookup"><span data-stu-id="c69e4-142">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="c69e4-143">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="c69e4-143">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="c69e4-144">エラーとその修復に関する詳細情報を含むオブジェクト。</span><span class="sxs-lookup"><span data-stu-id="c69e4-144">Object containing detailed information about the error and its remediation.</span></span> <span data-ttu-id="c69e4-145">[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c69e4-145">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="c69e4-146">eventName</span><span class="sxs-lookup"><span data-stu-id="c69e4-146">eventName</span></span>|<span data-ttu-id="c69e4-147">文字列</span><span class="sxs-lookup"><span data-stu-id="c69e4-147">String</span></span>|<span data-ttu-id="c69e4-148">トラブルシューティングイベントに対応するイベント名。</span><span class="sxs-lookup"><span data-stu-id="c69e4-148">Event Name corresponding to the Troubleshooting Event.</span></span> <span data-ttu-id="c69e4-149">[devicemanagementトラブルシューティングイベント](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)から継承されるオプションフィールドです</span><span class="sxs-lookup"><span data-stu-id="c69e4-149">It is an Optional field Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="c69e4-150">additionalinformation</span><span class="sxs-lookup"><span data-stu-id="c69e4-150">additionalInformation</span></span>|<span data-ttu-id="c69e4-151">[keyValuePair](../resources/intune-shared-keyvaluepair.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="c69e4-151">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="c69e4-152">[devicemanagementトラブルシューティングイベント](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)から継承されたトラブルシューティングイベントに関する追加情報を提供する文字列キーと文字列値のペアのセット。</span><span class="sxs-lookup"><span data-stu-id="c69e4-152">A set of string key and string value pairs which provides additional information on the Troubleshooting event Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="c69e4-153">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="c69e4-153">managedDeviceIdentifier</span></span>|<span data-ttu-id="c69e4-154">文字列</span><span class="sxs-lookup"><span data-stu-id="c69e4-154">String</span></span>|<span data-ttu-id="c69e4-155">Intune によって作成または収集されるデバイス識別子。</span><span class="sxs-lookup"><span data-stu-id="c69e4-155">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="c69e4-156">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="c69e4-156">operatingSystem</span></span>|<span data-ttu-id="c69e4-157">文字列</span><span class="sxs-lookup"><span data-stu-id="c69e4-157">String</span></span>|<span data-ttu-id="c69e4-158">オペレーティング システム。</span><span class="sxs-lookup"><span data-stu-id="c69e4-158">Operating System.</span></span>|
|<span data-ttu-id="c69e4-159">osVersion</span><span class="sxs-lookup"><span data-stu-id="c69e4-159">osVersion</span></span>|<span data-ttu-id="c69e4-160">文字列</span><span class="sxs-lookup"><span data-stu-id="c69e4-160">String</span></span>|<span data-ttu-id="c69e4-161">OS バージョン。</span><span class="sxs-lookup"><span data-stu-id="c69e4-161">OS Version.</span></span>|
|<span data-ttu-id="c69e4-162">userId</span><span class="sxs-lookup"><span data-stu-id="c69e4-162">userId</span></span>|<span data-ttu-id="c69e4-163">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="c69e4-163">String</span></span>|<span data-ttu-id="c69e4-164">デバイスを登録しようとするユーザーの識別子。</span><span class="sxs-lookup"><span data-stu-id="c69e4-164">Identifier for the user that tried to enroll the device.</span></span>|
|<span data-ttu-id="c69e4-165">deviceId</span><span class="sxs-lookup"><span data-stu-id="c69e4-165">deviceId</span></span>|<span data-ttu-id="c69e4-166">文字列</span><span class="sxs-lookup"><span data-stu-id="c69e4-166">String</span></span>|<span data-ttu-id="c69e4-167">Azure AD デバイス識別子。</span><span class="sxs-lookup"><span data-stu-id="c69e4-167">Azure AD device identifier.</span></span>|
|<span data-ttu-id="c69e4-168">enrollmentType</span><span class="sxs-lookup"><span data-stu-id="c69e4-168">enrollmentType</span></span>|[<span data-ttu-id="c69e4-169">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="c69e4-169">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="c69e4-170">登録の種類。</span><span class="sxs-lookup"><span data-stu-id="c69e4-170">Type of the enrollment.</span></span> <span data-ttu-id="c69e4-171">可能な値は、`unknown`、`userEnrollment`、`deviceEnrollmentManager`、`appleBulkWithUser`、`appleBulkWithoutUser`、`windowsAzureADJoin`、`windowsBulkUserless`、`windowsAutoEnrollment`、`windowsBulkAzureDomainJoin`、`windowsCoManagement` です。</span><span class="sxs-lookup"><span data-stu-id="c69e4-171">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span></span>|
|<span data-ttu-id="c69e4-172">failureCategory</span><span class="sxs-lookup"><span data-stu-id="c69e4-172">failureCategory</span></span>|[<span data-ttu-id="c69e4-173">deviceEnrollmentFailureReason</span><span class="sxs-lookup"><span data-stu-id="c69e4-173">deviceEnrollmentFailureReason</span></span>](../resources/intune-troubleshooting-deviceenrollmentfailurereason.md)|<span data-ttu-id="c69e4-174">高レベルのエラー カテゴリ。</span><span class="sxs-lookup"><span data-stu-id="c69e4-174">Highlevel failure category.</span></span> <span data-ttu-id="c69e4-175">可能な値は、`unknown`、`authentication`、`authorization`、`accountValidation`、`userValidation`、`deviceNotSupported`、`inMaintenance`、`badRequest`、`featureNotSupported`、`enrollmentRestrictionsEnforced`、`clientDisconnected`、`userAbandonment` です。</span><span class="sxs-lookup"><span data-stu-id="c69e4-175">Possible values are: `unknown`, `authentication`, `authorization`, `accountValidation`, `userValidation`, `deviceNotSupported`, `inMaintenance`, `badRequest`, `featureNotSupported`, `enrollmentRestrictionsEnforced`, `clientDisconnected`, `userAbandonment`.</span></span>|
|<span data-ttu-id="c69e4-176">failureReason</span><span class="sxs-lookup"><span data-stu-id="c69e4-176">failureReason</span></span>|<span data-ttu-id="c69e4-177">String</span><span class="sxs-lookup"><span data-stu-id="c69e4-177">String</span></span>|<span data-ttu-id="c69e4-178">詳細なエラーの理由:</span><span class="sxs-lookup"><span data-stu-id="c69e4-178">Detailed failure reason.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c69e4-179">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="c69e4-179">Relationships</span></span>
<span data-ttu-id="c69e4-180">なし</span><span class="sxs-lookup"><span data-stu-id="c69e4-180">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c69e4-181">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c69e4-181">JSON Representation</span></span>
<span data-ttu-id="c69e4-182">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="c69e4-182">Here is a JSON representation of the resource.</span></span>
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



