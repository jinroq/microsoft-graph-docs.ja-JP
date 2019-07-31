---
title: MobileAppTroubleshootingEvent を作成する
description: 複数のワークフローをサポートする Microsoft Graph API for Intune の Create mobileAppTroubleshootingEvent メソッドについて説明します。
localization_priority: Normal
author: rolyon
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9eae0c2d66dc28fd70d95c66f2ce034b16523d30
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35979751"
---
# <a name="create-mobileapptroubleshootingevent"></a><span data-ttu-id="4d7c3-103">MobileAppTroubleshootingEvent を作成する</span><span class="sxs-lookup"><span data-stu-id="4d7c3-103">Create mobileAppTroubleshootingEvent</span></span>

> <span data-ttu-id="4d7c3-104">**重要:** Microsoft Graph の/ベータ版の Api は変更される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="4d7c3-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="4d7c3-105">実稼働アプリケーションでは、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4d7c3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4d7c3-106">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="4d7c3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4d7c3-107">新しい[mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="4d7c3-107">Create a new [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4d7c3-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="4d7c3-108">Prerequisites</span></span>
<span data-ttu-id="4d7c3-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4d7c3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4d7c3-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4d7c3-111">Permission type</span></span>|<span data-ttu-id="4d7c3-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="4d7c3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4d7c3-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="4d7c3-113">Delegated (work or school account)</span></span>||
|<span data-ttu-id="4d7c3-114">&nbsp;&nbsp; **デバイスの管理**</span><span class="sxs-lookup"><span data-stu-id="4d7c3-114">&nbsp; &nbsp; **Device management**</span></span>|<span data-ttu-id="4d7c3-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4d7c3-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="4d7c3-116">&nbsp; &nbsp; **トラブルシューティング**</span><span class="sxs-lookup"><span data-stu-id="4d7c3-116">&nbsp; &nbsp; **Troubleshooting**</span></span>|<span data-ttu-id="4d7c3-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4d7c3-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="4d7c3-118">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4d7c3-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4d7c3-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4d7c3-119">Not supported.</span></span>|
|<span data-ttu-id="4d7c3-120">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4d7c3-120">Application</span></span>|<span data-ttu-id="4d7c3-121">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4d7c3-121">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4d7c3-122">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4d7c3-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/mobileAppTroubleshootingEvents
POST /users/{usersId}/mobileAppTroubleshootingEvents
```

## <a name="request-headers"></a><span data-ttu-id="4d7c3-123">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4d7c3-123">Request headers</span></span>
|<span data-ttu-id="4d7c3-124">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4d7c3-124">Header</span></span>|<span data-ttu-id="4d7c3-125">値</span><span class="sxs-lookup"><span data-stu-id="4d7c3-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4d7c3-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="4d7c3-126">Authorization</span></span>|<span data-ttu-id="4d7c3-127">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="4d7c3-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4d7c3-128">承諾</span><span class="sxs-lookup"><span data-stu-id="4d7c3-128">Accept</span></span>|<span data-ttu-id="4d7c3-129">application/json</span><span class="sxs-lookup"><span data-stu-id="4d7c3-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4d7c3-130">要求本文</span><span class="sxs-lookup"><span data-stu-id="4d7c3-130">Request body</span></span>
<span data-ttu-id="4d7c3-131">要求本文で、mobileAppTroubleshootingEvent オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="4d7c3-131">In the request body, supply a JSON representation for the mobileAppTroubleshootingEvent object.</span></span>

<span data-ttu-id="4d7c3-132">次の表に、mobileAppTroubleshootingEvent の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="4d7c3-132">The following table shows the properties that are required when you create the mobileAppTroubleshootingEvent.</span></span>

|<span data-ttu-id="4d7c3-133">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4d7c3-133">Property</span></span>|<span data-ttu-id="4d7c3-134">型</span><span class="sxs-lookup"><span data-stu-id="4d7c3-134">Type</span></span>|<span data-ttu-id="4d7c3-135">説明</span><span class="sxs-lookup"><span data-stu-id="4d7c3-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4d7c3-136">id</span><span class="sxs-lookup"><span data-stu-id="4d7c3-136">id</span></span>|<span data-ttu-id="4d7c3-137">文字列</span><span class="sxs-lookup"><span data-stu-id="4d7c3-137">String</span></span>|<span data-ttu-id="4d7c3-138">オブジェクトの GUID</span><span class="sxs-lookup"><span data-stu-id="4d7c3-138">The GUID for the object</span></span>|
|<span data-ttu-id="4d7c3-139">**トラブルシューティング**</span><span class="sxs-lookup"><span data-stu-id="4d7c3-139">**Troubleshooting**</span></span>|
|<span data-ttu-id="4d7c3-140">additionalInformation</span><span class="sxs-lookup"><span data-stu-id="4d7c3-140">additionalInformation</span></span>|<span data-ttu-id="4d7c3-141">[keyValuePair](../resources/intune-shared-keyvaluepair.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="4d7c3-141">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="4d7c3-142">トラブルシューティングイベントに関する追加情報を提供する文字列キーと文字列値のペアのセット。</span><span class="sxs-lookup"><span data-stu-id="4d7c3-142">A set of string key and string value pairs which provides additional information on the Troubleshooting event.</span></span>|
|<span data-ttu-id="4d7c3-143">applicationId</span><span class="sxs-lookup"><span data-stu-id="4d7c3-143">applicationId</span></span>|<span data-ttu-id="4d7c3-144">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="4d7c3-144">String</span></span>|<span data-ttu-id="4d7c3-145">Intune アプリケーション識別子。</span><span class="sxs-lookup"><span data-stu-id="4d7c3-145">Intune application identifier.</span></span>|
|<span data-ttu-id="4d7c3-146">correlationId</span><span class="sxs-lookup"><span data-stu-id="4d7c3-146">correlationId</span></span>|<span data-ttu-id="4d7c3-147">String</span><span class="sxs-lookup"><span data-stu-id="4d7c3-147">String</span></span>|<span data-ttu-id="4d7c3-148">サービスのエラーをトレースするために使用される ID。</span><span class="sxs-lookup"><span data-stu-id="4d7c3-148">ID used for tracing the failure in the service.</span></span> |
|<span data-ttu-id="4d7c3-149">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="4d7c3-149">eventDateTime</span></span>|<span data-ttu-id="4d7c3-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4d7c3-150">DateTimeOffset</span></span>|<span data-ttu-id="4d7c3-151">インシデントが発生した時間。</span><span class="sxs-lookup"><span data-stu-id="4d7c3-151">Time when the event occurred .</span></span> |
|<span data-ttu-id="4d7c3-152">eventName</span><span class="sxs-lookup"><span data-stu-id="4d7c3-152">eventName</span></span>|<span data-ttu-id="4d7c3-153">String</span><span class="sxs-lookup"><span data-stu-id="4d7c3-153">String</span></span>|<span data-ttu-id="4d7c3-154">トラブルシューティングイベントに対応するイベント名。</span><span class="sxs-lookup"><span data-stu-id="4d7c3-154">Event Name corresponding to the Troubleshooting Event.</span></span> <span data-ttu-id="4d7c3-155">省略可能。</span><span class="sxs-lookup"><span data-stu-id="4d7c3-155">Optional.</span></span>|
|<span data-ttu-id="4d7c3-156">履歴</span><span class="sxs-lookup"><span data-stu-id="4d7c3-156">history</span></span>|<span data-ttu-id="4d7c3-157">[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="4d7c3-157">[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md) collection</span></span>|<span data-ttu-id="4d7c3-158">Intune モバイルアプリケーションのトラブルシューティングの履歴項目</span><span class="sxs-lookup"><span data-stu-id="4d7c3-158">Intune Mobile Application Troubleshooting History Item</span></span>|
|<span data-ttu-id="4d7c3-159">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="4d7c3-159">managedDeviceIdentifier</span></span>|<span data-ttu-id="4d7c3-160">String</span><span class="sxs-lookup"><span data-stu-id="4d7c3-160">String</span></span>|<span data-ttu-id="4d7c3-161">Intune によって作成または収集されるデバイス識別子。</span><span class="sxs-lookup"><span data-stu-id="4d7c3-161">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="4d7c3-162">トラブルシューティングのエラーの詳細</span><span class="sxs-lookup"><span data-stu-id="4d7c3-162">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="4d7c3-163">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="4d7c3-163">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="4d7c3-164">エラーとその修復に関する詳細情報を含むオブジェクト。</span><span class="sxs-lookup"><span data-stu-id="4d7c3-164">Object containing detailed information about the error and its remediation.</span></span> |
|<span data-ttu-id="4d7c3-165">userId</span><span class="sxs-lookup"><span data-stu-id="4d7c3-165">userId</span></span>|<span data-ttu-id="4d7c3-166">String</span><span class="sxs-lookup"><span data-stu-id="4d7c3-166">String</span></span>|<span data-ttu-id="4d7c3-167">デバイスを登録しようとするユーザーの識別子。</span><span class="sxs-lookup"><span data-stu-id="4d7c3-167">Identifier for the user that tried to enroll the device.</span></span>|

## <a name="response"></a><span data-ttu-id="4d7c3-168">応答</span><span class="sxs-lookup"><span data-stu-id="4d7c3-168">Response</span></span>
<span data-ttu-id="4d7c3-169">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="4d7c3-169">If successful, this method returns a `201 Created` response code and a [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4d7c3-170">例</span><span class="sxs-lookup"><span data-stu-id="4d7c3-170">Example</span></span>

### <a name="request"></a><span data-ttu-id="4d7c3-171">要求</span><span class="sxs-lookup"><span data-stu-id="4d7c3-171">Request</span></span>
<span data-ttu-id="4d7c3-172">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="4d7c3-172">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/mobileAppTroubleshootingEvents
Content-type: application/json
Content-length: 71

{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingEvent"
}
```

### <a name="response"></a><span data-ttu-id="4d7c3-173">応答</span><span class="sxs-lookup"><span data-stu-id="4d7c3-173">Response</span></span>
<span data-ttu-id="4d7c3-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="4d7c3-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 120

{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingEvent",
  "id": "77943c10-3c10-7794-103c-9477103c9477"
}
```




