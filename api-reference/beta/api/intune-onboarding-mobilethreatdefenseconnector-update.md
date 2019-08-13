---
title: mobileThreatDefenseConnector の更新
description: mobileThreatDefenseConnector オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 94a3ed1a531c0d37faa771d54ff9268f5a9be97b
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36352540"
---
# <a name="update-mobilethreatdefenseconnector"></a><span data-ttu-id="e73b1-103">mobileThreatDefenseConnector の更新</span><span class="sxs-lookup"><span data-stu-id="e73b1-103">Update mobileThreatDefenseConnector</span></span>

> <span data-ttu-id="e73b1-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e73b1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e73b1-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="e73b1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e73b1-106">[mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="e73b1-106">Update the properties of a [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e73b1-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="e73b1-107">Prerequisites</span></span>
<span data-ttu-id="e73b1-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e73b1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e73b1-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e73b1-110">Permission type</span></span>|<span data-ttu-id="e73b1-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="e73b1-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e73b1-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e73b1-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e73b1-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e73b1-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="e73b1-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e73b1-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e73b1-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e73b1-115">Not supported.</span></span>|
|<span data-ttu-id="e73b1-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e73b1-116">Application</span></span>|<span data-ttu-id="e73b1-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e73b1-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e73b1-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e73b1-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/mobileThreatDefenseConnectors/{mobileThreatDefenseConnectorId}
```

## <a name="request-headers"></a><span data-ttu-id="e73b1-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e73b1-119">Request headers</span></span>
|<span data-ttu-id="e73b1-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e73b1-120">Header</span></span>|<span data-ttu-id="e73b1-121">値</span><span class="sxs-lookup"><span data-stu-id="e73b1-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e73b1-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e73b1-122">Authorization</span></span>|<span data-ttu-id="e73b1-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="e73b1-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e73b1-124">承諾</span><span class="sxs-lookup"><span data-stu-id="e73b1-124">Accept</span></span>|<span data-ttu-id="e73b1-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e73b1-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e73b1-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="e73b1-126">Request body</span></span>
<span data-ttu-id="e73b1-127">要求本文で、[mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="e73b1-127">In the request body, supply a JSON representation for the [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) object.</span></span>

<span data-ttu-id="e73b1-128">次の表に、[mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) 作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="e73b1-128">The following table shows the properties that are required when you create the [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md).</span></span>

|<span data-ttu-id="e73b1-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e73b1-129">Property</span></span>|<span data-ttu-id="e73b1-130">型</span><span class="sxs-lookup"><span data-stu-id="e73b1-130">Type</span></span>|<span data-ttu-id="e73b1-131">説明</span><span class="sxs-lookup"><span data-stu-id="e73b1-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e73b1-132">id</span><span class="sxs-lookup"><span data-stu-id="e73b1-132">id</span></span>|<span data-ttu-id="e73b1-133">String</span><span class="sxs-lookup"><span data-stu-id="e73b1-133">String</span></span>|<span data-ttu-id="e73b1-134">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="e73b1-134">Not yet documented</span></span>|
|<span data-ttu-id="e73b1-135">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="e73b1-135">lastHeartbeatDateTime</span></span>|<span data-ttu-id="e73b1-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e73b1-136">DateTimeOffset</span></span>|<span data-ttu-id="e73b1-137">データ同期パートナーから受信した最後のハートビートの日時</span><span class="sxs-lookup"><span data-stu-id="e73b1-137">DateTime of last Heartbeat recieved from the Data Sync Partner</span></span>|
|<span data-ttu-id="e73b1-138">partnerState</span><span class="sxs-lookup"><span data-stu-id="e73b1-138">partnerState</span></span>|[<span data-ttu-id="e73b1-139">mobileThreatPartnerTenantState</span><span class="sxs-lookup"><span data-stu-id="e73b1-139">mobileThreatPartnerTenantState</span></span>](../resources/intune-onboarding-mobilethreatpartnertenantstate.md)|<span data-ttu-id="e73b1-140">このアカウントのデータ同期パートナーの状態。</span><span class="sxs-lookup"><span data-stu-id="e73b1-140">Data Sync Partner state for this account.</span></span> <span data-ttu-id="e73b1-141">使用可能な値は、`unavailable`、`available`、`enabled`、`unresponsive` です。</span><span class="sxs-lookup"><span data-stu-id="e73b1-141">Possible values are: `unavailable`, `available`, `enabled`, `unresponsive`.</span></span>|
|<span data-ttu-id="e73b1-142">androidEnabled</span><span class="sxs-lookup"><span data-stu-id="e73b1-142">androidEnabled</span></span>|<span data-ttu-id="e73b1-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="e73b1-143">Boolean</span></span>|<span data-ttu-id="e73b1-144">Android において、準拠評価時にデータ同期パートナーからのデータを使用するかどうかを設定します</span><span class="sxs-lookup"><span data-stu-id="e73b1-144">For Android, set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="e73b1-145">iosEnabled</span><span class="sxs-lookup"><span data-stu-id="e73b1-145">iosEnabled</span></span>|<span data-ttu-id="e73b1-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="e73b1-146">Boolean</span></span>|<span data-ttu-id="e73b1-147">IOS において、準拠評価時にデータ同期パートナーからのデータを使用するかどうかを取得または設定します</span><span class="sxs-lookup"><span data-stu-id="e73b1-147">For IOS, get or set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="e73b1-148">windowsEnabled</span><span class="sxs-lookup"><span data-stu-id="e73b1-148">windowsEnabled</span></span>|<span data-ttu-id="e73b1-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="e73b1-149">Boolean</span></span>|<span data-ttu-id="e73b1-150">Windows の場合は、コンプライアンスの評価時にデータ同期パートナーからのデータを使用するかどうかを取得または設定します。</span><span class="sxs-lookup"><span data-stu-id="e73b1-150">For Windows, get or set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="e73b1-151">macEnabled</span><span class="sxs-lookup"><span data-stu-id="e73b1-151">macEnabled</span></span>|<span data-ttu-id="e73b1-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="e73b1-152">Boolean</span></span>|<span data-ttu-id="e73b1-153">Mac の場合は、コンプライアンス評価中にデータ同期パートナーからのデータを使用する必要があるかどうかを取得または設定します。</span><span class="sxs-lookup"><span data-stu-id="e73b1-153">For Mac, get or set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="e73b1-154">androidDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="e73b1-154">androidDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="e73b1-155">Boolean</span><span class="sxs-lookup"><span data-stu-id="e73b1-155">Boolean</span></span>|<span data-ttu-id="e73b1-156">Android において、デバイスを準拠させる前に Intune がデータ同期パートナーからデータを受信する必要があるかどうかを設定します</span><span class="sxs-lookup"><span data-stu-id="e73b1-156">For Android, set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="e73b1-157">iosDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="e73b1-157">iosDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="e73b1-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="e73b1-158">Boolean</span></span>|<span data-ttu-id="e73b1-159">IOS において、デバイスを準拠させる前に Intune がデータ同期パートナーからデータを受信する必要があるかどうかを設定します</span><span class="sxs-lookup"><span data-stu-id="e73b1-159">For IOS, set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="e73b1-160">windowsDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="e73b1-160">windowsDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="e73b1-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="e73b1-161">Boolean</span></span>|<span data-ttu-id="e73b1-162">Windows の場合は、デバイスに準拠したマークを付ける前に、Intune がデータ同期パートナーからデータを受信する必要があるかどうかを設定します。</span><span class="sxs-lookup"><span data-stu-id="e73b1-162">For Windows, set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="e73b1-163">macDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="e73b1-163">macDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="e73b1-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="e73b1-164">Boolean</span></span>|<span data-ttu-id="e73b1-165">Mac の場合、デバイスに準拠させる前に Intune がデータ同期パートナーからデータを受信する必要があるかどうかを取得または設定します。</span><span class="sxs-lookup"><span data-stu-id="e73b1-165">For Mac, get or set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="e73b1-166">partnerUnsupportedOsVersionBlocked</span><span class="sxs-lookup"><span data-stu-id="e73b1-166">partnerUnsupportedOsVersionBlocked</span></span>|<span data-ttu-id="e73b1-167">ブール型</span><span class="sxs-lookup"><span data-stu-id="e73b1-167">Boolean</span></span>|<span data-ttu-id="e73b1-168">データ同期パートナーの最小バージョンの要件を満たさない、有効なプラットフォーム上のデバイスをブロックするかどうかを取得または設定します</span><span class="sxs-lookup"><span data-stu-id="e73b1-168">Get or set whether to block devices on the enabled platforms that do not meet the minimum version requirements of the Data Sync Partner</span></span>|
|<span data-ttu-id="e73b1-169">partnerUnresponsivenessThresholdInDays</span><span class="sxs-lookup"><span data-stu-id="e73b1-169">partnerUnresponsivenessThresholdInDays</span></span>|<span data-ttu-id="e73b1-170">Int32</span><span class="sxs-lookup"><span data-stu-id="e73b1-170">Int32</span></span>|<span data-ttu-id="e73b1-171">このパートナー統合に関する、テナントごとの無応答許容範囲を取得または設定します</span><span class="sxs-lookup"><span data-stu-id="e73b1-171">Get or Set days the per tenant tolerance to unresponsiveness for this partner integration</span></span>|
|<span data-ttu-id="e73b1-172">allowPartnerToCollectIOSApplicationMetadata</span><span class="sxs-lookup"><span data-stu-id="e73b1-172">allowPartnerToCollectIOSApplicationMetadata</span></span>|<span data-ttu-id="e73b1-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="e73b1-173">Boolean</span></span>|<span data-ttu-id="e73b1-174">IOS デバイスでは、管理者が、インストールされたアプリケーションに関するメタデータを Intune からも収集できるかどうかを管理者が構成できるようにします。</span><span class="sxs-lookup"><span data-stu-id="e73b1-174">For IOS devices, allows the admin to configure whether the data sync partner may also collect metadata about installed applications from Intune</span></span>|



## <a name="response"></a><span data-ttu-id="e73b1-175">応答</span><span class="sxs-lookup"><span data-stu-id="e73b1-175">Response</span></span>
<span data-ttu-id="e73b1-176">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="e73b1-176">If successful, this method returns a `200 OK` response code and an updated [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e73b1-177">例</span><span class="sxs-lookup"><span data-stu-id="e73b1-177">Example</span></span>

### <a name="request"></a><span data-ttu-id="e73b1-178">要求</span><span class="sxs-lookup"><span data-stu-id="e73b1-178">Request</span></span>
<span data-ttu-id="e73b1-179">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="e73b1-179">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/mobileThreatDefenseConnectors/{mobileThreatDefenseConnectorId}
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

### <a name="response"></a><span data-ttu-id="e73b1-180">応答</span><span class="sxs-lookup"><span data-stu-id="e73b1-180">Response</span></span>
<span data-ttu-id="e73b1-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="e73b1-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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






