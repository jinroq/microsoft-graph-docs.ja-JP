---
title: deviceManagementExchangeOnPremisesPolicy の更新
description: deviceManagementExchangeOnPremisesPolicy オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a94f22aa4d7dffcd448ad5e742198ddca809d781
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30168027"
---
# <a name="update-devicemanagementexchangeonpremisespolicy"></a><span data-ttu-id="16def-103">deviceManagementExchangeOnPremisesPolicy の更新</span><span class="sxs-lookup"><span data-stu-id="16def-103">Update deviceManagementExchangeOnPremisesPolicy</span></span>

> <span data-ttu-id="16def-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="16def-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="16def-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="16def-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="16def-106">[deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="16def-106">Update the properties of a [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="16def-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="16def-107">Prerequisites</span></span>
<span data-ttu-id="16def-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="16def-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="16def-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="16def-110">Permission type</span></span>|<span data-ttu-id="16def-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="16def-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="16def-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="16def-112">Delegated (work or school account)</span></span>|<span data-ttu-id="16def-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="16def-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="16def-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="16def-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="16def-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="16def-115">Not supported.</span></span>|
|<span data-ttu-id="16def-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="16def-116">Application</span></span>|<span data-ttu-id="16def-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="16def-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="16def-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="16def-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/exchangeOnPremisesPolicy
PATCH /deviceManagement/exchangeOnPremisesPolicies/{deviceManagementExchangeOnPremisesPolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="16def-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="16def-119">Request headers</span></span>
|<span data-ttu-id="16def-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="16def-120">Header</span></span>|<span data-ttu-id="16def-121">値</span><span class="sxs-lookup"><span data-stu-id="16def-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="16def-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="16def-122">Authorization</span></span>|<span data-ttu-id="16def-123">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="16def-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="16def-124">承諾</span><span class="sxs-lookup"><span data-stu-id="16def-124">Accept</span></span>|<span data-ttu-id="16def-125">application/json</span><span class="sxs-lookup"><span data-stu-id="16def-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="16def-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="16def-126">Request body</span></span>
<span data-ttu-id="16def-127">要求本文で、 [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="16def-127">In the request body, supply a JSON representation for the [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) object.</span></span>

<span data-ttu-id="16def-128">次の表に、 [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="16def-128">The following table shows the properties that are required when you create the [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md).</span></span>

|<span data-ttu-id="16def-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="16def-129">Property</span></span>|<span data-ttu-id="16def-130">型</span><span class="sxs-lookup"><span data-stu-id="16def-130">Type</span></span>|<span data-ttu-id="16def-131">説明</span><span class="sxs-lookup"><span data-stu-id="16def-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="16def-132">id</span><span class="sxs-lookup"><span data-stu-id="16def-132">id</span></span>|<span data-ttu-id="16def-133">String</span><span class="sxs-lookup"><span data-stu-id="16def-133">String</span></span>|<span data-ttu-id="16def-134">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="16def-134">Not yet documented</span></span>|
|<span data-ttu-id="16def-135">notificationContent</span><span class="sxs-lookup"><span data-stu-id="16def-135">notificationContent</span></span>|<span data-ttu-id="16def-136">Binary</span><span class="sxs-lookup"><span data-stu-id="16def-136">Binary</span></span>|<span data-ttu-id="16def-137">このポリシーによって検疫されたユーザーに送信される通知テキスト。</span><span class="sxs-lookup"><span data-stu-id="16def-137">Notification text that will be sent to users quarantined by this policy.</span></span> <span data-ttu-id="16def-138">これは、UTF8 でエンコードされたバイト配列 HTML です。</span><span class="sxs-lookup"><span data-stu-id="16def-138">This is UTF8 encoded byte array HTML.</span></span>|
|<span data-ttu-id="16def-139">defaultaccesslevel</span><span class="sxs-lookup"><span data-stu-id="16def-139">defaultAccessLevel</span></span>|[<span data-ttu-id="16def-140">devicemanagementexchangeaccesslevel</span><span class="sxs-lookup"><span data-stu-id="16def-140">deviceManagementExchangeAccessLevel</span></span>](../resources/intune-onboarding-devicemanagementexchangeaccesslevel.md)|<span data-ttu-id="16def-141">Exchange の既定のアクセス状態。</span><span class="sxs-lookup"><span data-stu-id="16def-141">Default access state in Exchange.</span></span> <span data-ttu-id="16def-142">このルールは、Exchange 組織全体にグローバルに適用されます。</span><span class="sxs-lookup"><span data-stu-id="16def-142">This rule applies globally to the entire Exchange organization.</span></span> <span data-ttu-id="16def-143">使用可能な値は、`none`、`allow`、`block`、`quarantine` です。</span><span class="sxs-lookup"><span data-stu-id="16def-143">Possible values are: `none`, `allow`, `block`, `quarantine`.</span></span>|
|<span data-ttu-id="16def-144">accessrules</span><span class="sxs-lookup"><span data-stu-id="16def-144">accessRules</span></span>|<span data-ttu-id="16def-145">[devicemanagementexchangeaccessrule](../resources/intune-onboarding-devicemanagementexchangeaccessrule.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="16def-145">[deviceManagementExchangeAccessRule](../resources/intune-onboarding-devicemanagementexchangeaccessrule.md) collection</span></span>|<span data-ttu-id="16def-146">Exchange のデバイスアクセスルールの一覧。</span><span class="sxs-lookup"><span data-stu-id="16def-146">The list of device access rules in Exchange.</span></span> <span data-ttu-id="16def-147">アクセスルールは、Exchange 組織全体にグローバルに適用されます。</span><span class="sxs-lookup"><span data-stu-id="16def-147">The access rules apply globally to the entire Exchange organization</span></span>|
|<span data-ttu-id="16def-148">knowndeviceclasses 場合</span><span class="sxs-lookup"><span data-stu-id="16def-148">knownDeviceClasses</span></span>|<span data-ttu-id="16def-149">[devicemanagementexchangedeviceclass](../resources/intune-onboarding-devicemanagementexchangedeviceclass.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="16def-149">[deviceManagementExchangeDeviceClass](../resources/intune-onboarding-devicemanagementexchangedeviceclass.md) collection</span></span>|<span data-ttu-id="16def-150">Exchange に認識されているデバイスクラスの一覧</span><span class="sxs-lookup"><span data-stu-id="16def-150">The list of device classes known to Exchange</span></span>|



## <a name="response"></a><span data-ttu-id="16def-151">応答</span><span class="sxs-lookup"><span data-stu-id="16def-151">Response</span></span>
<span data-ttu-id="16def-152">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="16def-152">If successful, this method returns a `200 OK` response code and an updated [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="16def-153">例</span><span class="sxs-lookup"><span data-stu-id="16def-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="16def-154">要求</span><span class="sxs-lookup"><span data-stu-id="16def-154">Request</span></span>
<span data-ttu-id="16def-155">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="16def-155">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="16def-156">応答</span><span class="sxs-lookup"><span data-stu-id="16def-156">Response</span></span>
<span data-ttu-id="16def-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="16def-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




