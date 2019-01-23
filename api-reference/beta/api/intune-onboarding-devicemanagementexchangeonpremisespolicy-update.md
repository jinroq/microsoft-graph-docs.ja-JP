---
title: DeviceManagementExchangeOnPremisesPolicy を更新します。
description: DeviceManagementExchangeOnPremisesPolicy オブジェクトのプロパティを更新します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 633f1b80895bd84c27c57b5cee26aa286b1d0e49
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29407208"
---
# <a name="update-devicemanagementexchangeonpremisespolicy"></a><span data-ttu-id="a6b86-103">DeviceManagementExchangeOnPremisesPolicy を更新します。</span><span class="sxs-lookup"><span data-stu-id="a6b86-103">Update deviceManagementExchangeOnPremisesPolicy</span></span>

> <span data-ttu-id="a6b86-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="a6b86-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="a6b86-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a6b86-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a6b86-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="a6b86-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a6b86-107">[DeviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="a6b86-107">Update the properties of a [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a6b86-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="a6b86-108">Prerequisites</span></span>
<span data-ttu-id="a6b86-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a6b86-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="a6b86-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a6b86-111">Permission type</span></span>|<span data-ttu-id="a6b86-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="a6b86-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a6b86-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a6b86-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a6b86-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a6b86-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="a6b86-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a6b86-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a6b86-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a6b86-116">Not supported.</span></span>|
|<span data-ttu-id="a6b86-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a6b86-117">Application</span></span>|<span data-ttu-id="a6b86-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a6b86-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a6b86-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a6b86-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/exchangeOnPremisesPolicy
PATCH /deviceManagement/exchangeOnPremisesPolicies/{deviceManagementExchangeOnPremisesPolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="a6b86-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a6b86-120">Request headers</span></span>
|<span data-ttu-id="a6b86-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a6b86-121">Header</span></span>|<span data-ttu-id="a6b86-122">値</span><span class="sxs-lookup"><span data-stu-id="a6b86-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a6b86-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a6b86-123">Authorization</span></span>|<span data-ttu-id="a6b86-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="a6b86-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a6b86-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a6b86-125">Accept</span></span>|<span data-ttu-id="a6b86-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a6b86-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a6b86-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="a6b86-127">Request body</span></span>
<span data-ttu-id="a6b86-128">要求の本文に[deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="a6b86-128">In the request body, supply a JSON representation for the [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) object.</span></span>

<span data-ttu-id="a6b86-129">[DeviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="a6b86-129">The following table shows the properties that are required when you create the [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md).</span></span>

|<span data-ttu-id="a6b86-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a6b86-130">Property</span></span>|<span data-ttu-id="a6b86-131">型</span><span class="sxs-lookup"><span data-stu-id="a6b86-131">Type</span></span>|<span data-ttu-id="a6b86-132">説明</span><span class="sxs-lookup"><span data-stu-id="a6b86-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a6b86-133">id</span><span class="sxs-lookup"><span data-stu-id="a6b86-133">id</span></span>|<span data-ttu-id="a6b86-134">String</span><span class="sxs-lookup"><span data-stu-id="a6b86-134">String</span></span>|<span data-ttu-id="a6b86-135">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="a6b86-135">Not yet documented</span></span>|
|<span data-ttu-id="a6b86-136">notificationContent</span><span class="sxs-lookup"><span data-stu-id="a6b86-136">notificationContent</span></span>|<span data-ttu-id="a6b86-137">Binary</span><span class="sxs-lookup"><span data-stu-id="a6b86-137">Binary</span></span>|<span data-ttu-id="a6b86-138">このポリシーで検疫されたユーザーに送信される通知のテキストです。</span><span class="sxs-lookup"><span data-stu-id="a6b86-138">Notification text that will be sent to users quarantined by this policy.</span></span> <span data-ttu-id="a6b86-139">これは、UTF8 のエンコードされたバイト配列 HTML です。</span><span class="sxs-lookup"><span data-stu-id="a6b86-139">This is UTF8 encoded byte array HTML.</span></span>|
|<span data-ttu-id="a6b86-140">defaultAccessLevel</span><span class="sxs-lookup"><span data-stu-id="a6b86-140">defaultAccessLevel</span></span>|[<span data-ttu-id="a6b86-141">deviceManagementExchangeAccessLevel</span><span class="sxs-lookup"><span data-stu-id="a6b86-141">deviceManagementExchangeAccessLevel</span></span>](../resources/intune-onboarding-devicemanagementexchangeaccesslevel.md)|<span data-ttu-id="a6b86-142">Exchange の既定のアクセス状態。</span><span class="sxs-lookup"><span data-stu-id="a6b86-142">Default access state in Exchange.</span></span> <span data-ttu-id="a6b86-143">このルールは、Exchange 組織全体にグローバルに適用されます。</span><span class="sxs-lookup"><span data-stu-id="a6b86-143">This rule applies globally to the entire Exchange organization.</span></span> <span data-ttu-id="a6b86-144">可能な値は、`none`、`allow`、`block`、`quarantine` です。</span><span class="sxs-lookup"><span data-stu-id="a6b86-144">Possible values are: `none`, `allow`, `block`, `quarantine`.</span></span>|
|<span data-ttu-id="a6b86-145">accessRules</span><span class="sxs-lookup"><span data-stu-id="a6b86-145">accessRules</span></span>|<span data-ttu-id="a6b86-146">[deviceManagementExchangeAccessRule](../resources/intune-onboarding-devicemanagementexchangeaccessrule.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="a6b86-146">[deviceManagementExchangeAccessRule](../resources/intune-onboarding-devicemanagementexchangeaccessrule.md) collection</span></span>|<span data-ttu-id="a6b86-147">デバイスへのアクセスの一覧で Exchange ルールします。</span><span class="sxs-lookup"><span data-stu-id="a6b86-147">The list of device access rules in Exchange.</span></span> <span data-ttu-id="a6b86-148">アクセス ルールは、Exchange 組織全体にグローバルに適用します。</span><span class="sxs-lookup"><span data-stu-id="a6b86-148">The access rules apply globally to the entire Exchange organization</span></span>|
|<span data-ttu-id="a6b86-149">knownDeviceClasses</span><span class="sxs-lookup"><span data-stu-id="a6b86-149">knownDeviceClasses</span></span>|<span data-ttu-id="a6b86-150">[deviceManagementExchangeDeviceClass](../resources/intune-onboarding-devicemanagementexchangedeviceclass.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="a6b86-150">[deviceManagementExchangeDeviceClass](../resources/intune-onboarding-devicemanagementexchangedeviceclass.md) collection</span></span>|<span data-ttu-id="a6b86-151">Exchange に既知のデバイス クラスの一覧</span><span class="sxs-lookup"><span data-stu-id="a6b86-151">The list of device classes known to Exchange</span></span>|



## <a name="response"></a><span data-ttu-id="a6b86-152">応答</span><span class="sxs-lookup"><span data-stu-id="a6b86-152">Response</span></span>
<span data-ttu-id="a6b86-153">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="a6b86-153">If successful, this method returns a `200 OK` response code and an updated [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a6b86-154">例</span><span class="sxs-lookup"><span data-stu-id="a6b86-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="a6b86-155">要求</span><span class="sxs-lookup"><span data-stu-id="a6b86-155">Request</span></span>
<span data-ttu-id="a6b86-156">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="a6b86-156">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a6b86-157">応答</span><span class="sxs-lookup"><span data-stu-id="a6b86-157">Response</span></span>
<span data-ttu-id="a6b86-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="a6b86-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




