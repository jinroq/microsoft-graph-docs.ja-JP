---
title: Create mobileThreatDefenseConnector
description: 新しい mobileThreatDefenseConnector オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 3336c03f86ac7b6d9b926780fccd5cc9e60d5db2
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27950677"
---
# <a name="create-mobilethreatdefenseconnector"></a><span data-ttu-id="3cd82-103">Create mobileThreatDefenseConnector</span><span class="sxs-lookup"><span data-stu-id="3cd82-103">Create mobileThreatDefenseConnector</span></span>

> <span data-ttu-id="3cd82-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="3cd82-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3cd82-105">新しい [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="3cd82-105">Create a new [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3cd82-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="3cd82-106">Prerequisites</span></span>
<span data-ttu-id="3cd82-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3cd82-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3cd82-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3cd82-109">Permission type</span></span>|<span data-ttu-id="3cd82-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="3cd82-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3cd82-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3cd82-111">Delegated (work or school account)</span></span>|<span data-ttu-id="3cd82-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3cd82-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="3cd82-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3cd82-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3cd82-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3cd82-114">Not supported.</span></span>|
|<span data-ttu-id="3cd82-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3cd82-115">Application</span></span>|<span data-ttu-id="3cd82-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3cd82-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3cd82-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3cd82-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/mobileThreatDefenseConnectors
```

## <a name="request-headers"></a><span data-ttu-id="3cd82-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3cd82-118">Request headers</span></span>
|<span data-ttu-id="3cd82-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3cd82-119">Header</span></span>|<span data-ttu-id="3cd82-120">値</span><span class="sxs-lookup"><span data-stu-id="3cd82-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3cd82-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="3cd82-121">Authorization</span></span>|<span data-ttu-id="3cd82-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="3cd82-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3cd82-123">Accept</span><span class="sxs-lookup"><span data-stu-id="3cd82-123">Accept</span></span>|<span data-ttu-id="3cd82-124">application/json</span><span class="sxs-lookup"><span data-stu-id="3cd82-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3cd82-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="3cd82-125">Request body</span></span>
<span data-ttu-id="3cd82-126">要求本文で、mobileThreatDefenseConnector オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="3cd82-126">In the request body, supply a JSON representation for the mobileThreatDefenseConnector object.</span></span>

<span data-ttu-id="3cd82-127">次の表に、mobileThreatDefenseConnector 作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="3cd82-127">The following table shows the properties that are required when you create the mobileThreatDefenseConnector.</span></span>

|<span data-ttu-id="3cd82-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3cd82-128">Property</span></span>|<span data-ttu-id="3cd82-129">種類</span><span class="sxs-lookup"><span data-stu-id="3cd82-129">Type</span></span>|<span data-ttu-id="3cd82-130">説明</span><span class="sxs-lookup"><span data-stu-id="3cd82-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3cd82-131">ID</span><span class="sxs-lookup"><span data-stu-id="3cd82-131">id</span></span>|<span data-ttu-id="3cd82-132">String</span><span class="sxs-lookup"><span data-stu-id="3cd82-132">String</span></span>|<span data-ttu-id="3cd82-133">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="3cd82-133">Not yet documented</span></span>|
|<span data-ttu-id="3cd82-134">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="3cd82-134">lastHeartbeatDateTime</span></span>|<span data-ttu-id="3cd82-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3cd82-135">DateTimeOffset</span></span>|<span data-ttu-id="3cd82-136">データ同期パートナーから受信した最後のハートビートの日時</span><span class="sxs-lookup"><span data-stu-id="3cd82-136">DateTime of last Heartbeat recieved from the Data Sync Partner</span></span>|
|<span data-ttu-id="3cd82-137">partnerState</span><span class="sxs-lookup"><span data-stu-id="3cd82-137">partnerState</span></span>|[<span data-ttu-id="3cd82-138">mobileThreatPartnerTenantState</span><span class="sxs-lookup"><span data-stu-id="3cd82-138">mobileThreatPartnerTenantState</span></span>](../resources/intune-onboarding-mobilethreatpartnertenantstate.md)|<span data-ttu-id="3cd82-139">このアカウントのデータの同期パートナーの状態です。</span><span class="sxs-lookup"><span data-stu-id="3cd82-139">Data Sync Partner state for this account.</span></span> <span data-ttu-id="3cd82-140">可能な値は、`unavailable`、`available`、`enabled`、`unresponsive` です。</span><span class="sxs-lookup"><span data-stu-id="3cd82-140">Possible values are: `unavailable`, `available`, `enabled`, `unresponsive`.</span></span>|
|<span data-ttu-id="3cd82-141">androidEnabled</span><span class="sxs-lookup"><span data-stu-id="3cd82-141">androidEnabled</span></span>|<span data-ttu-id="3cd82-142">ブール型</span><span class="sxs-lookup"><span data-stu-id="3cd82-142">Boolean</span></span>|<span data-ttu-id="3cd82-143">Android において、準拠評価時にデータ同期パートナーからのデータを使用するかどうかを設定します</span><span class="sxs-lookup"><span data-stu-id="3cd82-143">For Android, set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="3cd82-144">iosEnabled</span><span class="sxs-lookup"><span data-stu-id="3cd82-144">iosEnabled</span></span>|<span data-ttu-id="3cd82-145">ブール型</span><span class="sxs-lookup"><span data-stu-id="3cd82-145">Boolean</span></span>|<span data-ttu-id="3cd82-146">IOS において、準拠評価時にデータ同期パートナーからのデータを使用するかどうかを取得または設定します</span><span class="sxs-lookup"><span data-stu-id="3cd82-146">For IOS, get or set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="3cd82-147">androidDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="3cd82-147">androidDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="3cd82-148">ブール型</span><span class="sxs-lookup"><span data-stu-id="3cd82-148">Boolean</span></span>|<span data-ttu-id="3cd82-149">Android において、デバイスを準拠させる前に Intune がデータ同期パートナーからデータを受信する必要があるかどうかを設定します</span><span class="sxs-lookup"><span data-stu-id="3cd82-149">For Android, set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="3cd82-150">iosDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="3cd82-150">iosDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="3cd82-151">ブール型</span><span class="sxs-lookup"><span data-stu-id="3cd82-151">Boolean</span></span>|<span data-ttu-id="3cd82-152">IOS において、デバイスを準拠させる前に Intune がデータ同期パートナーからデータを受信する必要があるかどうかを設定します</span><span class="sxs-lookup"><span data-stu-id="3cd82-152">For IOS, set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="3cd82-153">partnerUnsupportedOsVersionBlocked</span><span class="sxs-lookup"><span data-stu-id="3cd82-153">partnerUnsupportedOsVersionBlocked</span></span>|<span data-ttu-id="3cd82-154">ブール型</span><span class="sxs-lookup"><span data-stu-id="3cd82-154">Boolean</span></span>|<span data-ttu-id="3cd82-155">データ同期パートナーの最小バージョンの要件を満たさない、有効なプラットフォーム上のデバイスをブロックするかどうかを取得または設定します</span><span class="sxs-lookup"><span data-stu-id="3cd82-155">Get or set whether to block devices on the enabled platforms that do not meet the minimum version requirements of the Data Sync Partner</span></span>|
|<span data-ttu-id="3cd82-156">partnerUnresponsivenessThresholdInDays</span><span class="sxs-lookup"><span data-stu-id="3cd82-156">partnerUnresponsivenessThresholdInDays</span></span>|<span data-ttu-id="3cd82-157">Int32</span><span class="sxs-lookup"><span data-stu-id="3cd82-157">Int32</span></span>|<span data-ttu-id="3cd82-158">このパートナー統合に関する、テナントごとの無応答許容範囲を取得または設定します</span><span class="sxs-lookup"><span data-stu-id="3cd82-158">Get or Set days the per tenant tolerance to unresponsiveness for this partner integration</span></span>|



## <a name="response"></a><span data-ttu-id="3cd82-159">応答</span><span class="sxs-lookup"><span data-stu-id="3cd82-159">Response</span></span>
<span data-ttu-id="3cd82-160">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="3cd82-160">If successful, this method returns a `201 Created` response code and a [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3cd82-161">例</span><span class="sxs-lookup"><span data-stu-id="3cd82-161">Example</span></span>
### <a name="request"></a><span data-ttu-id="3cd82-162">要求</span><span class="sxs-lookup"><span data-stu-id="3cd82-162">Request</span></span>
<span data-ttu-id="3cd82-163">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="3cd82-163">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/mobileThreatDefenseConnectors
Content-type: application/json
Content-length: 414

{
  "@odata.type": "#microsoft.graph.mobileThreatDefenseConnector",
  "lastHeartbeatDateTime": "2016-12-31T23:59:37.9174975-08:00",
  "partnerState": "available",
  "androidEnabled": true,
  "iosEnabled": true,
  "androidDeviceBlockedOnMissingPartnerData": true,
  "iosDeviceBlockedOnMissingPartnerData": true,
  "partnerUnsupportedOsVersionBlocked": true,
  "partnerUnresponsivenessThresholdInDays": 6
}
```

### <a name="response"></a><span data-ttu-id="3cd82-164">応答</span><span class="sxs-lookup"><span data-stu-id="3cd82-164">Response</span></span>
<span data-ttu-id="3cd82-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="3cd82-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 463

{
  "@odata.type": "#microsoft.graph.mobileThreatDefenseConnector",
  "id": "e4bede14-de14-e4be-14de-bee414debee4",
  "lastHeartbeatDateTime": "2016-12-31T23:59:37.9174975-08:00",
  "partnerState": "available",
  "androidEnabled": true,
  "iosEnabled": true,
  "androidDeviceBlockedOnMissingPartnerData": true,
  "iosDeviceBlockedOnMissingPartnerData": true,
  "partnerUnsupportedOsVersionBlocked": true,
  "partnerUnresponsivenessThresholdInDays": 6
}
```



