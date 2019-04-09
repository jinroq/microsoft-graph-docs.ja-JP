---
title: securityBaselineDeviceState の更新
description: securityBaselineDeviceState オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a1797f166fea7eb3507ae6a477ae574f4146c558
ms.sourcegitcommit: 77f485ec03a8c917f59d2fbed4df1ec755f3da58
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/08/2019
ms.locfileid: "31522693"
---
# <a name="update-securitybaselinedevicestate"></a><span data-ttu-id="bcd64-103">securityBaselineDeviceState の更新</span><span class="sxs-lookup"><span data-stu-id="bcd64-103">Update securityBaselineDeviceState</span></span>

> <span data-ttu-id="bcd64-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bcd64-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bcd64-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="bcd64-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bcd64-106">[securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="bcd64-106">Update the properties of a [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bcd64-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="bcd64-107">Prerequisites</span></span>
<span data-ttu-id="bcd64-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bcd64-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bcd64-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="bcd64-110">Permission type</span></span>|<span data-ttu-id="bcd64-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="bcd64-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bcd64-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="bcd64-112">Delegated (work or school account)</span></span>|<span data-ttu-id="bcd64-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bcd64-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="bcd64-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="bcd64-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bcd64-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bcd64-115">Not supported.</span></span>|
|<span data-ttu-id="bcd64-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="bcd64-116">Application</span></span>|<span data-ttu-id="bcd64-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bcd64-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bcd64-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="bcd64-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/templates/{deviceManagementTemplateId}/microsoft.graph.securityBaselineTemplate/deviceStates/{securityBaselineDeviceStateId}
```

## <a name="request-headers"></a><span data-ttu-id="bcd64-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="bcd64-119">Request headers</span></span>
|<span data-ttu-id="bcd64-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="bcd64-120">Header</span></span>|<span data-ttu-id="bcd64-121">値</span><span class="sxs-lookup"><span data-stu-id="bcd64-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bcd64-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="bcd64-122">Authorization</span></span>|<span data-ttu-id="bcd64-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="bcd64-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bcd64-124">承諾</span><span class="sxs-lookup"><span data-stu-id="bcd64-124">Accept</span></span>|<span data-ttu-id="bcd64-125">application/json</span><span class="sxs-lookup"><span data-stu-id="bcd64-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bcd64-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="bcd64-126">Request body</span></span>
<span data-ttu-id="bcd64-127">要求本文で、 [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="bcd64-127">In the request body, supply a JSON representation for the [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md) object.</span></span>

<span data-ttu-id="bcd64-128">次の表に、 [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="bcd64-128">The following table shows the properties that are required when you create the [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md).</span></span>

|<span data-ttu-id="bcd64-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bcd64-129">Property</span></span>|<span data-ttu-id="bcd64-130">型</span><span class="sxs-lookup"><span data-stu-id="bcd64-130">Type</span></span>|<span data-ttu-id="bcd64-131">説明</span><span class="sxs-lookup"><span data-stu-id="bcd64-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bcd64-132">id</span><span class="sxs-lookup"><span data-stu-id="bcd64-132">id</span></span>|<span data-ttu-id="bcd64-133">String</span><span class="sxs-lookup"><span data-stu-id="bcd64-133">String</span></span>|<span data-ttu-id="bcd64-134">エンティティの一意識別子</span><span class="sxs-lookup"><span data-stu-id="bcd64-134">Unique identifier of the entity</span></span>|
|<span data-ttu-id="bcd64-135">manageddeviceid</span><span class="sxs-lookup"><span data-stu-id="bcd64-135">managedDeviceId</span></span>|<span data-ttu-id="bcd64-136">文字列</span><span class="sxs-lookup"><span data-stu-id="bcd64-136">String</span></span>|<span data-ttu-id="bcd64-137">Intune デバイス id</span><span class="sxs-lookup"><span data-stu-id="bcd64-137">Intune device id</span></span>|
|<span data-ttu-id="bcd64-138">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="bcd64-138">deviceDisplayName</span></span>|<span data-ttu-id="bcd64-139">String</span><span class="sxs-lookup"><span data-stu-id="bcd64-139">String</span></span>|<span data-ttu-id="bcd64-140">デバイスの表示名</span><span class="sxs-lookup"><span data-stu-id="bcd64-140">Display name of the device</span></span>|
|<span data-ttu-id="bcd64-141">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="bcd64-141">userPrincipalName</span></span>|<span data-ttu-id="bcd64-142">String</span><span class="sxs-lookup"><span data-stu-id="bcd64-142">String</span></span>|<span data-ttu-id="bcd64-143">ユーザー プリンシパル名</span><span class="sxs-lookup"><span data-stu-id="bcd64-143">User Principal Name</span></span>|
|<span data-ttu-id="bcd64-144">state</span><span class="sxs-lookup"><span data-stu-id="bcd64-144">state</span></span>|[<span data-ttu-id="bcd64-145">securityBaselineComplianceState</span><span class="sxs-lookup"><span data-stu-id="bcd64-145">securityBaselineComplianceState</span></span>](../resources/intune-deviceintent-securitybaselinecompliancestate.md)|<span data-ttu-id="bcd64-146">セキュリティベースラインコンプライアンスの状態。</span><span class="sxs-lookup"><span data-stu-id="bcd64-146">Security baseline compliance state.</span></span> <span data-ttu-id="bcd64-147">可能な値は `unknown`、`secure`、`notApplicable`、`notSecure`、`error`、`conflict` です。</span><span class="sxs-lookup"><span data-stu-id="bcd64-147">Possible values are: `unknown`, `secure`, `notApplicable`, `notSecure`, `error`, `conflict`.</span></span>|
|<span data-ttu-id="bcd64-148">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="bcd64-148">lastReportedDateTime</span></span>|<span data-ttu-id="bcd64-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bcd64-149">DateTimeOffset</span></span>|<span data-ttu-id="bcd64-150">ポリシーレポートの最終変更日時</span><span class="sxs-lookup"><span data-stu-id="bcd64-150">Last modified date time of the policy report</span></span>|



## <a name="response"></a><span data-ttu-id="bcd64-151">応答</span><span class="sxs-lookup"><span data-stu-id="bcd64-151">Response</span></span>
<span data-ttu-id="bcd64-152">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="bcd64-152">If successful, this method returns a `200 OK` response code and an updated [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bcd64-153">例</span><span class="sxs-lookup"><span data-stu-id="bcd64-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="bcd64-154">要求</span><span class="sxs-lookup"><span data-stu-id="bcd64-154">Request</span></span>
<span data-ttu-id="bcd64-155">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="bcd64-155">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/templates/{deviceManagementTemplateId}/microsoft.graph.securityBaselineTemplate/deviceStates/{securityBaselineDeviceStateId}
Content-type: application/json
Content-length: 310

{
  "@odata.type": "#microsoft.graph.securityBaselineDeviceState",
  "managedDeviceId": "Managed Device Id value",
  "deviceDisplayName": "Device Display Name value",
  "userPrincipalName": "User Principal Name value",
  "state": "secure",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00"
}
```

### <a name="response"></a><span data-ttu-id="bcd64-156">応答</span><span class="sxs-lookup"><span data-stu-id="bcd64-156">Response</span></span>
<span data-ttu-id="bcd64-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="bcd64-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 359

{
  "@odata.type": "#microsoft.graph.securityBaselineDeviceState",
  "id": "182749bf-49bf-1827-bf49-2718bf492718",
  "managedDeviceId": "Managed Device Id value",
  "deviceDisplayName": "Device Display Name value",
  "userPrincipalName": "User Principal Name value",
  "state": "secure",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00"
}
```







