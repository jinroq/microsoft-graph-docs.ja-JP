---
title: Create mobileThreatDefenseConnector
description: 新しい mobileThreatDefenseConnector オブジェクトを作成します。
author: tfitzmac
ms.openlocfilehash: e77b4684f2f330441b8d9ec1f7b14e8e788835a9
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27330983"
---
# <a name="create-mobilethreatdefenseconnector"></a><span data-ttu-id="235f2-103">Create mobileThreatDefenseConnector</span><span class="sxs-lookup"><span data-stu-id="235f2-103">Create mobileThreatDefenseConnector</span></span>

> <span data-ttu-id="235f2-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="235f2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="235f2-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="235f2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="235f2-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="235f2-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="235f2-107">新しい [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="235f2-107">Create a new [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="235f2-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="235f2-108">Prerequisites</span></span>
<span data-ttu-id="235f2-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="235f2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="235f2-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="235f2-111">Permission type</span></span>|<span data-ttu-id="235f2-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="235f2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="235f2-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="235f2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="235f2-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="235f2-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="235f2-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="235f2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="235f2-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="235f2-116">Not supported.</span></span>|
|<span data-ttu-id="235f2-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="235f2-117">Application</span></span>|<span data-ttu-id="235f2-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="235f2-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="235f2-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="235f2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/mobileThreatDefenseConnectors
```

## <a name="request-headers"></a><span data-ttu-id="235f2-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="235f2-120">Request headers</span></span>
|<span data-ttu-id="235f2-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="235f2-121">Header</span></span>|<span data-ttu-id="235f2-122">値</span><span class="sxs-lookup"><span data-stu-id="235f2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="235f2-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="235f2-123">Authorization</span></span>|<span data-ttu-id="235f2-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="235f2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="235f2-125">Accept</span><span class="sxs-lookup"><span data-stu-id="235f2-125">Accept</span></span>|<span data-ttu-id="235f2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="235f2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="235f2-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="235f2-127">Request body</span></span>
<span data-ttu-id="235f2-128">要求本文で、mobileThreatDefenseConnector オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="235f2-128">In the request body, supply a JSON representation for the mobileThreatDefenseConnector object.</span></span>

<span data-ttu-id="235f2-129">次の表に、mobileThreatDefenseConnector 作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="235f2-129">The following table shows the properties that are required when you create the mobileThreatDefenseConnector.</span></span>

|<span data-ttu-id="235f2-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="235f2-130">Property</span></span>|<span data-ttu-id="235f2-131">種類</span><span class="sxs-lookup"><span data-stu-id="235f2-131">Type</span></span>|<span data-ttu-id="235f2-132">説明</span><span class="sxs-lookup"><span data-stu-id="235f2-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="235f2-133">ID</span><span class="sxs-lookup"><span data-stu-id="235f2-133">id</span></span>|<span data-ttu-id="235f2-134">String</span><span class="sxs-lookup"><span data-stu-id="235f2-134">String</span></span>|<span data-ttu-id="235f2-135">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="235f2-135">Not yet documented</span></span>|
|<span data-ttu-id="235f2-136">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="235f2-136">lastHeartbeatDateTime</span></span>|<span data-ttu-id="235f2-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="235f2-137">DateTimeOffset</span></span>|<span data-ttu-id="235f2-138">データ同期パートナーから受信した最後のハートビートの日時</span><span class="sxs-lookup"><span data-stu-id="235f2-138">DateTime of last Heartbeat recieved from the Data Sync Partner</span></span>|
|<span data-ttu-id="235f2-139">partnerState</span><span class="sxs-lookup"><span data-stu-id="235f2-139">partnerState</span></span>|[<span data-ttu-id="235f2-140">mobileThreatPartnerTenantState</span><span class="sxs-lookup"><span data-stu-id="235f2-140">mobileThreatPartnerTenantState</span></span>](../resources/intune-onboarding-mobilethreatpartnertenantstate.md)|<span data-ttu-id="235f2-141">このアカウントのデータの同期パートナーの状態です。</span><span class="sxs-lookup"><span data-stu-id="235f2-141">Data Sync Partner state for this account.</span></span> <span data-ttu-id="235f2-142">可能な値は、`unavailable`、`available`、`enabled`、`unresponsive` です。</span><span class="sxs-lookup"><span data-stu-id="235f2-142">Possible values are: `unavailable`, `available`, `enabled`, `unresponsive`.</span></span>|
|<span data-ttu-id="235f2-143">androidEnabled</span><span class="sxs-lookup"><span data-stu-id="235f2-143">androidEnabled</span></span>|<span data-ttu-id="235f2-144">ブール型</span><span class="sxs-lookup"><span data-stu-id="235f2-144">Boolean</span></span>|<span data-ttu-id="235f2-145">Android において、準拠評価時にデータ同期パートナーからのデータを使用するかどうかを設定します</span><span class="sxs-lookup"><span data-stu-id="235f2-145">For Android, set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="235f2-146">iosEnabled</span><span class="sxs-lookup"><span data-stu-id="235f2-146">iosEnabled</span></span>|<span data-ttu-id="235f2-147">ブール型</span><span class="sxs-lookup"><span data-stu-id="235f2-147">Boolean</span></span>|<span data-ttu-id="235f2-148">IOS において、準拠評価時にデータ同期パートナーからのデータを使用するかどうかを取得または設定します</span><span class="sxs-lookup"><span data-stu-id="235f2-148">For IOS, get or set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="235f2-149">windowsEnabled</span><span class="sxs-lookup"><span data-stu-id="235f2-149">windowsEnabled</span></span>|<span data-ttu-id="235f2-150">ブール型</span><span class="sxs-lookup"><span data-stu-id="235f2-150">Boolean</span></span>|<span data-ttu-id="235f2-151">ウィンドウを取得または設定するコンプライアンスの評価中にデータの同期パートナーからのデータを使用する必要があるかどうか</span><span class="sxs-lookup"><span data-stu-id="235f2-151">For Windows, get or set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="235f2-152">macEnabled</span><span class="sxs-lookup"><span data-stu-id="235f2-152">macEnabled</span></span>|<span data-ttu-id="235f2-153">ブール型</span><span class="sxs-lookup"><span data-stu-id="235f2-153">Boolean</span></span>|<span data-ttu-id="235f2-154">For Mac を取得または設定するコンプライアンスの評価中にデータの同期パートナーからのデータを使用する必要があるかどうか</span><span class="sxs-lookup"><span data-stu-id="235f2-154">For Mac, get or set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="235f2-155">androidDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="235f2-155">androidDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="235f2-156">ブール型</span><span class="sxs-lookup"><span data-stu-id="235f2-156">Boolean</span></span>|<span data-ttu-id="235f2-157">Android において、デバイスを準拠させる前に Intune がデータ同期パートナーからデータを受信する必要があるかどうかを設定します</span><span class="sxs-lookup"><span data-stu-id="235f2-157">For Android, set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="235f2-158">iosDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="235f2-158">iosDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="235f2-159">ブール型</span><span class="sxs-lookup"><span data-stu-id="235f2-159">Boolean</span></span>|<span data-ttu-id="235f2-160">IOS において、デバイスを準拠させる前に Intune がデータ同期パートナーからデータを受信する必要があるかどうかを設定します</span><span class="sxs-lookup"><span data-stu-id="235f2-160">For IOS, set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="235f2-161">windowsDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="235f2-161">windowsDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="235f2-162">ブール型</span><span class="sxs-lookup"><span data-stu-id="235f2-162">Boolean</span></span>|<span data-ttu-id="235f2-163">Windows Intune は、準拠デバイスをマークする前にデータの同期パートナーからデータを受信する必要があるかどうかを設定します。</span><span class="sxs-lookup"><span data-stu-id="235f2-163">For Windows, set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="235f2-164">macDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="235f2-164">macDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="235f2-165">ブール型</span><span class="sxs-lookup"><span data-stu-id="235f2-165">Boolean</span></span>|<span data-ttu-id="235f2-166">For Mac を取得または設定する Intune 準拠デバイスをマークする前にデータの同期パートナーからデータを受信する必要があるかどうか</span><span class="sxs-lookup"><span data-stu-id="235f2-166">For Mac, get or set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="235f2-167">partnerUnsupportedOsVersionBlocked</span><span class="sxs-lookup"><span data-stu-id="235f2-167">partnerUnsupportedOsVersionBlocked</span></span>|<span data-ttu-id="235f2-168">ブール型</span><span class="sxs-lookup"><span data-stu-id="235f2-168">Boolean</span></span>|<span data-ttu-id="235f2-169">データ同期パートナーの最小バージョンの要件を満たさない、有効なプラットフォーム上のデバイスをブロックするかどうかを取得または設定します</span><span class="sxs-lookup"><span data-stu-id="235f2-169">Get or set whether to block devices on the enabled platforms that do not meet the minimum version requirements of the Data Sync Partner</span></span>|
|<span data-ttu-id="235f2-170">partnerUnresponsivenessThresholdInDays</span><span class="sxs-lookup"><span data-stu-id="235f2-170">partnerUnresponsivenessThresholdInDays</span></span>|<span data-ttu-id="235f2-171">Int32</span><span class="sxs-lookup"><span data-stu-id="235f2-171">Int32</span></span>|<span data-ttu-id="235f2-172">このパートナー統合に関する、テナントごとの無応答への許容日数の取得または設定を行います</span><span class="sxs-lookup"><span data-stu-id="235f2-172">Get or Set days the per tenant tolerance to unresponsiveness for this partner integration</span></span>|
|<span data-ttu-id="235f2-173">allowPartnerToCollectIOSApplicationMetadata</span><span class="sxs-lookup"><span data-stu-id="235f2-173">allowPartnerToCollectIOSApplicationMetadata</span></span>|<span data-ttu-id="235f2-174">ブール型</span><span class="sxs-lookup"><span data-stu-id="235f2-174">Boolean</span></span>|<span data-ttu-id="235f2-175">IOS デバイスでは、データの同期パートナー Intune からインストールされているアプリケーションについてのメタデータの収集もあるかどうかを構成するのには管理者では、します。</span><span class="sxs-lookup"><span data-stu-id="235f2-175">For IOS devices, allows the admin to configure whether the data sync partner may also collect metadata about installed applications from Intune</span></span>|



## <a name="response"></a><span data-ttu-id="235f2-176">応答</span><span class="sxs-lookup"><span data-stu-id="235f2-176">Response</span></span>
<span data-ttu-id="235f2-177">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="235f2-177">If successful, this method returns a `201 Created` response code and a [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="235f2-178">例</span><span class="sxs-lookup"><span data-stu-id="235f2-178">Example</span></span>
### <a name="request"></a><span data-ttu-id="235f2-179">要求</span><span class="sxs-lookup"><span data-stu-id="235f2-179">Request</span></span>
<span data-ttu-id="235f2-180">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="235f2-180">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/mobileThreatDefenseConnectors
Content-type: application/json
Content-length: 622

{
  "@odata.type": "#microsoft.graph.mobileThreatDefenseConnector",
  "lastHeartbeatDateTime": "2016-12-31T23:59:37.9174975-08:00",
  "partnerState": "available",
  "androidEnabled": true,
  "iosEnabled": true,
  "windowsEnabled": true,
  "macEnabled": true,
  "androidDeviceBlockedOnMissingPartnerData": true,
  "iosDeviceBlockedOnMissingPartnerData": true,
  "windowsDeviceBlockedOnMissingPartnerData": true,
  "macDeviceBlockedOnMissingPartnerData": true,
  "partnerUnsupportedOsVersionBlocked": true,
  "partnerUnresponsivenessThresholdInDays": 6,
  "allowPartnerToCollectIOSApplicationMetadata": true
}
```

### <a name="response"></a><span data-ttu-id="235f2-181">応答</span><span class="sxs-lookup"><span data-stu-id="235f2-181">Response</span></span>
<span data-ttu-id="235f2-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="235f2-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 671

{
  "@odata.type": "#microsoft.graph.mobileThreatDefenseConnector",
  "id": "e4bede14-de14-e4be-14de-bee414debee4",
  "lastHeartbeatDateTime": "2016-12-31T23:59:37.9174975-08:00",
  "partnerState": "available",
  "androidEnabled": true,
  "iosEnabled": true,
  "windowsEnabled": true,
  "macEnabled": true,
  "androidDeviceBlockedOnMissingPartnerData": true,
  "iosDeviceBlockedOnMissingPartnerData": true,
  "windowsDeviceBlockedOnMissingPartnerData": true,
  "macDeviceBlockedOnMissingPartnerData": true,
  "partnerUnsupportedOsVersionBlocked": true,
  "partnerUnresponsivenessThresholdInDays": 6,
  "allowPartnerToCollectIOSApplicationMetadata": true
}
```




