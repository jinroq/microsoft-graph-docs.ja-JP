---
title: editionUpgradeConfigurations のリスト
description: editionUpgradeConfiguration オブジェクトのプロパティとリレーションシップをリストします。
ms.openlocfilehash: 1b60625a37fb95fefc5748b4feef460341d9ebc4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27022749"
---
# <a name="list-editionupgradeconfigurations"></a><span data-ttu-id="aecf7-103">editionUpgradeConfigurations のリスト</span><span class="sxs-lookup"><span data-stu-id="aecf7-103">List editionUpgradeConfigurations</span></span>

> <span data-ttu-id="aecf7-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="aecf7-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="aecf7-105">[editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="aecf7-105">List properties and relationships of the [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="aecf7-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="aecf7-106">Prerequisites</span></span>
<span data-ttu-id="aecf7-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="aecf7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aecf7-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="aecf7-109">Permission type</span></span>|<span data-ttu-id="aecf7-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="aecf7-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="aecf7-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="aecf7-111">Delegated (work or school account)</span></span>|<span data-ttu-id="aecf7-112">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="aecf7-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="aecf7-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="aecf7-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="aecf7-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="aecf7-114">Not supported.</span></span>|
|<span data-ttu-id="aecf7-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="aecf7-115">Application</span></span>|<span data-ttu-id="aecf7-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="aecf7-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="aecf7-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="aecf7-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="aecf7-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="aecf7-118">Request headers</span></span>
|<span data-ttu-id="aecf7-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="aecf7-119">Header</span></span>|<span data-ttu-id="aecf7-120">値</span><span class="sxs-lookup"><span data-stu-id="aecf7-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="aecf7-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="aecf7-121">Authorization</span></span>|<span data-ttu-id="aecf7-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="aecf7-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="aecf7-123">Accept</span><span class="sxs-lookup"><span data-stu-id="aecf7-123">Accept</span></span>|<span data-ttu-id="aecf7-124">application/json</span><span class="sxs-lookup"><span data-stu-id="aecf7-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="aecf7-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="aecf7-125">Request body</span></span>
<span data-ttu-id="aecf7-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="aecf7-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="aecf7-127">応答</span><span class="sxs-lookup"><span data-stu-id="aecf7-127">Response</span></span>
<span data-ttu-id="aecf7-128">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="aecf7-128">If successful, this method returns a `200 OK` response code and a collection of [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aecf7-129">例</span><span class="sxs-lookup"><span data-stu-id="aecf7-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="aecf7-130">要求</span><span class="sxs-lookup"><span data-stu-id="aecf7-130">Request</span></span>
<span data-ttu-id="aecf7-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="aecf7-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="aecf7-132">応答</span><span class="sxs-lookup"><span data-stu-id="aecf7-132">Response</span></span>
<span data-ttu-id="aecf7-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="aecf7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 560

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.editionUpgradeConfiguration",
      "id": "f39fc471-c471-f39f-71c4-9ff371c49ff3",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7,
      "licenseType": "licenseFile",
      "targetEdition": "windows10EnterpriseN",
      "license": "License value",
      "productKey": "Product Key value"
    }
  ]
}
```



