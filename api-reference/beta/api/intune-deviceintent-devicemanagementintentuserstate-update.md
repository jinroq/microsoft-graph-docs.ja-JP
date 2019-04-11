---
title: devicemanagementintentuserstate の更新
description: devicemanagementintentuserstate オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4590a77b20cd5584c4d3edc885e869ba8d3064a6
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31775115"
---
# <a name="update-devicemanagementintentuserstate"></a><span data-ttu-id="8091c-103">devicemanagementintentuserstate の更新</span><span class="sxs-lookup"><span data-stu-id="8091c-103">Update deviceManagementIntentUserState</span></span>

> <span data-ttu-id="8091c-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8091c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8091c-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="8091c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8091c-106">[devicemanagementintentuserstate](../resources/intune-deviceintent-devicemanagementintentuserstate.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="8091c-106">Update the properties of a [deviceManagementIntentUserState](../resources/intune-deviceintent-devicemanagementintentuserstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8091c-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="8091c-107">Prerequisites</span></span>
<span data-ttu-id="8091c-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8091c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8091c-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8091c-110">Permission type</span></span>|<span data-ttu-id="8091c-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="8091c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8091c-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8091c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8091c-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8091c-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8091c-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8091c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8091c-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8091c-115">Not supported.</span></span>|
|<span data-ttu-id="8091c-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8091c-116">Application</span></span>|<span data-ttu-id="8091c-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8091c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8091c-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8091c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/intents/{deviceManagementIntentId}/userStates/{deviceManagementIntentUserStateId}
```

## <a name="request-headers"></a><span data-ttu-id="8091c-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8091c-119">Request headers</span></span>
|<span data-ttu-id="8091c-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8091c-120">Header</span></span>|<span data-ttu-id="8091c-121">値</span><span class="sxs-lookup"><span data-stu-id="8091c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8091c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8091c-122">Authorization</span></span>|<span data-ttu-id="8091c-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="8091c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8091c-124">承諾</span><span class="sxs-lookup"><span data-stu-id="8091c-124">Accept</span></span>|<span data-ttu-id="8091c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8091c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8091c-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="8091c-126">Request body</span></span>
<span data-ttu-id="8091c-127">要求本文で、 [devicemanagementintentuserstate](../resources/intune-deviceintent-devicemanagementintentuserstate.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="8091c-127">In the request body, supply a JSON representation for the [deviceManagementIntentUserState](../resources/intune-deviceintent-devicemanagementintentuserstate.md) object.</span></span>

<span data-ttu-id="8091c-128">次の表に、 [devicemanagementintentuserstate](../resources/intune-deviceintent-devicemanagementintentuserstate.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="8091c-128">The following table shows the properties that are required when you create the [deviceManagementIntentUserState](../resources/intune-deviceintent-devicemanagementintentuserstate.md).</span></span>

|<span data-ttu-id="8091c-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8091c-129">Property</span></span>|<span data-ttu-id="8091c-130">型</span><span class="sxs-lookup"><span data-stu-id="8091c-130">Type</span></span>|<span data-ttu-id="8091c-131">説明</span><span class="sxs-lookup"><span data-stu-id="8091c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8091c-132">id</span><span class="sxs-lookup"><span data-stu-id="8091c-132">id</span></span>|<span data-ttu-id="8091c-133">String</span><span class="sxs-lookup"><span data-stu-id="8091c-133">String</span></span>|<span data-ttu-id="8091c-134">ID</span><span class="sxs-lookup"><span data-stu-id="8091c-134">The ID</span></span>|
|<span data-ttu-id="8091c-135">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="8091c-135">userPrincipalName</span></span>|<span data-ttu-id="8091c-136">String</span><span class="sxs-lookup"><span data-stu-id="8091c-136">String</span></span>|<span data-ttu-id="8091c-137">デバイスで報告されているユーザープリンシパル名</span><span class="sxs-lookup"><span data-stu-id="8091c-137">The user principal name that is being reported on a device</span></span>|
|<span data-ttu-id="8091c-138">userName</span><span class="sxs-lookup"><span data-stu-id="8091c-138">userName</span></span>|<span data-ttu-id="8091c-139">String</span><span class="sxs-lookup"><span data-stu-id="8091c-139">String</span></span>|<span data-ttu-id="8091c-140">デバイスで報告されているユーザー名</span><span class="sxs-lookup"><span data-stu-id="8091c-140">The user name that is being reported on a device</span></span>|
|<span data-ttu-id="8091c-141">deviceCount</span><span class="sxs-lookup"><span data-stu-id="8091c-141">deviceCount</span></span>|<span data-ttu-id="8091c-142">Int32</span><span class="sxs-lookup"><span data-stu-id="8091c-142">Int32</span></span>|<span data-ttu-id="8091c-143">目的のためにユーザーに属しているデバイスの数</span><span class="sxs-lookup"><span data-stu-id="8091c-143">Count of Devices that belongs to a user for an intent</span></span>|
|<span data-ttu-id="8091c-144">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="8091c-144">lastReportedDateTime</span></span>|<span data-ttu-id="8091c-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8091c-145">DateTimeOffset</span></span>|<span data-ttu-id="8091c-146">インテントレポートの最終更新日時</span><span class="sxs-lookup"><span data-stu-id="8091c-146">Last modified date time of an intent report</span></span>|
|<span data-ttu-id="8091c-147">state</span><span class="sxs-lookup"><span data-stu-id="8091c-147">state</span></span>|[<span data-ttu-id="8091c-148">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="8091c-148">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="8091c-149">目的のユーザー状態。</span><span class="sxs-lookup"><span data-stu-id="8091c-149">User state for an intent.</span></span> <span data-ttu-id="8091c-150">可能な値は、`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned` です。</span><span class="sxs-lookup"><span data-stu-id="8091c-150">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|



## <a name="response"></a><span data-ttu-id="8091c-151">応答</span><span class="sxs-lookup"><span data-stu-id="8091c-151">Response</span></span>
<span data-ttu-id="8091c-152">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[devicemanagementintentuserstate](../resources/intune-deviceintent-devicemanagementintentuserstate.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="8091c-152">If successful, this method returns a `200 OK` response code and an updated [deviceManagementIntentUserState](../resources/intune-deviceintent-devicemanagementintentuserstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8091c-153">例</span><span class="sxs-lookup"><span data-stu-id="8091c-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="8091c-154">要求</span><span class="sxs-lookup"><span data-stu-id="8091c-154">Request</span></span>
<span data-ttu-id="8091c-155">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="8091c-155">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/userStates/{deviceManagementIntentUserStateId}
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

### <a name="response"></a><span data-ttu-id="8091c-156">応答</span><span class="sxs-lookup"><span data-stu-id="8091c-156">Response</span></span>
<span data-ttu-id="8091c-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="8091c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





