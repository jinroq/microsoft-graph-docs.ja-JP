---
title: SecurityBaselineDeviceState の更新
description: SecurityBaselineDeviceState オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 26a4a050320a669e27603cdf4eb2d3e93f310602
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33914465"
---
# <a name="update-securitybaselinedevicestate"></a><span data-ttu-id="7f3c6-103">SecurityBaselineDeviceState の更新</span><span class="sxs-lookup"><span data-stu-id="7f3c6-103">Update securityBaselineDeviceState</span></span>

> <span data-ttu-id="7f3c6-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7f3c6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7f3c6-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="7f3c6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7f3c6-106">[SecurityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="7f3c6-106">Update the properties of a [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7f3c6-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="7f3c6-107">Prerequisites</span></span>
<span data-ttu-id="7f3c6-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7f3c6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7f3c6-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7f3c6-110">Permission type</span></span>|<span data-ttu-id="7f3c6-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="7f3c6-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7f3c6-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7f3c6-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7f3c6-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f3c6-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7f3c6-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7f3c6-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7f3c6-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7f3c6-115">Not supported.</span></span>|
|<span data-ttu-id="7f3c6-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7f3c6-116">Application</span></span>|<span data-ttu-id="7f3c6-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7f3c6-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7f3c6-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7f3c6-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/templates/{deviceManagementTemplateId}/microsoft.graph.securityBaselineTemplate/deviceStates/{securityBaselineDeviceStateId}
```

## <a name="request-headers"></a><span data-ttu-id="7f3c6-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7f3c6-119">Request headers</span></span>
|<span data-ttu-id="7f3c6-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7f3c6-120">Header</span></span>|<span data-ttu-id="7f3c6-121">値</span><span class="sxs-lookup"><span data-stu-id="7f3c6-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7f3c6-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="7f3c6-122">Authorization</span></span>|<span data-ttu-id="7f3c6-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="7f3c6-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7f3c6-124">承諾</span><span class="sxs-lookup"><span data-stu-id="7f3c6-124">Accept</span></span>|<span data-ttu-id="7f3c6-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7f3c6-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7f3c6-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="7f3c6-126">Request body</span></span>
<span data-ttu-id="7f3c6-127">要求本文で、 [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="7f3c6-127">In the request body, supply a JSON representation for the [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md) object.</span></span>

<span data-ttu-id="7f3c6-128">次の表に、 [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="7f3c6-128">The following table shows the properties that are required when you create the [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md).</span></span>

|<span data-ttu-id="7f3c6-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7f3c6-129">Property</span></span>|<span data-ttu-id="7f3c6-130">型</span><span class="sxs-lookup"><span data-stu-id="7f3c6-130">Type</span></span>|<span data-ttu-id="7f3c6-131">説明</span><span class="sxs-lookup"><span data-stu-id="7f3c6-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7f3c6-132">id</span><span class="sxs-lookup"><span data-stu-id="7f3c6-132">id</span></span>|<span data-ttu-id="7f3c6-133">文字列</span><span class="sxs-lookup"><span data-stu-id="7f3c6-133">String</span></span>|<span data-ttu-id="7f3c6-134">エンティティの一意識別子</span><span class="sxs-lookup"><span data-stu-id="7f3c6-134">Unique identifier of the entity</span></span>|
|<span data-ttu-id="7f3c6-135">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="7f3c6-135">managedDeviceId</span></span>|<span data-ttu-id="7f3c6-136">String</span><span class="sxs-lookup"><span data-stu-id="7f3c6-136">String</span></span>|<span data-ttu-id="7f3c6-137">Intune デバイス id</span><span class="sxs-lookup"><span data-stu-id="7f3c6-137">Intune device id</span></span>|
|<span data-ttu-id="7f3c6-138">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="7f3c6-138">deviceDisplayName</span></span>|<span data-ttu-id="7f3c6-139">String</span><span class="sxs-lookup"><span data-stu-id="7f3c6-139">String</span></span>|<span data-ttu-id="7f3c6-140">デバイスの表示名</span><span class="sxs-lookup"><span data-stu-id="7f3c6-140">Display name of the device</span></span>|
|<span data-ttu-id="7f3c6-141">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="7f3c6-141">userPrincipalName</span></span>|<span data-ttu-id="7f3c6-142">String</span><span class="sxs-lookup"><span data-stu-id="7f3c6-142">String</span></span>|<span data-ttu-id="7f3c6-143">ユーザー プリンシパル名</span><span class="sxs-lookup"><span data-stu-id="7f3c6-143">User Principal Name</span></span>|
|<span data-ttu-id="7f3c6-144">state</span><span class="sxs-lookup"><span data-stu-id="7f3c6-144">state</span></span>|[<span data-ttu-id="7f3c6-145">securityBaselineComplianceState</span><span class="sxs-lookup"><span data-stu-id="7f3c6-145">securityBaselineComplianceState</span></span>](../resources/intune-deviceintent-securitybaselinecompliancestate.md)|<span data-ttu-id="7f3c6-146">セキュリティベースラインコンプライアンスの状態。</span><span class="sxs-lookup"><span data-stu-id="7f3c6-146">Security baseline compliance state.</span></span> <span data-ttu-id="7f3c6-147">使用可能な値: `unknown`、`secure`、`notApplicable`、`notSecure`、`error`、`conflict`。</span><span class="sxs-lookup"><span data-stu-id="7f3c6-147">Possible values are: `unknown`, `secure`, `notApplicable`, `notSecure`, `error`, `conflict`.</span></span>|
|<span data-ttu-id="7f3c6-148">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="7f3c6-148">lastReportedDateTime</span></span>|<span data-ttu-id="7f3c6-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7f3c6-149">DateTimeOffset</span></span>|<span data-ttu-id="7f3c6-150">ポリシーレポートの最終変更日時</span><span class="sxs-lookup"><span data-stu-id="7f3c6-150">Last modified date time of the policy report</span></span>|



## <a name="response"></a><span data-ttu-id="7f3c6-151">応答</span><span class="sxs-lookup"><span data-stu-id="7f3c6-151">Response</span></span>
<span data-ttu-id="7f3c6-152">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="7f3c6-152">If successful, this method returns a `200 OK` response code and an updated [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7f3c6-153">例</span><span class="sxs-lookup"><span data-stu-id="7f3c6-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="7f3c6-154">要求</span><span class="sxs-lookup"><span data-stu-id="7f3c6-154">Request</span></span>
<span data-ttu-id="7f3c6-155">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="7f3c6-155">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="7f3c6-156">応答</span><span class="sxs-lookup"><span data-stu-id="7f3c6-156">Response</span></span>
<span data-ttu-id="7f3c6-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="7f3c6-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




