---
title: DeviceManagementIntentUserState の作成
description: 新しい deviceManagementIntentUserState オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 932fd37d2460e6e6d0c967e2afb401a1a424fa08
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36343448"
---
# <a name="create-devicemanagementintentuserstate"></a><span data-ttu-id="af662-103">DeviceManagementIntentUserState の作成</span><span class="sxs-lookup"><span data-stu-id="af662-103">Create deviceManagementIntentUserState</span></span>

> <span data-ttu-id="af662-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="af662-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="af662-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="af662-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="af662-106">新しい[Devicemanagementintentuserstate](../resources/intune-deviceintent-devicemanagementintentuserstate.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="af662-106">Create a new [deviceManagementIntentUserState](../resources/intune-deviceintent-devicemanagementintentuserstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="af662-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="af662-107">Prerequisites</span></span>
<span data-ttu-id="af662-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="af662-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="af662-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="af662-110">Permission type</span></span>|<span data-ttu-id="af662-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="af662-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="af662-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="af662-112">Delegated (work or school account)</span></span>|<span data-ttu-id="af662-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="af662-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="af662-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="af662-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="af662-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="af662-115">Not supported.</span></span>|
|<span data-ttu-id="af662-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="af662-116">Application</span></span>|<span data-ttu-id="af662-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="af662-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="af662-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="af662-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/intents/{deviceManagementIntentId}/userStates
```

## <a name="request-headers"></a><span data-ttu-id="af662-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="af662-119">Request headers</span></span>
|<span data-ttu-id="af662-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="af662-120">Header</span></span>|<span data-ttu-id="af662-121">値</span><span class="sxs-lookup"><span data-stu-id="af662-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="af662-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="af662-122">Authorization</span></span>|<span data-ttu-id="af662-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="af662-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="af662-124">承諾</span><span class="sxs-lookup"><span data-stu-id="af662-124">Accept</span></span>|<span data-ttu-id="af662-125">application/json</span><span class="sxs-lookup"><span data-stu-id="af662-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="af662-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="af662-126">Request body</span></span>
<span data-ttu-id="af662-127">要求本文で、deviceManagementIntentUserState オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="af662-127">In the request body, supply a JSON representation for the deviceManagementIntentUserState object.</span></span>

<span data-ttu-id="af662-128">次の表に、deviceManagementIntentUserState の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="af662-128">The following table shows the properties that are required when you create the deviceManagementIntentUserState.</span></span>

|<span data-ttu-id="af662-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="af662-129">Property</span></span>|<span data-ttu-id="af662-130">型</span><span class="sxs-lookup"><span data-stu-id="af662-130">Type</span></span>|<span data-ttu-id="af662-131">説明</span><span class="sxs-lookup"><span data-stu-id="af662-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="af662-132">id</span><span class="sxs-lookup"><span data-stu-id="af662-132">id</span></span>|<span data-ttu-id="af662-133">文字列</span><span class="sxs-lookup"><span data-stu-id="af662-133">String</span></span>|<span data-ttu-id="af662-134">ID</span><span class="sxs-lookup"><span data-stu-id="af662-134">The ID</span></span>|
|<span data-ttu-id="af662-135">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="af662-135">userPrincipalName</span></span>|<span data-ttu-id="af662-136">String</span><span class="sxs-lookup"><span data-stu-id="af662-136">String</span></span>|<span data-ttu-id="af662-137">デバイスで報告されているユーザープリンシパル名</span><span class="sxs-lookup"><span data-stu-id="af662-137">The user principal name that is being reported on a device</span></span>|
|<span data-ttu-id="af662-138">userName</span><span class="sxs-lookup"><span data-stu-id="af662-138">userName</span></span>|<span data-ttu-id="af662-139">String</span><span class="sxs-lookup"><span data-stu-id="af662-139">String</span></span>|<span data-ttu-id="af662-140">デバイスで報告されているユーザー名</span><span class="sxs-lookup"><span data-stu-id="af662-140">The user name that is being reported on a device</span></span>|
|<span data-ttu-id="af662-141">deviceCount</span><span class="sxs-lookup"><span data-stu-id="af662-141">deviceCount</span></span>|<span data-ttu-id="af662-142">Int32</span><span class="sxs-lookup"><span data-stu-id="af662-142">Int32</span></span>|<span data-ttu-id="af662-143">目的のためにユーザーに属しているデバイスの数</span><span class="sxs-lookup"><span data-stu-id="af662-143">Count of Devices that belongs to a user for an intent</span></span>|
|<span data-ttu-id="af662-144">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="af662-144">lastReportedDateTime</span></span>|<span data-ttu-id="af662-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="af662-145">DateTimeOffset</span></span>|<span data-ttu-id="af662-146">インテントレポートの最終更新日時</span><span class="sxs-lookup"><span data-stu-id="af662-146">Last modified date time of an intent report</span></span>|
|<span data-ttu-id="af662-147">state</span><span class="sxs-lookup"><span data-stu-id="af662-147">state</span></span>|[<span data-ttu-id="af662-148">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="af662-148">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="af662-149">目的のユーザー状態。</span><span class="sxs-lookup"><span data-stu-id="af662-149">User state for an intent.</span></span> <span data-ttu-id="af662-150">可能な値は、`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned` です。</span><span class="sxs-lookup"><span data-stu-id="af662-150">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|



## <a name="response"></a><span data-ttu-id="af662-151">応答</span><span class="sxs-lookup"><span data-stu-id="af662-151">Response</span></span>
<span data-ttu-id="af662-152">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[Devicemanagementintentuserstate](../resources/intune-deviceintent-devicemanagementintentuserstate.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="af662-152">If successful, this method returns a `201 Created` response code and a [deviceManagementIntentUserState](../resources/intune-deviceintent-devicemanagementintentuserstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="af662-153">例</span><span class="sxs-lookup"><span data-stu-id="af662-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="af662-154">要求</span><span class="sxs-lookup"><span data-stu-id="af662-154">Request</span></span>
<span data-ttu-id="af662-155">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="af662-155">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/userStates
Content-type: application/json
Content-length: 275

{
  "@odata.type": "#microsoft.graph.deviceManagementIntentUserState",
  "userPrincipalName": "User Principal Name value",
  "userName": "User Name value",
  "deviceCount": 11,
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "state": "notApplicable"
}
```

### <a name="response"></a><span data-ttu-id="af662-156">応答</span><span class="sxs-lookup"><span data-stu-id="af662-156">Response</span></span>
<span data-ttu-id="af662-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="af662-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 324

{
  "@odata.type": "#microsoft.graph.deviceManagementIntentUserState",
  "id": "0201286a-286a-0201-6a28-01026a280102",
  "userPrincipalName": "User Principal Name value",
  "userName": "User Name value",
  "deviceCount": 11,
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "state": "notApplicable"
}
```






