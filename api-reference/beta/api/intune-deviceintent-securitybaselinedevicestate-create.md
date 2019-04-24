---
title: securityBaselineDeviceState を作成する
description: 新しい securityBaselineDeviceState オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d0b816fb81d85536dcb220b5cb7fc3483549ab85
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32466603"
---
# <a name="create-securitybaselinedevicestate"></a><span data-ttu-id="50a4f-103">securityBaselineDeviceState を作成する</span><span class="sxs-lookup"><span data-stu-id="50a4f-103">Create securityBaselineDeviceState</span></span>

> <span data-ttu-id="50a4f-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="50a4f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="50a4f-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="50a4f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="50a4f-106">新しい[securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="50a4f-106">Create a new [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="50a4f-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="50a4f-107">Prerequisites</span></span>
<span data-ttu-id="50a4f-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="50a4f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="50a4f-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="50a4f-110">Permission type</span></span>|<span data-ttu-id="50a4f-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="50a4f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="50a4f-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="50a4f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="50a4f-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="50a4f-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="50a4f-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="50a4f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="50a4f-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="50a4f-115">Not supported.</span></span>|
|<span data-ttu-id="50a4f-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="50a4f-116">Application</span></span>|<span data-ttu-id="50a4f-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="50a4f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="50a4f-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="50a4f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/templates/{deviceManagementTemplateId}/microsoft.graph.securityBaselineTemplate/deviceStates
```

## <a name="request-headers"></a><span data-ttu-id="50a4f-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="50a4f-119">Request headers</span></span>
|<span data-ttu-id="50a4f-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="50a4f-120">Header</span></span>|<span data-ttu-id="50a4f-121">値</span><span class="sxs-lookup"><span data-stu-id="50a4f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="50a4f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="50a4f-122">Authorization</span></span>|<span data-ttu-id="50a4f-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="50a4f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="50a4f-124">承諾</span><span class="sxs-lookup"><span data-stu-id="50a4f-124">Accept</span></span>|<span data-ttu-id="50a4f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="50a4f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="50a4f-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="50a4f-126">Request body</span></span>
<span data-ttu-id="50a4f-127">要求本文で、securityBaselineDeviceState オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="50a4f-127">In the request body, supply a JSON representation for the securityBaselineDeviceState object.</span></span>

<span data-ttu-id="50a4f-128">次の表に、securityBaselineDeviceState の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="50a4f-128">The following table shows the properties that are required when you create the securityBaselineDeviceState.</span></span>

|<span data-ttu-id="50a4f-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="50a4f-129">Property</span></span>|<span data-ttu-id="50a4f-130">型</span><span class="sxs-lookup"><span data-stu-id="50a4f-130">Type</span></span>|<span data-ttu-id="50a4f-131">説明</span><span class="sxs-lookup"><span data-stu-id="50a4f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="50a4f-132">id</span><span class="sxs-lookup"><span data-stu-id="50a4f-132">id</span></span>|<span data-ttu-id="50a4f-133">String</span><span class="sxs-lookup"><span data-stu-id="50a4f-133">String</span></span>|<span data-ttu-id="50a4f-134">エンティティの一意識別子</span><span class="sxs-lookup"><span data-stu-id="50a4f-134">Unique identifier of the entity</span></span>|
|<span data-ttu-id="50a4f-135">manageddeviceid</span><span class="sxs-lookup"><span data-stu-id="50a4f-135">managedDeviceId</span></span>|<span data-ttu-id="50a4f-136">String</span><span class="sxs-lookup"><span data-stu-id="50a4f-136">String</span></span>|<span data-ttu-id="50a4f-137">Intune デバイス id</span><span class="sxs-lookup"><span data-stu-id="50a4f-137">Intune device id</span></span>|
|<span data-ttu-id="50a4f-138">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="50a4f-138">deviceDisplayName</span></span>|<span data-ttu-id="50a4f-139">String</span><span class="sxs-lookup"><span data-stu-id="50a4f-139">String</span></span>|<span data-ttu-id="50a4f-140">デバイスの表示名</span><span class="sxs-lookup"><span data-stu-id="50a4f-140">Display name of the device</span></span>|
|<span data-ttu-id="50a4f-141">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="50a4f-141">userPrincipalName</span></span>|<span data-ttu-id="50a4f-142">String</span><span class="sxs-lookup"><span data-stu-id="50a4f-142">String</span></span>|<span data-ttu-id="50a4f-143">ユーザー プリンシパル名</span><span class="sxs-lookup"><span data-stu-id="50a4f-143">User Principal Name</span></span>|
|<span data-ttu-id="50a4f-144">state</span><span class="sxs-lookup"><span data-stu-id="50a4f-144">state</span></span>|[<span data-ttu-id="50a4f-145">securityBaselineComplianceState</span><span class="sxs-lookup"><span data-stu-id="50a4f-145">securityBaselineComplianceState</span></span>](../resources/intune-deviceintent-securitybaselinecompliancestate.md)|<span data-ttu-id="50a4f-146">セキュリティベースラインコンプライアンスの状態。</span><span class="sxs-lookup"><span data-stu-id="50a4f-146">Security baseline compliance state.</span></span> <span data-ttu-id="50a4f-147">可能な値は `unknown`、`secure`、`notApplicable`、`notSecure`、`error`、`conflict` です。</span><span class="sxs-lookup"><span data-stu-id="50a4f-147">Possible values are: `unknown`, `secure`, `notApplicable`, `notSecure`, `error`, `conflict`.</span></span>|
|<span data-ttu-id="50a4f-148">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="50a4f-148">lastReportedDateTime</span></span>|<span data-ttu-id="50a4f-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="50a4f-149">DateTimeOffset</span></span>|<span data-ttu-id="50a4f-150">ポリシーレポートの最終変更日時</span><span class="sxs-lookup"><span data-stu-id="50a4f-150">Last modified date time of the policy report</span></span>|



## <a name="response"></a><span data-ttu-id="50a4f-151">応答</span><span class="sxs-lookup"><span data-stu-id="50a4f-151">Response</span></span>
<span data-ttu-id="50a4f-152">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="50a4f-152">If successful, this method returns a `201 Created` response code and a [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="50a4f-153">例</span><span class="sxs-lookup"><span data-stu-id="50a4f-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="50a4f-154">要求</span><span class="sxs-lookup"><span data-stu-id="50a4f-154">Request</span></span>
<span data-ttu-id="50a4f-155">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="50a4f-155">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/templates/{deviceManagementTemplateId}/microsoft.graph.securityBaselineTemplate/deviceStates
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

### <a name="response"></a><span data-ttu-id="50a4f-156">応答</span><span class="sxs-lookup"><span data-stu-id="50a4f-156">Response</span></span>
<span data-ttu-id="50a4f-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="50a4f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





