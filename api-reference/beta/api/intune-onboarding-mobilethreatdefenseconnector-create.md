---
title: Create mobileThreatDefenseConnector
description: 新しい mobileThreatDefenseConnector オブジェクトを作成します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 68da053288b635454c3343bc2fd4795c51456095
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29418611"
---
# <a name="create-mobilethreatdefenseconnector"></a><span data-ttu-id="c2dee-103">Create mobileThreatDefenseConnector</span><span class="sxs-lookup"><span data-stu-id="c2dee-103">Create mobileThreatDefenseConnector</span></span>

> <span data-ttu-id="c2dee-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c2dee-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c2dee-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c2dee-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c2dee-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="c2dee-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c2dee-107">新しい [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="c2dee-107">Create a new [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c2dee-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="c2dee-108">Prerequisites</span></span>
<span data-ttu-id="c2dee-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c2dee-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="c2dee-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c2dee-111">Permission type</span></span>|<span data-ttu-id="c2dee-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="c2dee-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c2dee-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c2dee-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c2dee-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c2dee-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="c2dee-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c2dee-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c2dee-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c2dee-116">Not supported.</span></span>|
|<span data-ttu-id="c2dee-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c2dee-117">Application</span></span>|<span data-ttu-id="c2dee-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c2dee-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c2dee-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c2dee-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/mobileThreatDefenseConnectors
```

## <a name="request-headers"></a><span data-ttu-id="c2dee-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c2dee-120">Request headers</span></span>
|<span data-ttu-id="c2dee-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c2dee-121">Header</span></span>|<span data-ttu-id="c2dee-122">値</span><span class="sxs-lookup"><span data-stu-id="c2dee-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c2dee-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c2dee-123">Authorization</span></span>|<span data-ttu-id="c2dee-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="c2dee-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c2dee-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c2dee-125">Accept</span></span>|<span data-ttu-id="c2dee-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c2dee-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c2dee-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="c2dee-127">Request body</span></span>
<span data-ttu-id="c2dee-128">要求本文で、mobileThreatDefenseConnector オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="c2dee-128">In the request body, supply a JSON representation for the mobileThreatDefenseConnector object.</span></span>

<span data-ttu-id="c2dee-129">次の表に、mobileThreatDefenseConnector 作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="c2dee-129">The following table shows the properties that are required when you create the mobileThreatDefenseConnector.</span></span>

|<span data-ttu-id="c2dee-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c2dee-130">Property</span></span>|<span data-ttu-id="c2dee-131">型</span><span class="sxs-lookup"><span data-stu-id="c2dee-131">Type</span></span>|<span data-ttu-id="c2dee-132">説明</span><span class="sxs-lookup"><span data-stu-id="c2dee-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c2dee-133">id</span><span class="sxs-lookup"><span data-stu-id="c2dee-133">id</span></span>|<span data-ttu-id="c2dee-134">String</span><span class="sxs-lookup"><span data-stu-id="c2dee-134">String</span></span>|<span data-ttu-id="c2dee-135">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="c2dee-135">Not yet documented</span></span>|
|<span data-ttu-id="c2dee-136">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="c2dee-136">lastHeartbeatDateTime</span></span>|<span data-ttu-id="c2dee-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c2dee-137">DateTimeOffset</span></span>|<span data-ttu-id="c2dee-138">データ同期パートナーから受信した最後のハートビートの日時</span><span class="sxs-lookup"><span data-stu-id="c2dee-138">DateTime of last Heartbeat recieved from the Data Sync Partner</span></span>|
|<span data-ttu-id="c2dee-139">partnerState</span><span class="sxs-lookup"><span data-stu-id="c2dee-139">partnerState</span></span>|[<span data-ttu-id="c2dee-140">mobileThreatPartnerTenantState</span><span class="sxs-lookup"><span data-stu-id="c2dee-140">mobileThreatPartnerTenantState</span></span>](../resources/intune-onboarding-mobilethreatpartnertenantstate.md)|<span data-ttu-id="c2dee-141">このアカウントのデータの同期パートナーの状態です。</span><span class="sxs-lookup"><span data-stu-id="c2dee-141">Data Sync Partner state for this account.</span></span> <span data-ttu-id="c2dee-142">可能な値は、`unavailable`、`available`、`enabled`、`unresponsive` です。</span><span class="sxs-lookup"><span data-stu-id="c2dee-142">Possible values are: `unavailable`, `available`, `enabled`, `unresponsive`.</span></span>|
|<span data-ttu-id="c2dee-143">androidEnabled</span><span class="sxs-lookup"><span data-stu-id="c2dee-143">androidEnabled</span></span>|<span data-ttu-id="c2dee-144">ブール型</span><span class="sxs-lookup"><span data-stu-id="c2dee-144">Boolean</span></span>|<span data-ttu-id="c2dee-145">Android において、準拠評価時にデータ同期パートナーからのデータを使用するかどうかを設定します</span><span class="sxs-lookup"><span data-stu-id="c2dee-145">For Android, set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="c2dee-146">iosEnabled</span><span class="sxs-lookup"><span data-stu-id="c2dee-146">iosEnabled</span></span>|<span data-ttu-id="c2dee-147">ブール型</span><span class="sxs-lookup"><span data-stu-id="c2dee-147">Boolean</span></span>|<span data-ttu-id="c2dee-148">IOS において、準拠評価時にデータ同期パートナーからのデータを使用するかどうかを取得または設定します</span><span class="sxs-lookup"><span data-stu-id="c2dee-148">For IOS, get or set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="c2dee-149">windowsEnabled</span><span class="sxs-lookup"><span data-stu-id="c2dee-149">windowsEnabled</span></span>|<span data-ttu-id="c2dee-150">Boolean</span><span class="sxs-lookup"><span data-stu-id="c2dee-150">Boolean</span></span>|<span data-ttu-id="c2dee-151">ウィンドウを取得または設定するコンプライアンスの評価中にデータの同期パートナーからのデータを使用する必要があるかどうか</span><span class="sxs-lookup"><span data-stu-id="c2dee-151">For Windows, get or set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="c2dee-152">macEnabled</span><span class="sxs-lookup"><span data-stu-id="c2dee-152">macEnabled</span></span>|<span data-ttu-id="c2dee-153">Boolean</span><span class="sxs-lookup"><span data-stu-id="c2dee-153">Boolean</span></span>|<span data-ttu-id="c2dee-154">For Mac を取得または設定するコンプライアンスの評価中にデータの同期パートナーからのデータを使用する必要があるかどうか</span><span class="sxs-lookup"><span data-stu-id="c2dee-154">For Mac, get or set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="c2dee-155">androidDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="c2dee-155">androidDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="c2dee-156">ブール型</span><span class="sxs-lookup"><span data-stu-id="c2dee-156">Boolean</span></span>|<span data-ttu-id="c2dee-157">Android において、デバイスを準拠させる前に Intune がデータ同期パートナーからデータを受信する必要があるかどうかを設定します</span><span class="sxs-lookup"><span data-stu-id="c2dee-157">For Android, set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="c2dee-158">iosDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="c2dee-158">iosDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="c2dee-159">ブール型</span><span class="sxs-lookup"><span data-stu-id="c2dee-159">Boolean</span></span>|<span data-ttu-id="c2dee-160">IOS において、デバイスを準拠させる前に Intune がデータ同期パートナーからデータを受信する必要があるかどうかを設定します</span><span class="sxs-lookup"><span data-stu-id="c2dee-160">For IOS, set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="c2dee-161">windowsDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="c2dee-161">windowsDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="c2dee-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="c2dee-162">Boolean</span></span>|<span data-ttu-id="c2dee-163">Windows Intune は、準拠デバイスをマークする前にデータの同期パートナーからデータを受信する必要があるかどうかを設定します。</span><span class="sxs-lookup"><span data-stu-id="c2dee-163">For Windows, set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="c2dee-164">macDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="c2dee-164">macDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="c2dee-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="c2dee-165">Boolean</span></span>|<span data-ttu-id="c2dee-166">For Mac を取得または設定する Intune 準拠デバイスをマークする前にデータの同期パートナーからデータを受信する必要があるかどうか</span><span class="sxs-lookup"><span data-stu-id="c2dee-166">For Mac, get or set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="c2dee-167">partnerUnsupportedOsVersionBlocked</span><span class="sxs-lookup"><span data-stu-id="c2dee-167">partnerUnsupportedOsVersionBlocked</span></span>|<span data-ttu-id="c2dee-168">ブール型</span><span class="sxs-lookup"><span data-stu-id="c2dee-168">Boolean</span></span>|<span data-ttu-id="c2dee-169">データ同期パートナーの最小バージョンの要件を満たさない、有効なプラットフォーム上のデバイスをブロックするかどうかを取得または設定します</span><span class="sxs-lookup"><span data-stu-id="c2dee-169">Get or set whether to block devices on the enabled platforms that do not meet the minimum version requirements of the Data Sync Partner</span></span>|
|<span data-ttu-id="c2dee-170">partnerUnresponsivenessThresholdInDays</span><span class="sxs-lookup"><span data-stu-id="c2dee-170">partnerUnresponsivenessThresholdInDays</span></span>|<span data-ttu-id="c2dee-171">Int32</span><span class="sxs-lookup"><span data-stu-id="c2dee-171">Int32</span></span>|<span data-ttu-id="c2dee-172">このパートナー統合に関する、テナントごとの無応答への許容日数の取得または設定を行います</span><span class="sxs-lookup"><span data-stu-id="c2dee-172">Get or Set days the per tenant tolerance to unresponsiveness for this partner integration</span></span>|
|<span data-ttu-id="c2dee-173">allowPartnerToCollectIOSApplicationMetadata</span><span class="sxs-lookup"><span data-stu-id="c2dee-173">allowPartnerToCollectIOSApplicationMetadata</span></span>|<span data-ttu-id="c2dee-174">Boolean</span><span class="sxs-lookup"><span data-stu-id="c2dee-174">Boolean</span></span>|<span data-ttu-id="c2dee-175">IOS デバイスでは、データの同期パートナー Intune からインストールされているアプリケーションについてのメタデータの収集もあるかどうかを構成するのには管理者では、します。</span><span class="sxs-lookup"><span data-stu-id="c2dee-175">For IOS devices, allows the admin to configure whether the data sync partner may also collect metadata about installed applications from Intune</span></span>|



## <a name="response"></a><span data-ttu-id="c2dee-176">応答</span><span class="sxs-lookup"><span data-stu-id="c2dee-176">Response</span></span>
<span data-ttu-id="c2dee-177">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="c2dee-177">If successful, this method returns a `201 Created` response code and a [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c2dee-178">例</span><span class="sxs-lookup"><span data-stu-id="c2dee-178">Example</span></span>

### <a name="request"></a><span data-ttu-id="c2dee-179">要求</span><span class="sxs-lookup"><span data-stu-id="c2dee-179">Request</span></span>
<span data-ttu-id="c2dee-180">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c2dee-180">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c2dee-181">応答</span><span class="sxs-lookup"><span data-stu-id="c2dee-181">Response</span></span>
<span data-ttu-id="c2dee-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="c2dee-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




