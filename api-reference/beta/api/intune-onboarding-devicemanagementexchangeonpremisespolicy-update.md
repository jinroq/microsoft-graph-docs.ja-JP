---
title: DeviceManagementExchangeOnPremisesPolicy を更新します。
description: DeviceManagementExchangeOnPremisesPolicy オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 5cd001f6935836537fe06bd44af20ca9e6a6aa7b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27873970"
---
# <a name="update-devicemanagementexchangeonpremisespolicy"></a><span data-ttu-id="9fa62-103">DeviceManagementExchangeOnPremisesPolicy を更新します。</span><span class="sxs-lookup"><span data-stu-id="9fa62-103">Update deviceManagementExchangeOnPremisesPolicy</span></span>

> <span data-ttu-id="9fa62-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="9fa62-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9fa62-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9fa62-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9fa62-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="9fa62-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9fa62-107">[DeviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="9fa62-107">Update the properties of a [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9fa62-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="9fa62-108">Prerequisites</span></span>
<span data-ttu-id="9fa62-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9fa62-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9fa62-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9fa62-111">Permission type</span></span>|<span data-ttu-id="9fa62-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="9fa62-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9fa62-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9fa62-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9fa62-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9fa62-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="9fa62-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9fa62-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9fa62-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9fa62-116">Not supported.</span></span>|
|<span data-ttu-id="9fa62-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9fa62-117">Application</span></span>|<span data-ttu-id="9fa62-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9fa62-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9fa62-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9fa62-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/exchangeOnPremisesPolicy
PATCH /deviceManagement/exchangeOnPremisesPolicies/{deviceManagementExchangeOnPremisesPolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="9fa62-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9fa62-120">Request headers</span></span>
|<span data-ttu-id="9fa62-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9fa62-121">Header</span></span>|<span data-ttu-id="9fa62-122">値</span><span class="sxs-lookup"><span data-stu-id="9fa62-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9fa62-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9fa62-123">Authorization</span></span>|<span data-ttu-id="9fa62-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="9fa62-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9fa62-125">Accept</span><span class="sxs-lookup"><span data-stu-id="9fa62-125">Accept</span></span>|<span data-ttu-id="9fa62-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9fa62-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9fa62-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="9fa62-127">Request body</span></span>
<span data-ttu-id="9fa62-128">要求の本文に[deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="9fa62-128">In the request body, supply a JSON representation for the [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) object.</span></span>

<span data-ttu-id="9fa62-129">[DeviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="9fa62-129">The following table shows the properties that are required when you create the [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md).</span></span>

|<span data-ttu-id="9fa62-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9fa62-130">Property</span></span>|<span data-ttu-id="9fa62-131">種類</span><span class="sxs-lookup"><span data-stu-id="9fa62-131">Type</span></span>|<span data-ttu-id="9fa62-132">説明</span><span class="sxs-lookup"><span data-stu-id="9fa62-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9fa62-133">ID</span><span class="sxs-lookup"><span data-stu-id="9fa62-133">id</span></span>|<span data-ttu-id="9fa62-134">String</span><span class="sxs-lookup"><span data-stu-id="9fa62-134">String</span></span>|<span data-ttu-id="9fa62-135">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="9fa62-135">Not yet documented</span></span>|
|<span data-ttu-id="9fa62-136">notificationContent</span><span class="sxs-lookup"><span data-stu-id="9fa62-136">notificationContent</span></span>|<span data-ttu-id="9fa62-137">Binary</span><span class="sxs-lookup"><span data-stu-id="9fa62-137">Binary</span></span>|<span data-ttu-id="9fa62-138">このポリシーで検疫されたユーザーに送信される通知のテキストです。</span><span class="sxs-lookup"><span data-stu-id="9fa62-138">Notification text that will be sent to users quarantined by this policy.</span></span> <span data-ttu-id="9fa62-139">これは、UTF8 のエンコードされたバイト配列 HTML です。</span><span class="sxs-lookup"><span data-stu-id="9fa62-139">This is UTF8 encoded byte array HTML.</span></span>|
|<span data-ttu-id="9fa62-140">defaultAccessLevel</span><span class="sxs-lookup"><span data-stu-id="9fa62-140">defaultAccessLevel</span></span>|[<span data-ttu-id="9fa62-141">deviceManagementExchangeAccessLevel</span><span class="sxs-lookup"><span data-stu-id="9fa62-141">deviceManagementExchangeAccessLevel</span></span>](../resources/intune-onboarding-devicemanagementexchangeaccesslevel.md)|<span data-ttu-id="9fa62-142">Exchange の既定のアクセス状態。</span><span class="sxs-lookup"><span data-stu-id="9fa62-142">Default access state in Exchange.</span></span> <span data-ttu-id="9fa62-143">このルールは、Exchange 組織全体にグローバルに適用されます。</span><span class="sxs-lookup"><span data-stu-id="9fa62-143">This rule applies globally to the entire Exchange organization.</span></span> <span data-ttu-id="9fa62-144">可能な値は、`none`、`allow`、`block`、`quarantine` です。</span><span class="sxs-lookup"><span data-stu-id="9fa62-144">Possible values are: `none`, `allow`, `block`, `quarantine`.</span></span>|
|<span data-ttu-id="9fa62-145">accessRules</span><span class="sxs-lookup"><span data-stu-id="9fa62-145">accessRules</span></span>|<span data-ttu-id="9fa62-146">[deviceManagementExchangeAccessRule](../resources/intune-onboarding-devicemanagementexchangeaccessrule.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="9fa62-146">[deviceManagementExchangeAccessRule](../resources/intune-onboarding-devicemanagementexchangeaccessrule.md) collection</span></span>|<span data-ttu-id="9fa62-147">デバイスへのアクセスの一覧で Exchange ルールします。</span><span class="sxs-lookup"><span data-stu-id="9fa62-147">The list of device access rules in Exchange.</span></span> <span data-ttu-id="9fa62-148">アクセス ルールは、Exchange 組織全体にグローバルに適用します。</span><span class="sxs-lookup"><span data-stu-id="9fa62-148">The access rules apply globally to the entire Exchange organization</span></span>|
|<span data-ttu-id="9fa62-149">knownDeviceClasses</span><span class="sxs-lookup"><span data-stu-id="9fa62-149">knownDeviceClasses</span></span>|<span data-ttu-id="9fa62-150">[deviceManagementExchangeDeviceClass](../resources/intune-onboarding-devicemanagementexchangedeviceclass.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="9fa62-150">[deviceManagementExchangeDeviceClass](../resources/intune-onboarding-devicemanagementexchangedeviceclass.md) collection</span></span>|<span data-ttu-id="9fa62-151">Exchange に既知のデバイス クラスの一覧</span><span class="sxs-lookup"><span data-stu-id="9fa62-151">The list of device classes known to Exchange</span></span>|



## <a name="response"></a><span data-ttu-id="9fa62-152">応答</span><span class="sxs-lookup"><span data-stu-id="9fa62-152">Response</span></span>
<span data-ttu-id="9fa62-153">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="9fa62-153">If successful, this method returns a `200 OK` response code and an updated [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9fa62-154">例</span><span class="sxs-lookup"><span data-stu-id="9fa62-154">Example</span></span>
### <a name="request"></a><span data-ttu-id="9fa62-155">要求</span><span class="sxs-lookup"><span data-stu-id="9fa62-155">Request</span></span>
<span data-ttu-id="9fa62-156">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="9fa62-156">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/exchangeOnPremisesPolicy
Content-type: application/json
Content-length: 586

{
  "notificationContent": "bm90aWZpY2F0aW9uQ29udGVudA==",
  "defaultAccessLevel": "allow",
  "accessRules": [
    {
      "@odata.type": "microsoft.graph.deviceManagementExchangeAccessRule",
      "deviceClass": {
        "@odata.type": "microsoft.graph.deviceManagementExchangeDeviceClass",
        "name": "Name value",
        "type": "model"
      },
      "accessLevel": "allow"
    }
  ],
  "knownDeviceClasses": [
    {
      "@odata.type": "microsoft.graph.deviceManagementExchangeDeviceClass",
      "name": "Name value",
      "type": "model"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="9fa62-157">応答</span><span class="sxs-lookup"><span data-stu-id="9fa62-157">Response</span></span>
<span data-ttu-id="9fa62-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="9fa62-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 714

{
  "@odata.type": "#microsoft.graph.deviceManagementExchangeOnPremisesPolicy",
  "id": "16e76336-6336-16e7-3663-e7163663e716",
  "notificationContent": "bm90aWZpY2F0aW9uQ29udGVudA==",
  "defaultAccessLevel": "allow",
  "accessRules": [
    {
      "@odata.type": "microsoft.graph.deviceManagementExchangeAccessRule",
      "deviceClass": {
        "@odata.type": "microsoft.graph.deviceManagementExchangeDeviceClass",
        "name": "Name value",
        "type": "model"
      },
      "accessLevel": "allow"
    }
  ],
  "knownDeviceClasses": [
    {
      "@odata.type": "microsoft.graph.deviceManagementExchangeDeviceClass",
      "name": "Name value",
      "type": "model"
    }
  ]
}
```





