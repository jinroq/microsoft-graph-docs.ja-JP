---
title: MobileAppTroubleshootingEvent の更新
description: 複数のワークフローをサポートする Microsoft Graph API for Intune の Update mobileAppTroubleshootingEvent メソッドについて説明します。
localization_priority: Normal
author: rolyon
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2ed403d19ee0a686812fb0bdf1f4b6d7239638e7
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36350833"
---
# <a name="update-mobileapptroubleshootingevent"></a><span data-ttu-id="a2bee-103">MobileAppTroubleshootingEvent の更新</span><span class="sxs-lookup"><span data-stu-id="a2bee-103">Update mobileAppTroubleshootingEvent</span></span>

> <span data-ttu-id="a2bee-104">**重要:** Microsoft Graph の/ベータ版の Api は変更される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="a2bee-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="a2bee-105">実稼働アプリケーションでは、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a2bee-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a2bee-106">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="a2bee-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a2bee-107">[MobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="a2bee-107">Update the properties of a [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a2bee-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="a2bee-108">Prerequisites</span></span>
<span data-ttu-id="a2bee-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a2bee-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a2bee-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a2bee-111">Permission type</span></span>|<span data-ttu-id="a2bee-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="a2bee-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a2bee-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a2bee-113">Delegated (work or school account)</span></span>||
|<span data-ttu-id="a2bee-114">&nbsp;&nbsp; **デバイスの管理**</span><span class="sxs-lookup"><span data-stu-id="a2bee-114">&nbsp; &nbsp; **Device management**</span></span>|<span data-ttu-id="a2bee-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a2bee-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="a2bee-116">&nbsp; &nbsp; **トラブルシューティング**</span><span class="sxs-lookup"><span data-stu-id="a2bee-116">&nbsp; &nbsp; **Troubleshooting**</span></span>|<span data-ttu-id="a2bee-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a2bee-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="a2bee-118">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a2bee-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a2bee-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a2bee-119">Not supported.</span></span>|
|<span data-ttu-id="a2bee-120">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a2bee-120">Application</span></span>|<span data-ttu-id="a2bee-121">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a2bee-121">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a2bee-122">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a2bee-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}
PATCH /users/{usersId}/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}
```

## <a name="request-headers"></a><span data-ttu-id="a2bee-123">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a2bee-123">Request headers</span></span>
|<span data-ttu-id="a2bee-124">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a2bee-124">Header</span></span>|<span data-ttu-id="a2bee-125">値</span><span class="sxs-lookup"><span data-stu-id="a2bee-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a2bee-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="a2bee-126">Authorization</span></span>|<span data-ttu-id="a2bee-127">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="a2bee-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a2bee-128">承諾</span><span class="sxs-lookup"><span data-stu-id="a2bee-128">Accept</span></span>|<span data-ttu-id="a2bee-129">application/json</span><span class="sxs-lookup"><span data-stu-id="a2bee-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a2bee-130">要求本文</span><span class="sxs-lookup"><span data-stu-id="a2bee-130">Request body</span></span>
<span data-ttu-id="a2bee-131">要求本文で、 [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="a2bee-131">In the request body, supply a JSON representation for the [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) object.</span></span>

<span data-ttu-id="a2bee-132">次の表に、 [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="a2bee-132">The following table shows the properties that are required when you create the [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md).</span></span>

|<span data-ttu-id="a2bee-133">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a2bee-133">Property</span></span>|<span data-ttu-id="a2bee-134">型</span><span class="sxs-lookup"><span data-stu-id="a2bee-134">Type</span></span>|<span data-ttu-id="a2bee-135">説明</span><span class="sxs-lookup"><span data-stu-id="a2bee-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a2bee-136">id</span><span class="sxs-lookup"><span data-stu-id="a2bee-136">id</span></span>|<span data-ttu-id="a2bee-137">文字列</span><span class="sxs-lookup"><span data-stu-id="a2bee-137">String</span></span>|<span data-ttu-id="a2bee-138">オブジェクトの GUID</span><span class="sxs-lookup"><span data-stu-id="a2bee-138">The GUID for the object</span></span>|
|<span data-ttu-id="a2bee-139">**トラブルシューティング**</span><span class="sxs-lookup"><span data-stu-id="a2bee-139">**Troubleshooting**</span></span>|
|<span data-ttu-id="a2bee-140">additionalInformation</span><span class="sxs-lookup"><span data-stu-id="a2bee-140">additionalInformation</span></span>|<span data-ttu-id="a2bee-141">[keyValuePair](../resources/intune-shared-keyvaluepair.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="a2bee-141">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="a2bee-142">トラブルシューティングイベントに関する追加情報を提供する文字列キーと文字列値のペアのセット。</span><span class="sxs-lookup"><span data-stu-id="a2bee-142">A set of string key and string value pairs which provides additional information on the Troubleshooting event.</span></span>|
|<span data-ttu-id="a2bee-143">applicationId</span><span class="sxs-lookup"><span data-stu-id="a2bee-143">applicationId</span></span>|<span data-ttu-id="a2bee-144">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="a2bee-144">String</span></span>|<span data-ttu-id="a2bee-145">Intune アプリケーション識別子。</span><span class="sxs-lookup"><span data-stu-id="a2bee-145">Intune application identifier.</span></span>|
|<span data-ttu-id="a2bee-146">correlationId</span><span class="sxs-lookup"><span data-stu-id="a2bee-146">correlationId</span></span>|<span data-ttu-id="a2bee-147">String</span><span class="sxs-lookup"><span data-stu-id="a2bee-147">String</span></span>|<span data-ttu-id="a2bee-148">サービスのエラーをトレースするために使用される ID。</span><span class="sxs-lookup"><span data-stu-id="a2bee-148">ID used for tracing the failure in the service.</span></span> |
|<span data-ttu-id="a2bee-149">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="a2bee-149">eventDateTime</span></span>|<span data-ttu-id="a2bee-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a2bee-150">DateTimeOffset</span></span>|<span data-ttu-id="a2bee-151">イベントが発生した時刻。</span><span class="sxs-lookup"><span data-stu-id="a2bee-151">Time when the event occurred.</span></span> |
|<span data-ttu-id="a2bee-152">eventName</span><span class="sxs-lookup"><span data-stu-id="a2bee-152">eventName</span></span>|<span data-ttu-id="a2bee-153">String</span><span class="sxs-lookup"><span data-stu-id="a2bee-153">String</span></span>|<span data-ttu-id="a2bee-154">トラブルシューティングイベントに対応するイベント名。</span><span class="sxs-lookup"><span data-stu-id="a2bee-154">Event Name corresponding to the Troubleshooting Event.</span></span> <span data-ttu-id="a2bee-155">省略可能。</span><span class="sxs-lookup"><span data-stu-id="a2bee-155">Optional.</span></span>|
|<span data-ttu-id="a2bee-156">履歴</span><span class="sxs-lookup"><span data-stu-id="a2bee-156">history</span></span>|<span data-ttu-id="a2bee-157">[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="a2bee-157">[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md) collection</span></span>|<span data-ttu-id="a2bee-158">Intune モバイルアプリケーションのトラブルシューティングの履歴項目。</span><span class="sxs-lookup"><span data-stu-id="a2bee-158">Intune Mobile Application Troubleshooting History Item.</span></span>|
|<span data-ttu-id="a2bee-159">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="a2bee-159">managedDeviceIdentifier</span></span>|<span data-ttu-id="a2bee-160">String</span><span class="sxs-lookup"><span data-stu-id="a2bee-160">String</span></span>|<span data-ttu-id="a2bee-161">Intune によって作成または収集されるデバイス識別子。</span><span class="sxs-lookup"><span data-stu-id="a2bee-161">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="a2bee-162">トラブルシューティングのエラーの詳細</span><span class="sxs-lookup"><span data-stu-id="a2bee-162">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="a2bee-163">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="a2bee-163">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="a2bee-164">エラーとその修復に関する詳細情報を含むオブジェクト。</span><span class="sxs-lookup"><span data-stu-id="a2bee-164">Object containing detailed information about the error and its remediation.</span></span> |
|<span data-ttu-id="a2bee-165">userId</span><span class="sxs-lookup"><span data-stu-id="a2bee-165">userId</span></span>|<span data-ttu-id="a2bee-166">String</span><span class="sxs-lookup"><span data-stu-id="a2bee-166">String</span></span>|<span data-ttu-id="a2bee-167">デバイスを登録しようとするユーザーの識別子。</span><span class="sxs-lookup"><span data-stu-id="a2bee-167">Identifier for the user that tried to enroll the device.</span></span>|

## <a name="response"></a><span data-ttu-id="a2bee-168">応答</span><span class="sxs-lookup"><span data-stu-id="a2bee-168">Response</span></span>
<span data-ttu-id="a2bee-169">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="a2bee-169">If successful, this method returns a `200 OK` response code and an updated [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a2bee-170">例</span><span class="sxs-lookup"><span data-stu-id="a2bee-170">Example</span></span>

### <a name="request"></a><span data-ttu-id="a2bee-171">要求</span><span class="sxs-lookup"><span data-stu-id="a2bee-171">Request</span></span>
<span data-ttu-id="a2bee-172">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="a2bee-172">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}
Content-type: application/json
Content-length: 71

{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingEvent"
}
```

### <a name="response"></a><span data-ttu-id="a2bee-173">応答</span><span class="sxs-lookup"><span data-stu-id="a2bee-173">Response</span></span>
<span data-ttu-id="a2bee-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="a2bee-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 120

{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingEvent",
  "id": "77943c10-3c10-7794-103c-9477103c9477"
}
```







