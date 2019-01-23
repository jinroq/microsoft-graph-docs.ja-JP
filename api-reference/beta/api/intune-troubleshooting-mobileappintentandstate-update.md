---
title: MobileAppIntentAndState を更新します。
description: MobileAppIntentAndState オブジェクトのプロパティを更新します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 7157711819e4a5b3d4fbeb6ea6c8fce136da9380
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29405192"
---
# <a name="update-mobileappintentandstate"></a><span data-ttu-id="3d595-103">MobileAppIntentAndState を更新します。</span><span class="sxs-lookup"><span data-stu-id="3d595-103">Update mobileAppIntentAndState</span></span>

> <span data-ttu-id="3d595-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="3d595-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="3d595-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3d595-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3d595-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="3d595-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3d595-107">[MobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="3d595-107">Update the properties of a [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3d595-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="3d595-108">Prerequisites</span></span>
<span data-ttu-id="3d595-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3d595-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="3d595-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3d595-111">Permission type</span></span>|<span data-ttu-id="3d595-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="3d595-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3d595-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3d595-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3d595-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3d595-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="3d595-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3d595-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3d595-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3d595-116">Not supported.</span></span>|
|<span data-ttu-id="3d595-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3d595-117">Application</span></span>|<span data-ttu-id="3d595-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3d595-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3d595-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3d595-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /users/{usersId}/mobileAppIntentAndStates/{mobileAppIntentAndStateId}
```

## <a name="request-headers"></a><span data-ttu-id="3d595-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3d595-120">Request headers</span></span>
|<span data-ttu-id="3d595-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3d595-121">Header</span></span>|<span data-ttu-id="3d595-122">値</span><span class="sxs-lookup"><span data-stu-id="3d595-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3d595-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3d595-123">Authorization</span></span>|<span data-ttu-id="3d595-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="3d595-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3d595-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3d595-125">Accept</span></span>|<span data-ttu-id="3d595-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3d595-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3d595-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="3d595-127">Request body</span></span>
<span data-ttu-id="3d595-128">要求の本文に[mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="3d595-128">In the request body, supply a JSON representation for the [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) object.</span></span>

<span data-ttu-id="3d595-129">[MobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="3d595-129">The following table shows the properties that are required when you create the [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md).</span></span>

|<span data-ttu-id="3d595-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3d595-130">Property</span></span>|<span data-ttu-id="3d595-131">型</span><span class="sxs-lookup"><span data-stu-id="3d595-131">Type</span></span>|<span data-ttu-id="3d595-132">説明</span><span class="sxs-lookup"><span data-stu-id="3d595-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3d595-133">id</span><span class="sxs-lookup"><span data-stu-id="3d595-133">id</span></span>|<span data-ttu-id="3d595-134">String</span><span class="sxs-lookup"><span data-stu-id="3d595-134">String</span></span>|<span data-ttu-id="3d595-135">オブジェクトの UUID</span><span class="sxs-lookup"><span data-stu-id="3d595-135">UUID for the object</span></span>|
|<span data-ttu-id="3d595-136">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="3d595-136">managedDeviceIdentifier</span></span>|<span data-ttu-id="3d595-137">String</span><span class="sxs-lookup"><span data-stu-id="3d595-137">String</span></span>|<span data-ttu-id="3d595-138">Intune によって作成または収集されるデバイス識別子。</span><span class="sxs-lookup"><span data-stu-id="3d595-138">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="3d595-139">userId</span><span class="sxs-lookup"><span data-stu-id="3d595-139">userId</span></span>|<span data-ttu-id="3d595-140">String</span><span class="sxs-lookup"><span data-stu-id="3d595-140">String</span></span>|<span data-ttu-id="3d595-141">デバイスを登録しようとするユーザーの識別子。</span><span class="sxs-lookup"><span data-stu-id="3d595-141">Identifier for the user that tried to enroll the device.</span></span>|
|<span data-ttu-id="3d595-142">mobileAppList</span><span class="sxs-lookup"><span data-stu-id="3d595-142">mobileAppList</span></span>|<span data-ttu-id="3d595-143">[mobileAppIntentAndStateDetail](../resources/intune-troubleshooting-mobileappintentandstatedetail.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="3d595-143">[mobileAppIntentAndStateDetail](../resources/intune-troubleshooting-mobileappintentandstatedetail.md) collection</span></span>|<span data-ttu-id="3d595-144">ペイロードの目的と、テナントの状態の一覧です。</span><span class="sxs-lookup"><span data-stu-id="3d595-144">The list of payload intents and states for the tenant.</span></span>|



## <a name="response"></a><span data-ttu-id="3d595-145">応答</span><span class="sxs-lookup"><span data-stu-id="3d595-145">Response</span></span>
<span data-ttu-id="3d595-146">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="3d595-146">If successful, this method returns a `200 OK` response code and an updated [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3d595-147">例</span><span class="sxs-lookup"><span data-stu-id="3d595-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="3d595-148">要求</span><span class="sxs-lookup"><span data-stu-id="3d595-148">Request</span></span>
<span data-ttu-id="3d595-149">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="3d595-149">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="3d595-150">応答</span><span class="sxs-lookup"><span data-stu-id="3d595-150">Response</span></span>
<span data-ttu-id="3d595-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="3d595-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




