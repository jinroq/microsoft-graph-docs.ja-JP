---
title: DeviceManagementExchangeOnPremisesPolicy の更新
description: DeviceManagementExchangeOnPremisesPolicy オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 84813ed63976f298e2b768e96ea10b9f9cf6dec8
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33900111"
---
# <a name="update-devicemanagementexchangeonpremisespolicy"></a><span data-ttu-id="0a1bb-103">DeviceManagementExchangeOnPremisesPolicy の更新</span><span class="sxs-lookup"><span data-stu-id="0a1bb-103">Update deviceManagementExchangeOnPremisesPolicy</span></span>

> <span data-ttu-id="0a1bb-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0a1bb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0a1bb-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="0a1bb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0a1bb-106">[DeviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="0a1bb-106">Update the properties of a [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0a1bb-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="0a1bb-107">Prerequisites</span></span>
<span data-ttu-id="0a1bb-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0a1bb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0a1bb-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0a1bb-110">Permission type</span></span>|<span data-ttu-id="0a1bb-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="0a1bb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0a1bb-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0a1bb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0a1bb-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0a1bb-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="0a1bb-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0a1bb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0a1bb-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0a1bb-115">Not supported.</span></span>|
|<span data-ttu-id="0a1bb-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0a1bb-116">Application</span></span>|<span data-ttu-id="0a1bb-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0a1bb-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0a1bb-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0a1bb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/exchangeOnPremisesPolicy
PATCH /deviceManagement/exchangeOnPremisesPolicies/{deviceManagementExchangeOnPremisesPolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="0a1bb-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0a1bb-119">Request headers</span></span>
|<span data-ttu-id="0a1bb-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0a1bb-120">Header</span></span>|<span data-ttu-id="0a1bb-121">値</span><span class="sxs-lookup"><span data-stu-id="0a1bb-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0a1bb-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0a1bb-122">Authorization</span></span>|<span data-ttu-id="0a1bb-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="0a1bb-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0a1bb-124">承諾</span><span class="sxs-lookup"><span data-stu-id="0a1bb-124">Accept</span></span>|<span data-ttu-id="0a1bb-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0a1bb-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0a1bb-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="0a1bb-126">Request body</span></span>
<span data-ttu-id="0a1bb-127">要求本文で、 [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="0a1bb-127">In the request body, supply a JSON representation for the [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) object.</span></span>

<span data-ttu-id="0a1bb-128">次の表に、 [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="0a1bb-128">The following table shows the properties that are required when you create the [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md).</span></span>

|<span data-ttu-id="0a1bb-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0a1bb-129">Property</span></span>|<span data-ttu-id="0a1bb-130">型</span><span class="sxs-lookup"><span data-stu-id="0a1bb-130">Type</span></span>|<span data-ttu-id="0a1bb-131">説明</span><span class="sxs-lookup"><span data-stu-id="0a1bb-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0a1bb-132">id</span><span class="sxs-lookup"><span data-stu-id="0a1bb-132">id</span></span>|<span data-ttu-id="0a1bb-133">String</span><span class="sxs-lookup"><span data-stu-id="0a1bb-133">String</span></span>|<span data-ttu-id="0a1bb-134">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="0a1bb-134">Not yet documented</span></span>|
|<span data-ttu-id="0a1bb-135">notificationContent</span><span class="sxs-lookup"><span data-stu-id="0a1bb-135">notificationContent</span></span>|<span data-ttu-id="0a1bb-136">Binary</span><span class="sxs-lookup"><span data-stu-id="0a1bb-136">Binary</span></span>|<span data-ttu-id="0a1bb-137">このポリシーによって検疫されたユーザーに送信される通知テキスト。</span><span class="sxs-lookup"><span data-stu-id="0a1bb-137">Notification text that will be sent to users quarantined by this policy.</span></span> <span data-ttu-id="0a1bb-138">これは、UTF8 でエンコードされたバイト配列 HTML です。</span><span class="sxs-lookup"><span data-stu-id="0a1bb-138">This is UTF8 encoded byte array HTML.</span></span>|
|<span data-ttu-id="0a1bb-139">defaultAccessLevel</span><span class="sxs-lookup"><span data-stu-id="0a1bb-139">defaultAccessLevel</span></span>|[<span data-ttu-id="0a1bb-140">deviceManagementExchangeAccessLevel</span><span class="sxs-lookup"><span data-stu-id="0a1bb-140">deviceManagementExchangeAccessLevel</span></span>](../resources/intune-onboarding-devicemanagementexchangeaccesslevel.md)|<span data-ttu-id="0a1bb-141">Exchange の既定のアクセス状態。</span><span class="sxs-lookup"><span data-stu-id="0a1bb-141">Default access state in Exchange.</span></span> <span data-ttu-id="0a1bb-142">このルールは、Exchange 組織全体にグローバルに適用されます。</span><span class="sxs-lookup"><span data-stu-id="0a1bb-142">This rule applies globally to the entire Exchange organization.</span></span> <span data-ttu-id="0a1bb-143">使用可能な値は、`none`、`allow`、`block`、`quarantine` です。</span><span class="sxs-lookup"><span data-stu-id="0a1bb-143">Possible values are: `none`, `allow`, `block`, `quarantine`.</span></span>|
|<span data-ttu-id="0a1bb-144">accessRules</span><span class="sxs-lookup"><span data-stu-id="0a1bb-144">accessRules</span></span>|<span data-ttu-id="0a1bb-145">[Devicemanagementexchangeaccessrule](../resources/intune-onboarding-devicemanagementexchangeaccessrule.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="0a1bb-145">[deviceManagementExchangeAccessRule](../resources/intune-onboarding-devicemanagementexchangeaccessrule.md) collection</span></span>|<span data-ttu-id="0a1bb-146">Exchange のデバイスアクセスルールの一覧。</span><span class="sxs-lookup"><span data-stu-id="0a1bb-146">The list of device access rules in Exchange.</span></span> <span data-ttu-id="0a1bb-147">アクセスルールは、Exchange 組織全体にグローバルに適用されます。</span><span class="sxs-lookup"><span data-stu-id="0a1bb-147">The access rules apply globally to the entire Exchange organization</span></span>|
|<span data-ttu-id="0a1bb-148">knownDeviceClasses 場合</span><span class="sxs-lookup"><span data-stu-id="0a1bb-148">knownDeviceClasses</span></span>|<span data-ttu-id="0a1bb-149">[Devicemanagementexchangedeviceclass](../resources/intune-onboarding-devicemanagementexchangedeviceclass.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="0a1bb-149">[deviceManagementExchangeDeviceClass](../resources/intune-onboarding-devicemanagementexchangedeviceclass.md) collection</span></span>|<span data-ttu-id="0a1bb-150">Exchange に認識されているデバイスクラスの一覧</span><span class="sxs-lookup"><span data-stu-id="0a1bb-150">The list of device classes known to Exchange</span></span>|



## <a name="response"></a><span data-ttu-id="0a1bb-151">応答</span><span class="sxs-lookup"><span data-stu-id="0a1bb-151">Response</span></span>
<span data-ttu-id="0a1bb-152">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="0a1bb-152">If successful, this method returns a `200 OK` response code and an updated [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0a1bb-153">例</span><span class="sxs-lookup"><span data-stu-id="0a1bb-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="0a1bb-154">要求</span><span class="sxs-lookup"><span data-stu-id="0a1bb-154">Request</span></span>
<span data-ttu-id="0a1bb-155">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="0a1bb-155">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/exchangeOnPremisesPolicy
Content-type: application/json
Content-length: 665

{
  "@odata.type": "#microsoft.graph.deviceManagementExchangeOnPremisesPolicy",
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

### <a name="response"></a><span data-ttu-id="0a1bb-156">応答</span><span class="sxs-lookup"><span data-stu-id="0a1bb-156">Response</span></span>
<span data-ttu-id="0a1bb-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="0a1bb-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




