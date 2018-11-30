---
title: MobileAppIntentAndState を更新します。
description: MobileAppIntentAndState オブジェクトのプロパティを更新します。
ms.openlocfilehash: 36bbfa2ea41f68b84ae711204fcbdafb3c309aa2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27070016"
---
# <a name="update-mobileappintentandstate"></a><span data-ttu-id="c419d-103">MobileAppIntentAndState を更新します。</span><span class="sxs-lookup"><span data-stu-id="c419d-103">Update mobileAppIntentAndState</span></span>

> <span data-ttu-id="c419d-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c419d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c419d-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c419d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c419d-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="c419d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c419d-107">[MobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="c419d-107">Update the properties of a [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c419d-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="c419d-108">Prerequisites</span></span>
<span data-ttu-id="c419d-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c419d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c419d-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c419d-111">Permission type</span></span>|<span data-ttu-id="c419d-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="c419d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c419d-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c419d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c419d-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c419d-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="c419d-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c419d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c419d-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c419d-116">Not supported.</span></span>|
|<span data-ttu-id="c419d-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c419d-117">Application</span></span>|<span data-ttu-id="c419d-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c419d-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c419d-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c419d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /users/{usersId}/mobileAppIntentAndStates/{mobileAppIntentAndStateId}
```

## <a name="request-headers"></a><span data-ttu-id="c419d-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c419d-120">Request headers</span></span>
|<span data-ttu-id="c419d-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c419d-121">Header</span></span>|<span data-ttu-id="c419d-122">値</span><span class="sxs-lookup"><span data-stu-id="c419d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c419d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c419d-123">Authorization</span></span>|<span data-ttu-id="c419d-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="c419d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c419d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c419d-125">Accept</span></span>|<span data-ttu-id="c419d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c419d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c419d-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="c419d-127">Request body</span></span>
<span data-ttu-id="c419d-128">要求の本文に[mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="c419d-128">In the request body, supply a JSON representation for the [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) object.</span></span>

<span data-ttu-id="c419d-129">[MobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="c419d-129">The following table shows the properties that are required when you create the [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md).</span></span>

|<span data-ttu-id="c419d-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c419d-130">Property</span></span>|<span data-ttu-id="c419d-131">型</span><span class="sxs-lookup"><span data-stu-id="c419d-131">Type</span></span>|<span data-ttu-id="c419d-132">説明</span><span class="sxs-lookup"><span data-stu-id="c419d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c419d-133">id</span><span class="sxs-lookup"><span data-stu-id="c419d-133">id</span></span>|<span data-ttu-id="c419d-134">String</span><span class="sxs-lookup"><span data-stu-id="c419d-134">String</span></span>|<span data-ttu-id="c419d-135">オブジェクトの UUID</span><span class="sxs-lookup"><span data-stu-id="c419d-135">UUID for the object</span></span>|
|<span data-ttu-id="c419d-136">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="c419d-136">managedDeviceIdentifier</span></span>|<span data-ttu-id="c419d-137">String</span><span class="sxs-lookup"><span data-stu-id="c419d-137">String</span></span>|<span data-ttu-id="c419d-138">Intune によって作成または収集されるデバイス識別子。</span><span class="sxs-lookup"><span data-stu-id="c419d-138">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="c419d-139">userId</span><span class="sxs-lookup"><span data-stu-id="c419d-139">userId</span></span>|<span data-ttu-id="c419d-140">String</span><span class="sxs-lookup"><span data-stu-id="c419d-140">String</span></span>|<span data-ttu-id="c419d-141">デバイスを登録しようとするユーザーの識別子。</span><span class="sxs-lookup"><span data-stu-id="c419d-141">Identifier for the user that tried to enroll the device.</span></span>|
|<span data-ttu-id="c419d-142">mobileAppList</span><span class="sxs-lookup"><span data-stu-id="c419d-142">mobileAppList</span></span>|<span data-ttu-id="c419d-143">[mobileAppIntentAndStateDetail](../resources/intune-troubleshooting-mobileappintentandstatedetail.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="c419d-143">[mobileAppIntentAndStateDetail](../resources/intune-troubleshooting-mobileappintentandstatedetail.md) collection</span></span>|<span data-ttu-id="c419d-144">ペイロードの目的と、テナントの状態の一覧です。</span><span class="sxs-lookup"><span data-stu-id="c419d-144">The list of payload intents and states for the tenant.</span></span>|



## <a name="response"></a><span data-ttu-id="c419d-145">応答</span><span class="sxs-lookup"><span data-stu-id="c419d-145">Response</span></span>
<span data-ttu-id="c419d-146">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="c419d-146">If successful, this method returns a `200 OK` response code and an updated [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c419d-147">例</span><span class="sxs-lookup"><span data-stu-id="c419d-147">Example</span></span>
### <a name="request"></a><span data-ttu-id="c419d-148">要求</span><span class="sxs-lookup"><span data-stu-id="c419d-148">Request</span></span>
<span data-ttu-id="c419d-149">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c419d-149">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/users/{usersId}/mobileAppIntentAndStates/{mobileAppIntentAndStateId}
Content-type: application/json
Content-length: 769

{
  "managedDeviceIdentifier": "Managed Device Identifier value",
  "userId": "User Id value",
  "mobileAppList": [
    {
      "@odata.type": "microsoft.graph.mobileAppIntentAndStateDetail",
      "applicationId": "Application Id value",
      "displayName": "Display Name value",
      "mobileAppIntent": "notAvailable",
      "displayVersion": "Display Version value",
      "installState": "failed",
      "supportedDeviceTypes": [
        {
          "@odata.type": "microsoft.graph.mobileAppSupportedDeviceType",
          "type": "windowsRT",
          "minimumOperatingSystemVersion": "Minimum Operating System Version value",
          "maximumOperatingSystemVersion": "Maximum Operating System Version value"
        }
      ]
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="c419d-150">応答</span><span class="sxs-lookup"><span data-stu-id="c419d-150">Response</span></span>
<span data-ttu-id="c419d-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="c419d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 880

{
  "@odata.type": "#microsoft.graph.mobileAppIntentAndState",
  "id": "45a775d6-75d6-45a7-d675-a745d675a745",
  "managedDeviceIdentifier": "Managed Device Identifier value",
  "userId": "User Id value",
  "mobileAppList": [
    {
      "@odata.type": "microsoft.graph.mobileAppIntentAndStateDetail",
      "applicationId": "Application Id value",
      "displayName": "Display Name value",
      "mobileAppIntent": "notAvailable",
      "displayVersion": "Display Version value",
      "installState": "failed",
      "supportedDeviceTypes": [
        {
          "@odata.type": "microsoft.graph.mobileAppSupportedDeviceType",
          "type": "windowsRT",
          "minimumOperatingSystemVersion": "Minimum Operating System Version value",
          "maximumOperatingSystemVersion": "Maximum Operating System Version value"
        }
      ]
    }
  ]
}
```





