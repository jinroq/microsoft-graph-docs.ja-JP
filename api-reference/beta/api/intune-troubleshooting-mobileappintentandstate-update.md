---
title: MobileAppIntentAndState の更新
description: MobileAppIntentAndState オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 75a254632c09234b6ab4fd4045bac307797e5b16
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35993340"
---
# <a name="update-mobileappintentandstate"></a><span data-ttu-id="beb03-103">MobileAppIntentAndState の更新</span><span class="sxs-lookup"><span data-stu-id="beb03-103">Update mobileAppIntentAndState</span></span>

> <span data-ttu-id="beb03-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="beb03-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="beb03-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="beb03-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="beb03-106">[MobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="beb03-106">Update the properties of a [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="beb03-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="beb03-107">Prerequisites</span></span>
<span data-ttu-id="beb03-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="beb03-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="beb03-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="beb03-110">Permission type</span></span>|<span data-ttu-id="beb03-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="beb03-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="beb03-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="beb03-112">Delegated (work or school account)</span></span>|<span data-ttu-id="beb03-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="beb03-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="beb03-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="beb03-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="beb03-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="beb03-115">Not supported.</span></span>|
|<span data-ttu-id="beb03-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="beb03-116">Application</span></span>|<span data-ttu-id="beb03-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="beb03-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="beb03-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="beb03-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /users/{usersId}/mobileAppIntentAndStates/{mobileAppIntentAndStateId}
```

## <a name="request-headers"></a><span data-ttu-id="beb03-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="beb03-119">Request headers</span></span>
|<span data-ttu-id="beb03-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="beb03-120">Header</span></span>|<span data-ttu-id="beb03-121">値</span><span class="sxs-lookup"><span data-stu-id="beb03-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="beb03-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="beb03-122">Authorization</span></span>|<span data-ttu-id="beb03-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="beb03-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="beb03-124">承諾</span><span class="sxs-lookup"><span data-stu-id="beb03-124">Accept</span></span>|<span data-ttu-id="beb03-125">application/json</span><span class="sxs-lookup"><span data-stu-id="beb03-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="beb03-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="beb03-126">Request body</span></span>
<span data-ttu-id="beb03-127">要求本文で、 [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="beb03-127">In the request body, supply a JSON representation for the [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) object.</span></span>

<span data-ttu-id="beb03-128">次の表に、 [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="beb03-128">The following table shows the properties that are required when you create the [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md).</span></span>

|<span data-ttu-id="beb03-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="beb03-129">Property</span></span>|<span data-ttu-id="beb03-130">型</span><span class="sxs-lookup"><span data-stu-id="beb03-130">Type</span></span>|<span data-ttu-id="beb03-131">説明</span><span class="sxs-lookup"><span data-stu-id="beb03-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="beb03-132">id</span><span class="sxs-lookup"><span data-stu-id="beb03-132">id</span></span>|<span data-ttu-id="beb03-133">文字列</span><span class="sxs-lookup"><span data-stu-id="beb03-133">String</span></span>|<span data-ttu-id="beb03-134">オブジェクトの UUID</span><span class="sxs-lookup"><span data-stu-id="beb03-134">UUID for the object</span></span>|
|<span data-ttu-id="beb03-135">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="beb03-135">managedDeviceIdentifier</span></span>|<span data-ttu-id="beb03-136">String</span><span class="sxs-lookup"><span data-stu-id="beb03-136">String</span></span>|<span data-ttu-id="beb03-137">Intune によって作成または収集されるデバイス識別子。</span><span class="sxs-lookup"><span data-stu-id="beb03-137">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="beb03-138">userId</span><span class="sxs-lookup"><span data-stu-id="beb03-138">userId</span></span>|<span data-ttu-id="beb03-139">String</span><span class="sxs-lookup"><span data-stu-id="beb03-139">String</span></span>|<span data-ttu-id="beb03-140">デバイスを登録しようとするユーザーの識別子。</span><span class="sxs-lookup"><span data-stu-id="beb03-140">Identifier for the user that tried to enroll the device.</span></span>|
|<span data-ttu-id="beb03-141">mobileAppList</span><span class="sxs-lookup"><span data-stu-id="beb03-141">mobileAppList</span></span>|<span data-ttu-id="beb03-142">[mobileAppIntentAndStateDetail](../resources/intune-troubleshooting-mobileappintentandstatedetail.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="beb03-142">[mobileAppIntentAndStateDetail](../resources/intune-troubleshooting-mobileappintentandstatedetail.md) collection</span></span>|<span data-ttu-id="beb03-143">テナントのペイロードの意図と状態の一覧。</span><span class="sxs-lookup"><span data-stu-id="beb03-143">The list of payload intents and states for the tenant.</span></span>|



## <a name="response"></a><span data-ttu-id="beb03-144">応答</span><span class="sxs-lookup"><span data-stu-id="beb03-144">Response</span></span>
<span data-ttu-id="beb03-145">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="beb03-145">If successful, this method returns a `200 OK` response code and an updated [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="beb03-146">例</span><span class="sxs-lookup"><span data-stu-id="beb03-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="beb03-147">要求</span><span class="sxs-lookup"><span data-stu-id="beb03-147">Request</span></span>
<span data-ttu-id="beb03-148">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="beb03-148">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/users/{usersId}/mobileAppIntentAndStates/{mobileAppIntentAndStateId}
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

### <a name="response"></a><span data-ttu-id="beb03-149">応答</span><span class="sxs-lookup"><span data-stu-id="beb03-149">Response</span></span>
<span data-ttu-id="beb03-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="beb03-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





