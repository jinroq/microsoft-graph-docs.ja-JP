---
title: windowsInformationProtectionAppLockerFiles のリスト
description: windowsInformationProtectionAppLockerFile オブジェクトのプロパティとリレーションシップをリストします。
ms.openlocfilehash: 1d765ad7c0ed09eda68ed8d2b08aa2a80986e424
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27066401"
---
# <a name="list-windowsinformationprotectionapplockerfiles"></a><span data-ttu-id="2b402-103">windowsInformationProtectionAppLockerFiles のリスト</span><span class="sxs-lookup"><span data-stu-id="2b402-103">List windowsInformationProtectionAppLockerFiles</span></span>

> <span data-ttu-id="2b402-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="2b402-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2b402-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2b402-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2b402-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="2b402-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2b402-107">[windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="2b402-107">List properties and relationships of the [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2b402-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="2b402-108">Prerequisites</span></span>
<span data-ttu-id="2b402-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2b402-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2b402-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2b402-111">Permission type</span></span>|<span data-ttu-id="2b402-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="2b402-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2b402-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2b402-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2b402-114">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="2b402-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="2b402-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2b402-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2b402-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2b402-116">Not supported.</span></span>|
|<span data-ttu-id="2b402-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2b402-117">Application</span></span>|<span data-ttu-id="2b402-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2b402-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2b402-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2b402-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/exemptAppLockerFiles
GET /deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/protectedAppLockerFiles
GET /deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}/exemptAppLockerFiles
GET /deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}/protectedAppLockerFiles
```

## <a name="request-headers"></a><span data-ttu-id="2b402-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2b402-120">Request headers</span></span>
|<span data-ttu-id="2b402-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2b402-121">Header</span></span>|<span data-ttu-id="2b402-122">値</span><span class="sxs-lookup"><span data-stu-id="2b402-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2b402-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2b402-123">Authorization</span></span>|<span data-ttu-id="2b402-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="2b402-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2b402-125">Accept</span><span class="sxs-lookup"><span data-stu-id="2b402-125">Accept</span></span>|<span data-ttu-id="2b402-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2b402-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2b402-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="2b402-127">Request body</span></span>
<span data-ttu-id="2b402-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="2b402-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2b402-129">応答</span><span class="sxs-lookup"><span data-stu-id="2b402-129">Response</span></span>
<span data-ttu-id="2b402-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="2b402-130">If successful, this method returns a `200 OK` response code and a collection of [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2b402-131">例</span><span class="sxs-lookup"><span data-stu-id="2b402-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="2b402-132">要求</span><span class="sxs-lookup"><span data-stu-id="2b402-132">Request</span></span>
<span data-ttu-id="2b402-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="2b402-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/exemptAppLockerFiles
```

### <a name="response"></a><span data-ttu-id="2b402-134">応答</span><span class="sxs-lookup"><span data-stu-id="2b402-134">Response</span></span>
<span data-ttu-id="2b402-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="2b402-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 317

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsInformationProtectionAppLockerFile",
      "displayName": "Display Name value",
      "fileHash": "File Hash value",
      "file": "ZmlsZQ==",
      "id": "d81f0e40-0e40-d81f-400e-1fd8400e1fd8",
      "version": "Version value"
    }
  ]
}
```




