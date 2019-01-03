---
title: MobileAppIntentAndState を作成します。
description: 新しい mobileAppIntentAndState オブジェクトを作成します。
author: tfitzmac
ms.openlocfilehash: 590cbb01e8b1f41ce1a1c43be7c3a97872ea737a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27308702"
---
# <a name="create-mobileappintentandstate"></a><span data-ttu-id="6cc10-103">MobileAppIntentAndState を作成します。</span><span class="sxs-lookup"><span data-stu-id="6cc10-103">Create mobileAppIntentAndState</span></span>

> <span data-ttu-id="6cc10-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="6cc10-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6cc10-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6cc10-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6cc10-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="6cc10-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6cc10-107">新しい[mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="6cc10-107">Create a new [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6cc10-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="6cc10-108">Prerequisites</span></span>
<span data-ttu-id="6cc10-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6cc10-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6cc10-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6cc10-111">Permission type</span></span>|<span data-ttu-id="6cc10-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="6cc10-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6cc10-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6cc10-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6cc10-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6cc10-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="6cc10-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6cc10-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6cc10-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6cc10-116">Not supported.</span></span>|
|<span data-ttu-id="6cc10-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6cc10-117">Application</span></span>|<span data-ttu-id="6cc10-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6cc10-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6cc10-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6cc10-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/mobileAppIntentAndStates
```

## <a name="request-headers"></a><span data-ttu-id="6cc10-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6cc10-120">Request headers</span></span>
|<span data-ttu-id="6cc10-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6cc10-121">Header</span></span>|<span data-ttu-id="6cc10-122">値</span><span class="sxs-lookup"><span data-stu-id="6cc10-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6cc10-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6cc10-123">Authorization</span></span>|<span data-ttu-id="6cc10-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="6cc10-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6cc10-125">Accept</span><span class="sxs-lookup"><span data-stu-id="6cc10-125">Accept</span></span>|<span data-ttu-id="6cc10-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6cc10-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6cc10-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="6cc10-127">Request body</span></span>
<span data-ttu-id="6cc10-128">要求の本文に mobileAppIntentAndState オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="6cc10-128">In the request body, supply a JSON representation for the mobileAppIntentAndState object.</span></span>

<span data-ttu-id="6cc10-129">次の表は、mobileAppIntentAndState を作成するときに必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="6cc10-129">The following table shows the properties that are required when you create the mobileAppIntentAndState.</span></span>

|<span data-ttu-id="6cc10-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6cc10-130">Property</span></span>|<span data-ttu-id="6cc10-131">種類</span><span class="sxs-lookup"><span data-stu-id="6cc10-131">Type</span></span>|<span data-ttu-id="6cc10-132">説明</span><span class="sxs-lookup"><span data-stu-id="6cc10-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6cc10-133">ID</span><span class="sxs-lookup"><span data-stu-id="6cc10-133">id</span></span>|<span data-ttu-id="6cc10-134">String</span><span class="sxs-lookup"><span data-stu-id="6cc10-134">String</span></span>|<span data-ttu-id="6cc10-135">オブジェクトの UUID</span><span class="sxs-lookup"><span data-stu-id="6cc10-135">UUID for the object</span></span>|
|<span data-ttu-id="6cc10-136">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="6cc10-136">managedDeviceIdentifier</span></span>|<span data-ttu-id="6cc10-137">String</span><span class="sxs-lookup"><span data-stu-id="6cc10-137">String</span></span>|<span data-ttu-id="6cc10-138">Intune によって作成または収集されるデバイス識別子。</span><span class="sxs-lookup"><span data-stu-id="6cc10-138">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="6cc10-139">userId</span><span class="sxs-lookup"><span data-stu-id="6cc10-139">userId</span></span>|<span data-ttu-id="6cc10-140">String</span><span class="sxs-lookup"><span data-stu-id="6cc10-140">String</span></span>|<span data-ttu-id="6cc10-141">デバイスを登録しようとするユーザーの識別子。</span><span class="sxs-lookup"><span data-stu-id="6cc10-141">Identifier for the user that tried to enroll the device.</span></span>|
|<span data-ttu-id="6cc10-142">mobileAppList</span><span class="sxs-lookup"><span data-stu-id="6cc10-142">mobileAppList</span></span>|<span data-ttu-id="6cc10-143">[mobileAppIntentAndStateDetail](../resources/intune-troubleshooting-mobileappintentandstatedetail.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="6cc10-143">[mobileAppIntentAndStateDetail](../resources/intune-troubleshooting-mobileappintentandstatedetail.md) collection</span></span>|<span data-ttu-id="6cc10-144">ペイロードの目的と、テナントの状態の一覧です。</span><span class="sxs-lookup"><span data-stu-id="6cc10-144">The list of payload intents and states for the tenant.</span></span>|



## <a name="response"></a><span data-ttu-id="6cc10-145">応答</span><span class="sxs-lookup"><span data-stu-id="6cc10-145">Response</span></span>
<span data-ttu-id="6cc10-146">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="6cc10-146">If successful, this method returns a `201 Created` response code and a [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6cc10-147">例</span><span class="sxs-lookup"><span data-stu-id="6cc10-147">Example</span></span>
### <a name="request"></a><span data-ttu-id="6cc10-148">要求</span><span class="sxs-lookup"><span data-stu-id="6cc10-148">Request</span></span>
<span data-ttu-id="6cc10-149">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="6cc10-149">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/users/{usersId}/mobileAppIntentAndStates
Content-type: application/json
Content-length: 831

{
  "@odata.type": "#microsoft.graph.mobileAppIntentAndState",
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

### <a name="response"></a><span data-ttu-id="6cc10-150">応答</span><span class="sxs-lookup"><span data-stu-id="6cc10-150">Response</span></span>
<span data-ttu-id="6cc10-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="6cc10-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




