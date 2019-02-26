---
title: mobileThreatDefenseConnector の更新
description: mobileThreatDefenseConnector オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 71d72ca72e3eba2522881081d0b44804a33fd803
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30262308"
---
# <a name="update-mobilethreatdefenseconnector"></a><span data-ttu-id="f0e98-103">mobileThreatDefenseConnector の更新</span><span class="sxs-lookup"><span data-stu-id="f0e98-103">Update mobileThreatDefenseConnector</span></span>

> <span data-ttu-id="f0e98-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="f0e98-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f0e98-105">[mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="f0e98-105">Update the properties of a [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f0e98-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="f0e98-106">Prerequisites</span></span>
<span data-ttu-id="f0e98-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f0e98-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="f0e98-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f0e98-109">Permission type</span></span>|<span data-ttu-id="f0e98-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="f0e98-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f0e98-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f0e98-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f0e98-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f0e98-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="f0e98-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f0e98-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f0e98-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f0e98-114">Not supported.</span></span>|
|<span data-ttu-id="f0e98-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f0e98-115">Application</span></span>|<span data-ttu-id="f0e98-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f0e98-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f0e98-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f0e98-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/mobileThreatDefenseConnectors/{mobileThreatDefenseConnectorId}
```

## <a name="request-headers"></a><span data-ttu-id="f0e98-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f0e98-118">Request headers</span></span>
|<span data-ttu-id="f0e98-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f0e98-119">Header</span></span>|<span data-ttu-id="f0e98-120">値</span><span class="sxs-lookup"><span data-stu-id="f0e98-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f0e98-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="f0e98-121">Authorization</span></span>|<span data-ttu-id="f0e98-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="f0e98-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f0e98-123">承諾</span><span class="sxs-lookup"><span data-stu-id="f0e98-123">Accept</span></span>|<span data-ttu-id="f0e98-124">application/json</span><span class="sxs-lookup"><span data-stu-id="f0e98-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f0e98-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="f0e98-125">Request body</span></span>
<span data-ttu-id="f0e98-126">要求本文で、[mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="f0e98-126">In the request body, supply a JSON representation for the [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) object.</span></span>

<span data-ttu-id="f0e98-127">次の表に、[mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) 作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="f0e98-127">The following table shows the properties that are required when you create the [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md).</span></span>

|<span data-ttu-id="f0e98-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f0e98-128">Property</span></span>|<span data-ttu-id="f0e98-129">型</span><span class="sxs-lookup"><span data-stu-id="f0e98-129">Type</span></span>|<span data-ttu-id="f0e98-130">説明</span><span class="sxs-lookup"><span data-stu-id="f0e98-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f0e98-131">id</span><span class="sxs-lookup"><span data-stu-id="f0e98-131">id</span></span>|<span data-ttu-id="f0e98-132">String</span><span class="sxs-lookup"><span data-stu-id="f0e98-132">String</span></span>|<span data-ttu-id="f0e98-133">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="f0e98-133">Not yet documented</span></span>|
|<span data-ttu-id="f0e98-134">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="f0e98-134">lastHeartbeatDateTime</span></span>|<span data-ttu-id="f0e98-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f0e98-135">DateTimeOffset</span></span>|<span data-ttu-id="f0e98-136">データ同期パートナーから受信した最後のハートビートの日時</span><span class="sxs-lookup"><span data-stu-id="f0e98-136">DateTime of last Heartbeat recieved from the Data Sync Partner</span></span>|
|<span data-ttu-id="f0e98-137">partnerState</span><span class="sxs-lookup"><span data-stu-id="f0e98-137">partnerState</span></span>|[<span data-ttu-id="f0e98-138">mobileThreatPartnerTenantState</span><span class="sxs-lookup"><span data-stu-id="f0e98-138">mobileThreatPartnerTenantState</span></span>](../resources/intune-onboarding-mobilethreatpartnertenantstate.md)|<span data-ttu-id="f0e98-139">このアカウントのデータ同期パートナーの状態。</span><span class="sxs-lookup"><span data-stu-id="f0e98-139">Data Sync Partner state for this account.</span></span> <span data-ttu-id="f0e98-140">使用可能な値は、`unavailable`、`available`、`enabled`、`unresponsive` です。</span><span class="sxs-lookup"><span data-stu-id="f0e98-140">Possible values are: `unavailable`, `available`, `enabled`, `unresponsive`.</span></span>|
|<span data-ttu-id="f0e98-141">androidEnabled</span><span class="sxs-lookup"><span data-stu-id="f0e98-141">androidEnabled</span></span>|<span data-ttu-id="f0e98-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0e98-142">Boolean</span></span>|<span data-ttu-id="f0e98-143">Android において、準拠評価時にデータ同期パートナーからのデータを使用するかどうかを設定します</span><span class="sxs-lookup"><span data-stu-id="f0e98-143">For Android, set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="f0e98-144">iosEnabled</span><span class="sxs-lookup"><span data-stu-id="f0e98-144">iosEnabled</span></span>|<span data-ttu-id="f0e98-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0e98-145">Boolean</span></span>|<span data-ttu-id="f0e98-146">IOS において、準拠評価時にデータ同期パートナーからのデータを使用するかどうかを取得または設定します</span><span class="sxs-lookup"><span data-stu-id="f0e98-146">For IOS, get or set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="f0e98-147">androidDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="f0e98-147">androidDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="f0e98-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0e98-148">Boolean</span></span>|<span data-ttu-id="f0e98-149">Android において、デバイスを準拠させる前に Intune がデータ同期パートナーからデータを受信する必要があるかどうかを設定します</span><span class="sxs-lookup"><span data-stu-id="f0e98-149">For Android, set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="f0e98-150">iosDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="f0e98-150">iosDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="f0e98-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0e98-151">Boolean</span></span>|<span data-ttu-id="f0e98-152">IOS において、デバイスを準拠させる前に Intune がデータ同期パートナーからデータを受信する必要があるかどうかを設定します</span><span class="sxs-lookup"><span data-stu-id="f0e98-152">For IOS, set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="f0e98-153">partnerUnsupportedOsVersionBlocked</span><span class="sxs-lookup"><span data-stu-id="f0e98-153">partnerUnsupportedOsVersionBlocked</span></span>|<span data-ttu-id="f0e98-154">ブール型</span><span class="sxs-lookup"><span data-stu-id="f0e98-154">Boolean</span></span>|<span data-ttu-id="f0e98-155">データ同期パートナーの最小バージョンの要件を満たさない、有効なプラットフォーム上のデバイスをブロックするかどうかを取得または設定します</span><span class="sxs-lookup"><span data-stu-id="f0e98-155">Get or set whether to block devices on the enabled platforms that do not meet the minimum version requirements of the Data Sync Partner</span></span>|
|<span data-ttu-id="f0e98-156">partnerUnresponsivenessThresholdInDays</span><span class="sxs-lookup"><span data-stu-id="f0e98-156">partnerUnresponsivenessThresholdInDays</span></span>|<span data-ttu-id="f0e98-157">Int32</span><span class="sxs-lookup"><span data-stu-id="f0e98-157">Int32</span></span>|<span data-ttu-id="f0e98-158">このパートナー統合に関する、テナントごとの無応答許容範囲を取得または設定します</span><span class="sxs-lookup"><span data-stu-id="f0e98-158">Get or Set days the per tenant tolerance to unresponsiveness for this partner integration</span></span>|



## <a name="response"></a><span data-ttu-id="f0e98-159">応答</span><span class="sxs-lookup"><span data-stu-id="f0e98-159">Response</span></span>
<span data-ttu-id="f0e98-160">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="f0e98-160">If successful, this method returns a `200 OK` response code and an updated [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f0e98-161">例</span><span class="sxs-lookup"><span data-stu-id="f0e98-161">Example</span></span>

### <a name="request"></a><span data-ttu-id="f0e98-162">要求</span><span class="sxs-lookup"><span data-stu-id="f0e98-162">Request</span></span>
<span data-ttu-id="f0e98-163">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f0e98-163">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/mobileThreatDefenseConnectors/{mobileThreatDefenseConnectorId}
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

### <a name="response"></a><span data-ttu-id="f0e98-164">応答</span><span class="sxs-lookup"><span data-stu-id="f0e98-164">Response</span></span>
<span data-ttu-id="f0e98-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f0e98-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



